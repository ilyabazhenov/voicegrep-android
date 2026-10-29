<div align="center">

<img src=".github/assets/icon.png" alt="VoiceGrep" width="128" height="128">

# VoiceGrep for Android

**The meetings on your Mac, in your pocket.**

A companion to [VoiceGrep for Mac](https://github.com/ilyabazhenov/voicegrep-releases): meetings, transcripts,
participants and the assistant on your phone. Your Mac still stores and processes the meetings.

[![Version](https://img.shields.io/github/v/release/ilyabazhenov/voicegrep-android?label=version&color=0e7c6b)](https://github.com/ilyabazhenov/voicegrep-android/releases/latest)
![Android 10+](https://img.shields.io/badge/Android-10%2B-111111?logo=android)
![Requires VoiceGrep for Mac](https://img.shields.io/badge/requires-VoiceGrep%20for%20Mac-111111?logo=apple)
[![Obtainium](https://img.shields.io/badge/Obtainium-auto--updates-555555)](#updates)

**[Download the APK](https://github.com/ilyabazhenov/voicegrep-android/releases/latest)** ·
[voicegrep.com](https://voicegrep.com/#phone) ·
[Русский](README.md)

</div>

VoiceGrep on the Mac records calls, transcribes them on-device and recognizes who’s speaking by voice.
The Android app is a remote for that archive: open a meeting on the go, find what was agreed, name a new
speaker or record a meeting in a conference room. Every edit and recording goes to the Mac and is
carried out there.

This is a beta. The interface is in Russian.

## What it does

**Meetings**
- **Search meeting text.** A word from the conversation finds the line and opens the meeting right on it.
- **Transcript, recap and tasks** of each meeting; play back any line.
- **Filter by participant:** tap a person above the transcript to keep only their lines; “Подряд”
  (In a row) plays them one after another.

**Participants**
- **Name an unnamed voice** — all its lines move to that person, and the voice is recognized in future
  meetings.
- **Fix recognition:** move lines to another person or correct a name across all meetings.
- **People** — the list and cards of everyone you talk to.

**Assistant**
- **Questions about your meetings** — answered by the assistant on the Mac; conversations are shared
  with the Mac.
- **Daily recap:** what was decided, what you took on, what you were promised.
- Requires a language model connected in VoiceGrep on the Mac.

**In-room recording**
- The red button at the bottom records a meeting live. The recording travels to the Mac and is
  transcribed there like any call; the phone deletes its copy only once the Mac has it.

## Installation

1. Install [VoiceGrep for Mac](https://github.com/ilyabazhenov/voicegrep-releases) 1.12.0 or newer.
2. **[Download the APK](https://github.com/ilyabazhenov/voicegrep-android/releases/latest)** to your phone and open it.
   Android will ask you to allow installs from that source.
3. On the Mac: Settings → Данные → Телефон (Data → Phone), turn on Доступ с телефона (Phone access).
   It’s off by default.
4. In the same place, click Подключить телефон… (Connect phone…) — a QR code appears. Scan it in the app.
   The first time, the phone and the Mac must be on the same Wi-Fi; the code is single-use and valid
   for 5 minutes.

**Requirements:** Android 10 or newer; a Mac running VoiceGrep that is on and awake.

**Away from home** the phone connects through a relay (the Подключаться через relay switch in the same
Mac settings section).

## Updates

With [Obtainium](https://github.com/ImranR98/Obtainium): “Add App” → the address

```
https://github.com/ilyabazhenov/voicegrep-android
```

Obtainium finds new versions in this repository’s releases by itself. Without it, download the APK
from the [latest release](https://github.com/ilyabazhenov/voicegrep-android/releases/latest) and install it
over the old one.

## Privacy

The Mac stays in charge: meetings, audio and processing live there.

| What | Where |
|---|---|
| Call audio, transcription, voice recognition | on the Mac |
| Voiceprints | on the Mac, never sent to the phone |
| Meetings you’ve opened | a copy on the phone, so they open faster |
| In-room recording | on the phone until the Mac receives it |
| Sent to the cloud | **0 bytes**: the relay only passes encrypted data and can’t see meetings |

The link to the Mac is TLS 1.3, and the phone and the Mac know each other’s keys from pairing on.
Since the phone holds copies of transcripts, the app asks for your fingerprint, face or screen lock
when it opens (and after a minute in the background). To disconnect a phone, use Settings → Данные →
Телефон → Отозвать (Revoke) on the Mac: access ends immediately.

**Permissions:** Camera — to scan the QR code; Microphone — to record an in-room meeting;
Notifications — to show that a recording or an upload to the Mac is in progress.

## Feedback

Found a bug or have an idea — [message us on Telegram](https://t.me/ilyabazhenov).

## What’s in this repository

The app’s source is closed. This repository holds builds only:

| What | Where |
|---|---|
| `VoiceGrep-Android-<version>.apk` | [Releases](https://github.com/ilyabazhenov/voicegrep-android/releases) |
| Mac builds, website, update feed | [voicegrep-releases](https://github.com/ilyabazhenov/voicegrep-releases) |

<sub>Authenticity check: every APK is signed with the same key, certificate SHA-256
`D3:31:ED:88:87:A2:B7:75:B1:18:42:08:F4:4E:39:8F:6C:4A:8A:74:8F:C6:03:BA:C9:77:95:D8:99:FD:6C:2D`.</sub>

---

<div align="center">
<sub>VoiceGrep — local call recording and transcription. The phone is a remote; your data stays on your Mac.</sub>
</div>
