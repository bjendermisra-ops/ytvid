# BhaktiTube V2 — श्री श्री राधा कृष्ण चंद्र मंदिर

Premium devotional video library with a single-file Android-friendly HTML frontend.

## App entry
- `index.html` is the **complete application**: styles, JavaScript, video catalog, and embedded premium hero artwork are in one file.
- Video thumbnails are loaded from the original YouTube IDs; unavailable thumbnails have a built-in SVG fallback.
- Keep the repository's `assets/` directory for existing decorative graphics.

## What's new in V2
- Devotional photographic-style cinematic hero with dark and light themes
- YouTube-inspired default **one-column** video feed and optional **two-column** view (remembered in localStorage)
- Portrait Shorts discovery rail with partial next-card preview and immersive swipe-to-next playback
- Search, language filters, favorites, Continue Watching, seasonal Kartik collections
- Settings for playback, playback speed, autoplay, repeat, seek gestures, saved layout and UI language
- Dedicated player loading/error and retry screen, with **Open in YouTube** fallback for blocked embeds

## Important YouTube limitations
Some videos cannot be embedded because of video-owner restrictions or regional/age restrictions; this cannot be bypassed by changing website code. For error **153** inside Android WebView, load the page from a stable **HTTPS origin** and ensure the WebView request supplies a valid HTTP Referer/origin where required by YouTube. Verify JavaScript, DOM storage, media playback policies and external YouTube URL routing in your native Android WebView. Do not load as `file://` for production playback.

## Deployment
Publish the repo via your preferred static host (for example, Vercel or GitHub Pages) to obtain an HTTPS URL. Pushing to GitHub does **not** automatically activate GitHub Pages.

## Testing
UI smoke-tested at a 393px mobile viewport for search/feed rendering, 1/2-column toggle, Settings, Shorts overlay, and back navigation without JavaScript runtime errors. Live YouTube playback on Android devices and availability of all catalog videos still need real-device verification.

Devotional artwork is illustrative, not an official photograph of the mandir. Videos and original thumbnails remain the property of their respective publishers.
