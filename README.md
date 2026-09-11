# hey there, vex here!

I build low-level systems software in pure C23 — a vertically integrated
multi-repo engine ecosystem where **everything is a pointer**. I work in tight
pair-programming partnership with an AI coding assistant, and the codebase is
engineered the way it is deliberately: explicit dereferences, one class per
file, zero steady-state allocation, and a living constitution that both of us
follow to the letter.

## what I'm building

The `vexgraph` ecosystem: a relational C23 runtime driven up through GPU
drivers, a retained UI toolkit and compositor, and a family of end-user
applications — an IDE, a DAW, a spatial studio, a drawing app, and a 3D game
engine.

```text
R1 Host        hotcwap        — Kernel, OS windows, dynamic hot-loader
R2 Behavior    vexspoke       — memory arena, BitPool, types, dest-last math
R3 Drivers     graphvex       — Vulkan/WGPU, fonts, SDF, meshlets
               api-haven      — MCP / AI / DB / asset connectors
               language        — LSP/grammar dylibs
               darkbase       — native vex database store
R4 Interfaces  darling-framework — retained UI toolkit, compositor
               sesh           — session sync, VPS relay
R5 Apps        semicolon      — mini IDE
               samplerate     — bare-metal DAW
               darling-editor — spatial studio
               drawling       — drawing studio
               anti           — 3D game engine
```

## how I work

- `(*ptr).field`, never `->` — a dereference is a memory hop and it stays visible.
- One class per file; every struct field gets a symmetric getter/setter.
- Dest-last. Two-layer access cap. Zero allocations on frame paths.
- Every commit is atomic, buildable, and owned by one logical feature.
- No auto-push unless I say so — history stays reviewable.

You can reach the whole thing under the
[`vexgraph-ecosystem`](https://github.com/vexgraph-ecosystem) organization.