# GOV Voice Teleprompter v4

Voice-following teleprompter for Hindi/Hinglish.

## v4 changes
- Whisper Local ASR using Transformers.js + multilingual Whisper Tiny.
- Runs speech recognition in the browser; no GOV server is required for transcription.
- Uses overlapping audio windows so short recognition errors do not immediately move the teleprompter.
- Whole-script matcher: local tracking + n-gram recovery + fuzzy token alignment.
- Handles skipped words, natural wording changes, ad-lib pauses, and backward re-sync better than v3.
- Browser Speech remains available as a lightweight fallback.
- Debug panel shows transcript, match score and matched position.

## GitHub Pages
Upload `index.html`, `manifest.webmanifest`, and `sw.js` to the repository root. Do not upload the ZIP itself.

## First use
1. Open the HTTPS GitHub Pages URL in Chrome.
2. Paste script and press **Load Script**.
3. Keep **ASR = Whisper Local**.
4. Press **Load Whisper** once and wait for the model to finish downloading/caching.
5. Press **Voice Start** and allow microphone access.
6. Open **Debug** if tracking needs inspection.

The Whisper model is downloaded from Hugging Face on first use. The model and Transformers.js runtime are third-party dependencies; GitHub Pages only hosts the app shell.
