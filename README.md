# GOV Voice Teleprompter v3
Browser teleprompter with word-level voice tracking.

Important: Voice tracking uses the browser Web Speech API. Chrome/Edge/Safari support varies by device and language. The matching engine is client-side and searches a rolling speech window against the script, with whole-script recovery and mismatch hysteresis.

Deploy the three files to the repository root:
- index.html
- manifest.webmanifest
- sw.js
