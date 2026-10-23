# Changelog

All notable changes to Sorify are listed here. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), versions follow [Semantic Versioning](https://semver.org/).

## [1.0.0] - 2026-10-23

First public release.

### Added
- Desktop app: drag-and-drop queue for files and folders, live transcript preview, per-file status, language and timing.
- All Whisper models (`tiny` to `large-v3`, `turbo`), with download size, speed and GPU-memory hints; *Auto* picks `turbo` on a GPU and `base` on the CPU.
- 99 languages with auto-detection, *Translate to English*.
- Output formats: text paragraphs, timestamped text, SRT, VTT, TSV, JSON; save next to each file or into one folder; skip or overwrite existing transcripts.
- Advanced options: beam search / greedy, GPU / CPU, word-level timestamps, subtitle line width, vocabulary prompt, context carry-over switch.
- Windows installer (per user, no admin rights) that downloads PyTorch (GPU or CPU build, chosen from the NVIDIA driver), Whisper and ffmpeg into a private runtime.
- Explorer right-click menu *Transcribe with Sorify* for audio and video files; multiple files go to the open window.
- `sorify` command-line batch mode, optionally on PATH.
- Update check at launch with *Update now / Remind me later / Skip this version*; downloads are verified by SHA-256 before Setup runs.
- About dialog with engine details, component versions, log folder, Ko-fi and GitHub links, *Reinstall components*.
- Dark, light and system appearance.

[1.0.0]: https://github.com/AnthonyFararoni/Sorify/releases/tag/v1.0.0
