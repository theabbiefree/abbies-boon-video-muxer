# abbies® Boon Video Muxer

**Combine your WebM video and music into a single post-ready MP4 — runs entirely in your browser.**

Drop your video. Drop your music. Hit Mux. Download your MP4.

⚡ **[Open the Muxer](https://theabbiefree.github.io/abbies-boon-video-muxer)**

---

## What It Does

Boon Video Muxer takes the WebM video from **abbies® Boon Video Studio** and your music file and combines them into a single MP4 — one file, ready to post to Instagram Reels, TikTok, YouTube Shorts, or anywhere else.

No upload. No account. No subscription. Your files never leave your machine. Everything runs inside your browser tab using ffmpeg.wasm — the full professional FFmpeg tool compiled to run locally.

---

## How To Use

### 1. Drop Your Files
- **Video** — drop the `.webm` file from your Boon Video Studio ZIP
- **Audio** — drop your music file (MP3, WAV, OGG)

### 2. Wait for ffmpeg
On your first visit ffmpeg.wasm downloads (~30MB) and is cached by your browser. The status panel shows when it's ready. Every visit after that is instant.

### 3. Hit Mux
Press **⚡ Mux to MP4** — ffmpeg combines your video and audio streams into a single optimised MP4 and downloads it to your machine.

That's it. Your MP4 is ready to post.

---

## The Two-Tool Pipeline

This tool is the second half of a two-part system:

```
abbies® Boon Video Studio
        ↓
   Export ZIP
   (WebM + music)
        ↓
abbies® Boon Video Muxer
        ↓
   Post-ready MP4
```

**[Boon Video Studio](https://theabbiefree.github.io/abbies-boon-video-studio)** generates your music-reactive video from your design images and exports a ZIP containing the WebM and your music file.

**Boon Video Muxer** (this tool) takes those two files and delivers a single finished MP4.

---

## Technical Notes

- **Input:** Any WebM video + MP3, WAV, or OGG audio
- **Output:** MP4 (H.264 video + AAC audio, web-optimised with faststart)
- **Video stream:** Copied directly — no re-encoding, no quality loss
- **Audio:** Encoded to AAC 192kbps — high quality, universally compatible
- **Duration:** `-shortest` flag keeps video and audio perfectly in sync
- **Powered by:** [ffmpeg.wasm](https://github.com/ffmpegwasm/ffmpeg.wasm) — FFmpeg compiled to WebAssembly
- **Requires:** Must be opened from a web server (GitHub Pages, localhost) — not a local `file://` path. This tool at `theabbiefree.github.io` works automatically.
- **No data leaves your machine** — all processing is local

---

## The abbies® Toolkit

| Tool | Description |
|------|-------------|
| [Boon Video Studio](https://theabbiefree.github.io/abbies-boon-video-studio) | Generate music-reactive videos from your images |
| [Boon Video Muxer](https://theabbiefree.github.io/abbies-boon-video-muxer) | Combine WebM + audio into a post-ready MP4 |
| [Boon Design Studio](https://theabbiefree.github.io/abbies-boon-design-studio) | Stamp and compose your kaleidoscope designs |
| [Pattern Boon Studio](https://theabbiefree.github.io/Pattern-Boon-Studio) | Upload, tile, watermark, export |
| [Image Boon Transformer](https://theabbiefree.github.io/Image-Boon-Transformer) | Bulk resize, watermark, and export |
| [Build-AI-Bare](https://theabbiefree.github.io/Build-AI-Bare) | Configure any AI assistant in 6 steps |

---

## License

MIT — free forever, use it, share it, build on it.

Built by **Abbie Free** in collaboration with Boon (Claude) · March 2026 · abbies® 🐻⚡🎨
