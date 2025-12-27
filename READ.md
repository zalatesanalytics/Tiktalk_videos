# TikTok Amharic Daily Video Agent (GitHub Actions)

## What it does
- Rotates 1 story/day from `stories/1.txt ... 5.txt`
- Generates Amharic voice using Azure Speech
- Creates a 1080x1920 TikTok video (60 seconds) + burned subtitles
- Uploads the MP4 as a GitHub Actions artifact

## Setup
1) Add your 5 Amharic stories to `stories/1.txt ... 5.txt`
2) Put a vertical background video in `assets/background.mp4`
   - Tip: 1080x1920, 60s, loopable
3) Optional music: `assets/music.mp3`

## GitHub Secrets
Repo Settings → Secrets and variables → Actions → New repository secret:
- AZURE_SPEECH_KEY
- AZURE_SPEECH_REGION

## Run
- Automatic daily schedule via Actions
- Or manual: Actions → "Daily TikTok Video" → Run workflow

## Get the MP4
Actions → latest run → Artifacts → download `tiktok-output`
