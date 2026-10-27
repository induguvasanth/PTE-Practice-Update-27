# PTE Practice — Deployment and Maintenance

## GitHub Pages
Upload the contents of this project folder to the publishing directory of your GitHub Pages repository. Keep all HTML, JS, and `pronunciation-assets/` files together. GitHub Pages must use HTTPS for microphone access.

## Browser Whisper
The `browser-whisper-worker.js` worker runs Whisper locally on mobile/tablet after recording. It downloads model assets on first use. The PC speech recognition implementation remains in the page scripts. Do not delete `browser-whisper-worker.js`, `browser-acoustics.js`, `whisper-config.js`, or `pronunciation-assets/`.

## Student progress
Keep `student-progress.js`, `cloud-sync.js`, `student-auth.js`, `sync-config.js`, and `Google-Apps-Script/`. Before changing the Apps Script deployment, back up the existing Google Sheet. Deploy `Code.gs` and `Bridge.html` to the existing script project, verify its URL in `sync-config.js`, then test login, completed questions, score saving, and retrieval from a second device.

## Scoring
Keep `pte-mcq-scoring.js`, `task-scoring.js`, `free-evaluator.js`, `pronunciation-evaluator.js`, and related assets. Test multiple-answer partial credit and speaking scoring before student use.

## Removed items
Old update-by-update guides, optional Python/Whisper server experiments, build-time pronunciation source, duplicate reference files, and obsolete change manifests were removed. This does not delete or change data in your Google Sheet.

## Verification
Files were retained based on the current static website references and required assets; this cleanup is not a full browser/device regression test.
