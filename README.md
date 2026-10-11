# Lullo

A private, before-bed video journal for macOS. Talk the day down.

Each night Lullo asks you three questions and records a short video of your answer. Your nights collect in a calendar you can look back on, with transcripts made on your own Mac. Nothing is uploaded, ever. Everything lives in `~/Lullo`.

## Download

**[Download Lullo for Mac](https://github.com/abdullahridwan/lullo-releases/releases/latest/download/Lullo.dmg)** (Apple Silicon, macOS 12 or later)

All versions are listed under [Releases](https://github.com/abdullahridwan/lullo-releases/releases).

## Install

1. Open `Lullo.dmg` and drag Lullo into Applications.
2. Lullo is not notarized by Apple yet, so macOS blocks the first launch. Right-click Lullo, choose Open, then Open again. If macOS still refuses, go to System Settings, Privacy & Security, and click Open Anyway.
3. Allow camera and microphone access when asked.

## Transcripts (optional)

Transcripts run locally with whisper.cpp. One-time setup:

```bash
brew install whisper-cpp
mkdir -p ~/Lullo/models
curl -L -o ~/Lullo/models/ggml-base.en.bin https://huggingface.co/ggerganov/whisper.cpp/resolve/main/ggml-base.en.bin
```

## Privacy

Lullo has no accounts, no analytics and no servers. Your videos, questions and transcripts are plain files on your computer.
