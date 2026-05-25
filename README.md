# Willow Whispers — Birth Tarot Widget

A self-contained, single-page tarot reading widget. Visitors enter their birth
month and day, watch a cinematic card-flip animation, and receive a
personalised reading drawn from the two (or three) Major Arcana cards
associated with their birth number — then opt in to a weekly written reading.

## Live demo

Deployed via GitHub Pages — open the repo's Pages URL.

## Stack

Pure static — no build step.

- HTML / CSS / vanilla JavaScript
- [Alpine.js](https://alpinejs.dev/) (loaded from jsDelivr CDN) for reactivity
- Google Fonts (Cormorant Garamond + Raleway)
- Tarot artwork in `tarot_card_images/`
- Email captures POST to an external n8n webhook

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploying to GitHub Pages

1. Push this folder to a GitHub repo.
2. Repo **Settings → Pages → Source: Deploy from a branch → `main` / root**.
3. The site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Project structure

```
.
├── index.html              # the entire widget
├── tarot_card_images/      # Major Arcana artwork (0.png, 2–22.png + back)
├── .gitignore
└── README.md
```
