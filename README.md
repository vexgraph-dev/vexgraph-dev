# hey there, vex here!

just a dude writing serious C23 systems code in **very** unserious quantities.

pair-programming with an AI in a tight loop, building a whole ecosystem out of
pointers. everything is a pointer. no arrow sugar. no allocations on the hot
path. just vibes and `(*ptr).field`.

---

## current projects

- **anti** — 3D game engine. bindless, meshlets, physics. the name lives here and only here
- **semicolon** — mini IDE. tiny ~5MB jGRASP/Zed energy
- **samplerate** — bare-metal DAW. realtime mixer, spatial audio, 3D HRTF
- **darling-editor** — spatial studio. figma × miro on an infinite canvas, HTML/SVG export
- **drawling** — drawing studio. layers, brushes, flipaclip timeline energy

## under the hood

the apps above all sit on the same stack, so it isn't N projects — it's one ecosystem:

- **hotcwap** — kernel host. OS windows, dynamic hot-loader
- **vexspoke** — the spoke. memory arena, bitpool, dest-last math
- **graphvex** — GPU driver. vulkan/wgpu, fonts, sdf, meshlets
- **api-haven** — connectors. mcp / ai / db / assets
- **language** — grammar dylibs
- **darkbase** — native database store
- **darling-framework** — the UI toolkit + compositor
- **sesh** — session sync, VPS relay

## future projects

- something that reacts to you — still plotting
- a whiteboard that actually feels like a whiteboard
- whatever the next "that's a fun idea, let me build it" turns out to be

## the philosophy

- `(*ptr).field`, never `->` — a dereference is a memory hop and i want to see it
- one class per file. one problem in one file
- zero steady-state allocation. bounded waits everywhere
- every commit is buildable and bisectable, or it's not a commit
- teardown top-down, `Memory_freeAll` dead last

---

i have an ecosystem, you might wanna check it out → [**vexgraph-ecosystem**](https://github.com/vexgraph-ecosystem)

the constitution everything follows → [`preferences.md`](https://github.com/vexgraph-ecosystem/vexspoke/blob/main/preferences.md)