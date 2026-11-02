# HabitGreen — App Store & website assets

## Website (static)
Open `index.html` (or host this folder on GitHub Pages / Netlify / any static host).

| Page | File |
| --- | --- |
| Home (Download button → App Store) | `index.html` |
| Privacy policy | `privacy.html` |
| Support (→ habitgreen@googlegroups.com) | `support.html` |

Once hosted, make the `og:image` / `twitter:image` URLs in `index.html` absolute
(e.g. `https://yourdomain/assets/og-image.png`) so link previews work, and use these URLs in App Store Connect:
Support URL → `…/support.html`, Privacy Policy URL → `…/privacy.html`, Marketing URL → `…/`.
Apple asks that the download button use its official badge; swap the CSS button for the badge from
<https://developer.apple.com/app-store/marketing/guidelines/> when you have a moment.

## Upload to App Store Connect (`store-assets/`)

| What | Where | Size |
| --- | --- | --- |
| iPhone 6.3" screenshots (6) | `screenshots/iphone-6.3in-1206x2622/` | 1206 × 2622 PNG |
| iPad 13" screenshots (6) | `screenshots/ipad-13in-2064x2752/` | 2064 × 2752 PNG |
| iPhone 6.3" app preview (29.6 s) | `app-preview/iphone-6.3in-886x1920.mp4` | 886 × 1920, 30 fps, H.264 + AAC |
| iPad 13" app preview (29.6 s) | `app-preview/ipad-13in-1200x1600.mp4` | 1200 × 1600, 30 fps, H.264 + AAC |
| **Header** | `header-and-search/header-5244x2950.png` or `header-3840x1646.png` | 5244 × 2950 / 3840 × 1646 |
| **Search result** | `header-and-search/search-result-5244x2950.png`, `-3840x2560.png` or `-1920x1280.png` | 5244 × 2950 / 3840 × 2560 / 1920 × 1280 |
| Web / social banners (not for App Store Connect) | `web-social/` (1500 × 500 banner, 1200 × 630 link preview) | — |

Each screenshot folder also has `plain/` with the raw, un-captioned screenshots.
The iPhone 6.3" set (1206 × 2622) also covers the 6.1" slot.
Order matters: the first three screenshots (and the preview video) show in App Store search results.

## Regenerating
`tools/` holds the scripts used (they use the simulators' IDs and `/tmp` working paths — edit before reuse).
The app has debug-only launch arguments for this: `-HG_SHOWCASE` (six sample habits, Pro on),
`-HG_OPEN detail-multi|share|stats|new|detail`, `-HG_DEMO` (scripted tour for the video).
