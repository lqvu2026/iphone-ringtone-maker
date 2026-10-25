# iPhone Ringtone Maker

A single-page web app that turns any song into an iPhone ringtone (30 seconds max). Everything runs in the browser; no files are uploaded anywhere.

## Features
- Load MP3, M4A, WAV, etc.
- Drag on the waveform (or use sliders) to choose the start point and length (up to 30 s)
- Fade in / fade out
- Preview before exporting
- Export as **WAV**, **M4A** or **M4R**, with a custom file name
- Share / Save to Files, or Download

## Files
- `index.html` - the app
- `ringtone-maker-icon.png` - 180x180 Home Screen icon (referenced by `apple-touch-icon`)

## Publishing (GitHub Pages)
Commit `index.html` and the icon PNG, wait 1-2 minutes, then Add to Home Screen in Safari. If the old version still shows, delete the shortcut, quit Safari, reload and add it again.

## How to make a ringtone in GarageBand

1. **Open GarageBand.**

2. **Switch to Tracks view.**
   Choose Audio Recorder, then tap the Tracks view button (it looks like several horizontal tracks) near the top-left.

3. **Import your music.**
   - Tap the Loop Browser icon near the top-right, then select **Files**.
   - Tap **Browse items from the Files app**.
   - Find your WAV, MP3 or audio file.
   - Press and hold the file, then drag it into the tracks area.
   - If your song is in Apple Music, some protected or subscription tracks cannot be imported.

4. **Trim the section you want.**
   Drag the edges of the audio region to select the part you want for your ringtone. Keep it to 30 seconds or less to avoid compatibility issues. For example, select the chorus or your favorite piano passage.

5. **Export as a ringtone.**
   - Tap the downward arrow at the top-left.
   - Choose **My Songs**.
   - In the song browser, press and hold your project.
   - Tap **Share**.
   - Select **Ringtone**.
   - Name your ringtone and tap **Export**.

6. **Set it as your ringtone.**
   After exporting, tap **Use sound as** and choose **Standard Ringtone**. You can also assign it to a contact, or tap **Done** and set it later under Settings → Sounds & Haptics → Ringtone.

GarageBand can import AIFF, WAV, CAF, Apple Loops, AAC, MP3 and MIDI files. Files imported from iCloud Drive can be found under Files → Browse items from the Files app.

## Alternative: with a Mac
Export as M4R, then drag it onto your iPhone in Finder (Sounds, or the General tab). Pick it in Settings → Sounds & Haptics → Ringtone.

## Notes
- M4A/M4R export needs a browser with AAC encoding (WebCodecs): Safari 16.4+ or Chrome, plus the mp4-muxer library from a CDN. WAV export works everywhere.
- Make sure the exported file name ends in `.wav` / `.m4a`, not `.txt`.
