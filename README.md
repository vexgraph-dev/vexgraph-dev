# hey there, vex here!

just a dude writing serious C23 systems code in **very** unserious quantities.

pair-programming with an AI in a tight loop, building a whole ecosystem out of
pointers. everything is a pointer. no arrow sugar. no allocations on the hot
path. just vibes (if you think so, idc) and `(*ptr).field`. because `Object ptr = new Object();`

---

## current projects
the apps above all sit on the same stack, so it isn't N projects — it's one ecosystem:

- **[hotcwap](https://github.com/vexgraph-ecosystem/hotcwap)** — kernel host. OS windows, dynamic hot-loader
- **[vexspoke](https://github.com/vexgraph-ecosystem/vexspoke)** — the spoke. memory arena, bitpool, dest-last math
- **[graphvex](https://github.com/vexgraph-ecosystem/graphvex)** — GPU driver. vulkan/wgpu, fonts, sdf, meshlets
- **[api-haven](https://github.com/vexgraph-ecosystem/api-haven)** — connectors. mcp / ai / db / assets
- **[language](https://github.com/vexgraph-ecosystem/language)** — grammar dylibs and lsps
- **[darkbase](https://github.com/vexgraph-ecosystem/darkbase)** — native database store (spoke style)
- **[darling-framework](https://github.com/vexgraph-ecosystem/darling-framework)** — the UI toolkit + compositor
- **[sesh](https://github.com/vexgraph-ecosystem/sesh)** — session sync, VPS relay

## future projects

- **[anti](https://github.com/vexgraph-ecosystem/anti)** — a spatial ide, maybe a multimedia engine, or people call a **game engine**
- **[semicolon](https://github.com/vexgraph-ecosystem/semicolon)** — mini IDE. tiny jGRASP/Zed/JetBrains energy
- **[samplerate](https://github.com/vexgraph-ecosystem/samplerate)** — bare-metal DAW. realtime mixer, spatial audio, 3D HRTF
- **[darling](https://github.com/vexgraph-ecosystem/darling)** — spatial studio. figma × miro on an infinite canvas, HTML/SVG/Web export
- **[drawling](https://github.com/vexgraph-ecosystem/drawling)** — drawing studio. layers, brushes, animation, timelines

## the philosophy

- `(*ptr).field`, never `->` — a dereference is a memory hop and i want to see it
- one class per file, one problem in one file, solutions breed in one file
- zero steady-state allocation. bounded waits everywhere
- every commit is buildable and bisectable, or it's not a commit
- teardown top-down, `Memory_freeAll` dead last.

---

## i have an ecosystem, you might wanna check it out → [**vexgraph-ecosystem**](https://github.com/vexgraph-ecosystem)

### the constitution everything follows → [`preferences.md`](https://github.com/vexgraph-ecosystem/vexspoke/blob/main/preferences.md)