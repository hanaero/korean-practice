# 조각 · Jogak — Korean in Pieces

A small, standalone Korean learning web app built for visual, explanation-first learning. No dependencies, accounts, or paid APIs.

## Try it

Open `index.html` in a desktop browser. The app is mobile-friendly, but for reliable use on an iPhone it's better to host it on a static website (see below), rather than previewing an HTML file inside the Files app.

## What's included

- **Four short lessons**, with 12 example sentences in Korean.
- **Tap-to-explain word pieces**: nouns, particles, and verbs, with plain-English explanations and particle-form rules.
- **Consistent particle colours:** subject = green, object = coral, topic = blue, place/direction = purple. The app also labels roles in words, not only colour.
- **Three stages of support:** guided colour backgrounds, colour-only markings, and natural Korean.
- **20 short practice questions** across the four lessons. Hints and skips are allowed; there are no penalties.
- **Local progress tracking** using your browser's `localStorage` when permitted.

## Publish on GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html` at the repository root and commit it to `main`.
3. Open the repository's **Settings → Pages**.
4. Select **Deploy from a branch**, choose `main` and `/ (root)`, then save.
5. Visit the GitHub Pages URL provided in the repository settings. Open it in Safari on your phone.

This publishes the file as a static website. If the repository is public, the source and lesson content will be public; no personal progress is sent to the site because it is stored in the browser.

## Editing lesson content

Open `index.html` in a text editor. Inside its `<script>` block:
- `sentences` defines the Korean example phrases, translations, and segments.
- `lessons` defines the lesson sequence and explanation.
- `questions` defines the practice prompts and answers.

Everything is plain HTML, CSS, and JavaScript for easy experimentation. No framework or install step is required for this prototype.

## Current limitations

- There is no audio or spaced-repetition scheduler yet.
- Progress is tied to the current browser and site origin, not synced between devices.
- Sentence content has been manually curated; it is not a general-purpose Korean parser.
- The app is designed for learning common particles, not as a complete Korean grammar reference.
