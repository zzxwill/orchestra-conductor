# Orchestra Conductor

A webcam-driven orchestra conductor simulator in a single self-contained HTML file — no external libraries.

Wave your hand like a baton in front of the camera. Faster waving speeds the orchestra up, slower waving relaxes it, and putting your hands down stops the music. The orchestra plays *Twinkle Twinkle Little Star*.

- Motion detection by frame differencing on the webcam feed
- Instruments synthesized with the Web Audio API (strings, woodwinds, brass, timpani)
- Concert-hall stage where each section lights up as it plays
- Mirrored webcam view with detected motion drawn over it, live BPM, and the current lyric line

## Run locally

Open `index.html` in Chrome, or serve the folder:

```
python3 -m http.server 8000
```

Live: https://orchestra-conductor.zzxwill.workers.dev

Deploy with `npx wrangler deploy` (static assets from `public/`).

`PROMPT.html` is the original brief the app was built from.
