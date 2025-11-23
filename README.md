# Editor Refactor (web-ready)

This project is a refactored web-ready version of the editor with:
- Stickers (packs) + drag to move + remove (double-click)
- Green Screen (chroma key) demo
- Face Tracking (tfjs face-landmarks-detection)
- Body Slim demo (slice-based warp using BodyPix segmentation)
- Video filters via ffmpeg.wasm (lazy-loaded)
- AI Avatar generator (client-side posterize demo)

## Quick start

1. Install Node.js (LTS)
2. Install deps:
   ```
   npm install
   ```
3. Run dev server:
   ```
   npm run dev
   ```
4. Open http://localhost:5173

## Build
```
npm run build
# preview production
npm run preview
```

## Notes & Limitations
- TFJS models and ffmpeg.wasm are large; they load lazily. Expect delays on first use.
- Body-slim is a demo—quality is not production-grade.
- For heavy video work, prefer server-side ffmpeg.
- If you want, I can open a PR to your GitHub repo merging these changes.

