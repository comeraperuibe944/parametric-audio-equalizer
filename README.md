# parametric-audio-equalizer

Interactive Web Audio API parametric equalizer with draggable frequency response curve nodes, real-time preview, and Linux EasyEffects JSON preset exporter.

## Overview

parametric-audio-equalizer is a standalone browser-based parametric curve designer built with the HTML5 Web Audio API and Tailwind CSS. It enables precise acoustic calibration directly in the browser and exports ready-to-use JSON presets for Linux EasyEffects (PipeWire).

Features:
- Multi-band biquad filter chain (peaking, low-shelf, high-shelf, notch, band-pass).
- Interactive 60 FPS HTML5 canvas displaying the combined frequency response curve with draggable control nodes.
- Integrated tone generator and audio file player for instantaneous A/B comparison.
- Full compatibility with Linux EasyEffects: directly exports presets formatted for PipeWire filter chains.
- Zero build dependencies: standalone single-file implementation.

## Usage

Simply open `index.html` in any modern web browser:

```bash
xdg-open index.html
```

Or serve locally:

```bash
python3 -m http.server 8080
```

## Presets

The repository includes standard baseline presets under `presets/`:
- `flat.json`: Reference 0 dB response.
- `bass_boost.json`: Low-frequency shelf enhancement.
- `vocal.json`: Mid-range vocal presence curve.

## License

MIT
