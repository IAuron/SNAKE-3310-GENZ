# SNAKE 3310 GENZ — Playables Certification Checklist

## Implemented in this candidate
- Responsive UI and resize handling
- Touch, mouse and keyboard input
- No in-game external links
- No in-game sharing prompt
- No in-game exit/quit button
- `firstFrameReady()` / `gameReady()` adapter
- `loadData()` before `saveData()`
- `saveData()` for progression
- `sendScore()` using the saved best score
- `isAudioEnabled()` / `onAudioEnabledChange()`
- `onPause()` / `onResume()`
- Original game visuals and assets
- Small initial asset set

## Before submission
1. Insert the exact official YouTube Playables SDK script supplied by the Developer Portal before game code.
2. Run the official Playables SDK Test Suite.
3. Verify cloud-save migration from previous save versions.
4. Test pause/resume and audio mute behavior on supported devices.
5. Test all aspect ratios and zero/near-zero WebView viewport startup behavior.
6. Validate metadata and required thumbnails in the Developer Portal.
7. Complete YouTube certification/review.

The current Google documentation requires the Playables SDK to load before game code, `firstFrameReady` before `gameReady`, cloud save through `loadData`/`saveData`, and SDK pause/audio callbacks. It also requires responsive touch/mouse support and prohibits in-game external links and sharing prompts.
