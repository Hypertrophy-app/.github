<div align="center">

<img src="https://raw.githubusercontent.com/Hypertrophy-app/.github/main/assets/wordmark.png" alt="Hypertrophy" width="420" />

**Offline-first strength training for Android.**

<sub>[hypertrophy.app](https://hypertrophy.app) &nbsp;&middot;&nbsp; [Issues](https://github.com/Hypertrophy-app/hypertrophy-android/issues) &nbsp;&middot;&nbsp; [Releases](https://github.com/Hypertrophy-app/hypertrophy-android/releases)</sub>

</div>

---

Hypertrophy is a training log that keeps working in a basement gym with no
signal. Every set is written to the device first, every screen reads from local
storage, and the network is an optional convenience rather than a dependency.

## Repositories

| Repository | Description | Stack |
| --- | --- | --- |
| [`hypertrophy-android`](https://github.com/Hypertrophy-app/hypertrophy-android) | Android client and edge backend monorepo. | Kotlin, Compose, Room, Hilt, Ktor, Cloudflare Workers |
| [`hypertrophy-site`](https://github.com/Hypertrophy-app/hypertrophy-site) | Public site, including the legal pages Play Console requires. | HTML, CSS, GitHub Pages |
| [`hypertrophy-brand`](https://github.com/Hypertrophy-app/hypertrophy-brand) | Brand rules, store assets, listing copy, and Data safety answers. | Markdown, PNG |
| [`.github`](https://github.com/Hypertrophy-app/.github) | Organization profile and shared community health files. | Markdown |

## What ships

- **Training.** Exercise library, weekly planner, set builder, substitution and
  rescheduling engines, Health Connect export.
- **Coach.** On-device pose analysis through MediaPipe, rep and range-of-motion
  tracking, form faults, tempo, and an offline voice coach.
- **Squad.** Invite codes, live presence, group chat, and shared milestones,
  serialized through a Cloudflare Durable Object.
- **Progress.** Recovery map, 90-day consistency heatmap, PR trophy wall,
  estimated-1RM progression.

## Principles

1. **Offline first.** UI reads local storage only. Writes land locally, then
   drain through an outbox.
2. **Privacy first.** Camera frames are analyzed in memory and closed. Nothing
   raw is stored or transmitted.
3. **No paid utilities.** No paid APIs, no paid SaaS, no cloud build services.
   Pose detection, voice, and rendering run on the device.
4. **One design language.** Phoenix UI: Obsidian Forge and Daylight Ash, Space
   Grotesk, Plus Jakarta Sans, JetBrains Mono.

## Contributing

Read [`CONTRIBUTING.md`](https://github.com/Hypertrophy-app/hypertrophy-android/blob/main/CONTRIBUTING.md)
before opening a pull request. Report security issues privately as described in
[`SECURITY.md`](https://github.com/Hypertrophy-app/hypertrophy-android/blob/main/SECURITY.md).
