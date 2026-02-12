# mathsgames
A place to store and share all the maths based games created for Northlands School. 
# ⚡ Jakmann's Arcade — IB Mathematics Game Centre

> Interactive mathematics games for IB students. Built for genuine engagement, not compliance.

🕹️ **Live site:** [jakmann86.github.io/mathsgames](https://jakmann86.github.io/mathsgames)

---

## 🎮 Games

| Game | Topic | IB Relevance | Link |
|------|-------|--------------|------|
| ⚡ TRANSFORM | Geometric Transformations | AA & AI — Geometry | [Play](https://jakmann86.github.io/mathsgames/transform-game) |
| *(coming soon)* | — | — | — |
| *(coming soon)* | — | — | — |

---

## 🗂️ Repo Structure

```
mathsgames/
├── index.html              ← Landing page (arcade homepage)
├── README.md               ← This file
├── transform-game/         ← Transformations game
│   ├── index.html
│   ├── css/
│   │   └── styles.css
│   └── js/
│       ├── game.js
│       ├── levels.js
│       ├── drawing.js
│       ├── transformations.js
│       ├── ui.js
│       ├── particles.js
│       └── sounds.js
└── [future-game]/          ← Each new game gets its own folder
```

---

## 🕹️ TRANSFORM — Geometric Transformations

**URL:** `jakmann86.github.io/mathsgames/transform-game`

A puzzle game where students move a cyan shape to match a pink target using geometric transformations.

**Features:**
- 30 levels across 6 worlds
- Translations, reflections, and rotations
- Par move system with star ratings
- Ghost trail on undo
- Out-of-bounds detection with move penalty
- Challenge mode (timed, unlocks after completing all levels)

**Worlds:**
1. Translations
2. Reflections  
3. Rotations
4. Mixed Transformations
5. Combined Transformations
6. Master Challenge

**IB Topics Covered:**
- Translation vectors
- Reflection across x = k, y = k, y = x, y = -x
- Rotation about the origin and arbitrary points (90°, 180°, 270°)
- Combining transformations

---

## 🚀 Running Locally

No build process needed — this is pure HTML/CSS/JavaScript.

```bash
# Clone the repo
git clone https://github.com/jakmann86/mathsgames.git
cd mathsgames

# Serve with any static file server
npx serve .
# or
python3 -m http.server 5501
```

Then open `http://localhost:5501` in your browser.

---

## 🌐 Deployment

This site is hosted on **GitHub Pages**.

To deploy updates:
```bash
git add .
git commit -m "describe your change"
git push
```

GitHub Pages automatically rebuilds within ~60 seconds of a push.

**Settings:** Repo → Settings → Pages → Branch: `main` → Root `/`

---

## ➕ Adding a New Game

1. Create a new folder: `mkdir new-game-name`
2. Build your game inside it with its own `index.html`
3. Add a new cabinet card to the root `index.html` (copy an existing cabinet block and update the content)
4. Push to GitHub — it's live

Each game's shareable URL will be:
```
https://jakmann86.github.io/mathsgames/new-game-name
```

---

## 🏫 Teaching Philosophy

These tools are built around a few principles:

- **Active over passive** — students build and solve from the start
- **Conceptual before procedural** — understanding *why* before mastering *how*  
- **Puzzles over problems** — multiple valid approaches, productive struggle
- **Place-based** — designed for an IB context in Buenos Aires

---

## 📋 Google Sheets Reference

For easy sharing with staff, paste these links directly into your resource spreadsheet:

```
Landing page:     https://jakmann86.github.io/mathsgames
Transform game:   https://jakmann86.github.io/mathsgames/transform-game
```

---

*Built with p5.js, vanilla JS, and a lot of 80s arcade energy.*