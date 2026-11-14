# Live-Lightning-to-Audio-tracker
# AETHER // BOLT

Real-time global lightning visualization on a minimalist 3D globe paired with a generative Web Audio ambient synthesizer.

## Features
- **Live Blitzortung WebSocket Stream:** Connects to Blitzortung nodes with LZW frame decoding, plus an automatic/manual **Storm Simulator** fallback.
- **Minimalist 3D Globe:** Built with Three.js, custom GLSL Fresnel atmospheric scattering, and vector coastlines from `world-atlas`.
- **Generative Ambient Web Audio:** Maps lightning latitude to musical scales (Lydian, Minor Pentatonic, Hirajoshi, Dorian, Whole Tone), longitude to stereo panning, and multi-detector intensity to sub-bass thunder rumbles through a procedural convolution reverb and ping-pong delay.

## Running Locally
Because the app uses ES modules (`<script type="importmap">`), serve the directory over a local HTTP server rather than opening `index.html` via `file://`:

```bash
# Python 3
python3 -m http.server 8080

# Or Node.js
npx serve .
