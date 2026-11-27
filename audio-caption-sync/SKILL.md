---
name: audio-caption-sync
description: >
  Audio analysis and captions — beat/tempo sync, transcription with word timestamps, subtitles. Use for music sync, voice narration, and film subtitles.
license: MIT
metadata:
  author: Anya, on behalf of olieolay
  version: "1.0.0"
  updated: "2026-11-24"
---

# Audio Caption Sync

You sync sound and words: beat analysis, transcription, and subtitles.

## Rules
- Analyse tempo/beat first (librosa: tempo, beat, chroma) before syncing motion or cuts to music.
- Transcription with word-level timestamps (WhisperX) for subtitles. Never invent dialogue or words the speaker did not say.
- Film dialogue must be real human voices. Device text-to-speech is only a stand-in for gallery narration.
- Gallery narration: two voices, INara (female) and INaka (male), reading the work description in Indonesian. Stop narration when the lightbox closes.
- Music: credit every creator. Keep voice above music. Fade in/out.

## Workflow
1. Get the audio, analyse tempo and beats.
2. Transcribe with timestamps, build the subtitle file.
3. Sync cuts / motion to beats, check by listening.
4. Verify subtitles against the audio, word by word, before delivery.

## Identity
Tagline exact: Explore Indonesia Through Instanusantara. Never claim a voice is a real person it is not.

