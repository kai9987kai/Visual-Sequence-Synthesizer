
# Visual-Sequence-Synthesizer

A tiny, static **browser-based “visual sequence synthesizer”** prototype built as a single-page project (currently just an `index.html` in the repo). :contentReference[oaicite:0]{index=0}

At the moment, the UI copy indicates a simple workflow:

- **Synthesize** (generate/output a visual result)
- Choose an output **Style**
- Export as **PNG** or **JPEG** :contentReference[oaicite:1]{index=1}

> Status: early / minimal scaffold (good base for expanding into a real sequence/image synthesizer tool). :contentReference[oaicite:2]{index=2}

---

## What it’s for

Use this repo as a starting point for a lightweight web tool that can:
- generate/compose visuals in the browser (canvas/WebGL),
- step through or produce **sequences** (frames),
- export frames (PNG/JPEG),
- later: stitch frames into GIF/WebM, add “styles” (filters/presets), etc.

---

## Quick start

### Option A — open directly
1. Download / clone the repo
2. Open `index.html` in your browser

### Option B — run a local static server (recommended)
Some browser features (file saving, modules, fetch) behave better over HTTP.

**Python**
```bash
python -m http.server 8000
````

Then open:

* `http://localhost:8000`

**Node (http-server)**

```bash
npx http-server -p 8000
```

---

## Project structure

```text
Visual-Sequence-Synthesizer/
└── index.html
```

([GitHub][1])

---

## Roadmap ideas (if you extend it)

* Canvas pipeline: layer system (shapes/images/text) + deterministic RNG (seed)
* Sequencer/timeline: BPM, steps, easing curves, keyframes
* “Style” system: preset JSON (filters, palettes, noise params)
* Export:

  * individual frames (PNG/JPEG)
  * batch export (ZIP)
  * GIF/WebM encode (ffmpeg.wasm or MediaRecorder)
* GPU acceleration: WebGL / WebGPU render backend

---

## Contributing

PRs welcome:

* UI/UX (dark-mode synth controls)
* Rendering engine (Canvas/WebGL)
* Export pipeline (multi-frame)

---

## License

No license file is currently present in the repository—add one (MIT/Apache-2.0/GPL-3.0) if you want clear reuse terms. ([GitHub][1])

```
::contentReference[oaicite:5]{index=5}
```

[1]: https://github.com/kai9987kai/Visual-Sequence-Synthesizer "GitHub - kai9987kai/Visual-Sequence-Synthesizer"
