# Changelog

## v1.1.0 — 2026-07-05

- Restructured both prompt files as proper coaching system prompts. Each now leads with **role → behavior rules → first turn**, followed by the framework as reference material for the coach. Paste the file whole into any LLM and it will immediately begin coaching, one section at a time.
- Removed the redundant "Master Prompt to Give the LLM" sections that were buried in the middle of each file (the whole file *is* the prompt now).
- Removed the `skills/` directory. Claude Skills bundles are out of scope for v1 — the plain markdown prompts work in every LLM.
- Added "Open in Claude" / "Open in ChatGPT" one-click deeplinks to the README. Links pre-fill a message asking the model to fetch and follow the raw prompt from GitHub.

## v1.0.0 — 2026-07-05

Initial release.

- Added `prompts/favorite-product.md` — coaching framework for the "What's your favorite product?" interview question.
- Added `prompts/root-cause-analysis.md` — coaching framework for metric-drop / RCA interview questions.
