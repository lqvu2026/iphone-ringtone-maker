# iPhone Ringtone Maker

A single-page web app that turns any song into an iPhone ringtone (30 seconds max). Everything runs in the browser; no files are uploaded anywhere.

## Features
- Load MP3, M4A, WAV, etc.
- Drag on the waveform (or use sliders) to choose the start point and length (up to 30 s)
- Fade in / fade out
- Preview before exporting
- Export as **M4R** (ringtone) or **M4A**, with a custom file name
- Share / Save to Files, or Download

## Files
- `index.html` - the app
- `ringtone-maker-icon.png` - 180x180 Home Screen icon (add your own; referenced by `apple-touch-icon`)

## Publishing (GitHub Pages)
Commit `index.html` and the icon PNG, wait 1-2 minutes, then Add to Home Screen in Safari.

## Using the ringtone on iPhone
- **With a Mac:** export M4R, drag it onto your iPhone in Finder, then Settings > Sounds & Haptics > Ringtone.
- **iPhone only:** export M4A, import it into GarageBand, then Share > Ringtone > Export.

## Notes
Needs a browser with AAC encoding (WebCodecs): Safari 16.4+ or Chrome. Uses the mp4-muxer library from a CDN.
