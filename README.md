# Dictate — releases

[Dictate](https://github.com/f1lcry) is a fast, private dictation and
meeting-transcription app for macOS: on-device Whisper transcription, a
notch HUD, a global hotkey with paste-at-cursor, and speaker-labelled
meeting transcripts. Your voice, recordings and transcripts never leave
your Mac.

**Download:** grab the latest `Dictate-x.y.z.dmg` from
[Releases](https://github.com/f1lcry/dictate-releases/releases/latest),
open it and drag Dictate to Applications. Requires macOS 26 (Tahoe) or
later on Apple silicon. Builds are code-signed and notarized.

The app updates itself via [Sparkle](https://sparkle-project.org);
`appcast.xml` in this repo is the update feed. Each version's notes are on
its Releases page and in the app's update dialog.

## What Dictate does

- **Dictation** — press the hotkey in any app, talk, and the polished text
  lands at your cursor. Mixed Russian/English, no time limit, nothing sent
  anywhere. A live transcript window, a compact HUD that unfurls from the
  MacBook notch, clipboard history.
- **Meetings** — drop a recorded meeting into the Meetings section and get
  a speaker-labelled transcript: you say how many people spoke, Whisper and
  on-device speaker detection do the rest. Talk time per speaker, search
  across every meeting, tap a timestamp to hear that moment, rename speakers,
  export Markdown / text / SRT. Summaries (overview, key points, action items,
  chapters) come from Apple Intelligence or any OpenAI-compatible server you
  configure — a Pro feature.
- **Meeting recording** (Pro) — record the meeting in Dictate: the
  microphone, the system audio of a Zoom / Meet / Teams call, or both, from
  the Meetings section, the menu bar or a global shortcut. Audio is written
  to disk as it happens and survives a crash; long meetings roll over into
  parts.

## Permissions

- **Microphone** — asked on the first dictation or recording.
- **Accessibility** — asked by the first hotkey dictation; it is what lets
  Dictate press ⌘V for you. Without it, finished dictations are copied to the
  clipboard instead of pasted.
- **System Audio Recording** — asked once by the first meeting recording that
  includes system audio (System Settings › Privacy & Security › Screen &
  System Audio Recording). If it is denied the recording contains silence
  rather than failing; Dictate points it out after a few seconds.

## Tiers

Free: dictation in the app window and menu bar, meeting import and
transcription. Pro (license key): meeting recording, meeting summaries, the
global hotkey, auto-paste at the cursor, clipboard history, AI cleanup.

## 0.4.0 highlights

- Meetings: import, speaker-labelled transcripts, talk time, search, export,
  per-meeting language (Auto / Russian / English) and model choice,
  summaries with Pro.
- Meeting recording (Pro): microphone, system audio or both; a floating
  capsule with timer and levels; crash-safe recordings that come back as
  *Recovered* after a crash; four-hour rollover into parts; an update that
  arrives mid-recording waits for the recording to stop.
- Settings › Meetings: record shortcut, default sources, permission status
  with a system-audio test, default language and model, speaker models,
  storage.
- Dictation: the phantom "Thank you." at the end of a dictation is gone;
  plain buttons have proper hit targets.
