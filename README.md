# Workforce Improvement Lab

Productivity & Safety. AI-assisted tools for ideas, incident analysis, procedures, permits, shift handover, toolbox talks and gas training.

A prototype. It uses generic training values and fictional examples. It never approves work: a human decides.

## Files (all in the repository root)
- `index.html` : the whole app
- `sw.js`, `manifest.webmanifest`, `icon-*.png`, `apple-touch-icon.png` : install on a device and open without internet
- `version.json` : lets the app tell you when a new version is uploaded
- `lock-config.js` : the passcode file (starts in OPEN mode)

## The AI
Without a key the app runs in demo mode (ready examples). To turn the real AI on:
Settings > API key > paste your Anthropic API key > Save > Test.
The key stays in that browser only. Set a spending limit for the key in the Anthropic console. Never put the key in the repository.

## Your data
Everything you save stays on your device (a database in your browser) and is never sent to GitHub.
Use Library > Download backup file regularly. Restore with Library > Restore from backup file.

## Passcode (optional)
`lock-config.js` starts in OPEN mode. To protect the app, create a new `lock-config.js` with the passcode generator and replace this file. GitHub Pages sites are public, so use a long passphrase (3 or 4 words).

## Updating
Upload the new files over the old ones with the same names (Add file > Upload files). The app shows "A new version is available" and updates itself.
