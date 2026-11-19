# DemoHero changelog

Paste the **App Store “What’s New”** block into App Store Connect when you upload a new build. Keep this file in version order, newest first.

---

## 0.1.1 — unreleased

### App Store “What’s New”

```
Free recordings no longer stop at 10 minutes. Free exports still stay 720p and now include a DemoHero watermark in the bottom-right corner. Pro can turn that watermark off, and still unlocks 1080p and 4K.
```

### Changes

- Removed the free-tier 10-minute recording cap.
- Free exports (and preview) show an app-logo + “DemoHero” wordmark at the bottom right.
- Pro can turn the wordmark off per take from the editor.
- Free vs Pro is now 720p + watermark vs 1080p/4K and optional watermark removal.

---

## 0.1.0 (2) — 8 September 2026

Commits: `f66e014`, `9281e23`.

### App Store “What’s New”

```
Region capture is easier to get right. Drag a rectangle, see its width and height, then drag the edges to resize before you confirm. Cancel and Confirm sit on the selection so they stay clear of the camera housing.

When you record a window or a region, the orange outline stays on screen so you can see the boundary. It is not included in the recording.
```

### Changes

- Region picker shows live pixel size (`width × height`).
- Drag region edges and corners to resize; drag inside to move; Confirm / Enter to capture.
- Confirm and Cancel sit on the selected region (not under the Mac camera housing).
- Window and region orange highlight stays visible during countdown and recording, and is excluded from the take.
- In-app Privacy Policy opens `https://demoheroapp.github.io/demohero/PRIVACY.md`.
