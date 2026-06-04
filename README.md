# NorskOrd — AI Vocabulary Builder

A Norwegian (Bokmål) vocabulary tool built through iterative LLM collaboration. Look up any word or phrase and get a full linguistic entry — translation, IPA, all inflected forms, example sentences, grammar notes, and register (formal / informal / slang) — then save what you're weak at and track high-frequency-word progress.

## Demo mode vs full version

The hosted demo covers a fixed, curated set of words that work instantly with no API key and no cost, so anyone can try the full interface. To look up *any* word, add your own Anthropic API key — it is stored only in your browser (`localStorage`) and used only for your own lookups. No key is bundled in this code.

## How it works

- A single self-contained `index.html` — no build step, no dependencies.
- State (your saved words and progress) persists in the browser via `localStorage`.
- Live lookups call the Claude API with a structured-output prompt. The model returns a JSON linguistic entry that the app renders into the word card.

## Features

- **Lookup** — translation, IPA, word class and gender, full inflected forms, two example sentences, a B1-level grammar note, register tag, and tappable related words.
- **My Words** — a filterable bank of saved entries, with one-click JSON export for backup.
- **HFW Progress** — track your way through the most common Norwegian words in tiers and sets.

## Tech

HTML, CSS, vanilla JavaScript, Claude API.

---

Built by [@kspinghar](https://github.com/kspinghar).
