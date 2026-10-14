# Brightpath — Safer AI, together

## Download the source

The complete project is bundled in `brightpath-repository.zip` in this repository. Download and extract it to access the `dist/`, `extension/`, `tests/` and `assets/` folders. Run the commands below from the extracted `brightpath` folder.

[Live demo](https://brightpath-family-ai.majorauk256.chatgpt.site)


A hackathon MVP for families with children aged approximately 10–15. Original child and parent mini lessons teach privacy, verification, deepfakes, healthy AI boundaries, kindness and help seeking. A companion Manifest V3 Chrome extension gates selected new visits until its bundled privacy mini module is passed. The website includes a labelled interactive simulation and an 80-second captioned video.

## Run

From this directory: `python3 -m http.server 8000 --directory dist`, then visit http://localhost:8000.

No build, API key or server database is required. Source: `dist/index.html`, `dist/style.css`, `dist/app.js`.

## Demo

Use the demo home page to choose Parent login or Child login. Open Chrome extension in the sidebar to download the extension, try the interactive simulation and watch the captioned video. See extension/README.md for installation and live Chrome checks. The video uses captured simulation UI frames, not live installed-extension enforcement footage.

## Scope and honesty

This website cannot block other websites or installed applications. The packaged extension redirects new top-level visits to example.com and chatgpt.com only. Role selection is not authentication. Local storage can be changed or cleared. There is no remote parent-child synchronisation. Real enforcement requires a protected parent account, pairing, a browser extension or platform-specific device controls. Support remains accessible regardless of lesson status. External services may have age restrictions; the launcher is not a certification of suitability.

The MVP teaches about AI; it does not call an AI model or automatically detect harmful content. To strengthen AI relevance in a future version, add vetted adaptive scenarios with age-appropriate guardrails, evaluation and human oversight. Do not claim automated detection or effective device blocking in the submission.

No chats, names or browsing history are collected. Local storage contains completion IDs, gate settings, unlock expiry and agreement choices. Google Fonts requests are external. No analytics included.

## Evaluation before wider use

Test comprehension and accessibility with consenting families. Measure scenario accuracy before/after lessons, successful help-route access, and usability of retry/unlock flows. Avoid claiming demonstrated impact without a study. Evaluate unintended consequences including coercive gate use, inaccessible quiz content and false confidence.

## Background

Original content draws on UNICEF's child privacy, literacy and safety principles:
- https://www.unicef.org/protection/keeping-children-safe-online
- https://www.unicef.org/innocenti/projects/ai-for-children

## Submission

This repository includes the family app, installable Chrome extension demo, and an 80-second captioned simulation video at `dist/brightpath-extension-demo.mp4`. The video is not a recording of installed Chrome enforcement.

## Repository layout and checks

- `dist/`: website and downloadable demos
- `extension/`: unpacked Manifest V3 extension and installation guide
- `tests/extension-lifecycle.cjs`: mocked Chrome lifecycle checks
- `assets/`: presentation thumbnail

With Node.js installed, run `npm test` and `npm run check`. No npm dependencies are required.
