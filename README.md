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
| ✦ DIVISIBILITY CONNECT | Divisibility rules | Number | [Play](https://jakmann86.github.io/mathsgames/divisibility-connect) |
| ♠ TARGET ZERO | Integer addition | Number | [Play](https://jakmann86.github.io/mathsgames/target-zero) |
| ☢ MELTDOWN | Powers / indices | Number & Algebra | [Play](https://jakmann86.github.io/mathsgames/meltdown) |
| ✧ NUMBER BLASTER | Number properties | Number | [Play](https://jakmann86.github.io/mathsgames/number-blaster) |
| ▧ FRACTIS | Adding fractions | Number | [Play](https://jakmann86.github.io/mathsgames/fractis) |
| ★ JOHN'S PAINT SHOP | Ratio & proportion | Number & Algebra | [Play](https://jakmann86.github.io/mathsgames/johns-paint-shop) |
| ✶ QUICKDRAW | Factors, multiples, primes, fractions, decimals, %, ratio | Number | [Play](https://jakmann86.github.io/mathsgames/quickdraw) |
| ♥ BESSIE'S BAKERY | Scaling recipes (proportion) | Number & Algebra | [Play](https://jakmann86.github.io/mathsgames/bessies-bakery) |
| ☀ FUNCTIFORNIA GAMES | Functions: input/output, linear, quadratics, exponentials, logs, inverses | Functions | [Play](https://jakmann86.github.io/mathsgames/functifornia) |
| ✎ MATHS HANGMAN | Maths vocabulary (IGCSE + Year 12 word banks) | All topics | [Play](https://jakmann86.github.io/mathsgames/hangman) |
| ✈ FLYER² | Area of squares, rectangles, triangles, parallelograms, circles | Geometry & Measure | [Play](https://jakmann86.github.io/mathsgames/flyer-squared) |
| ◎ MX + CANNON | Coordinates on a straight line (y = mx + c) | Functions / Linear graphs | [Play](https://jakmann86.github.io/mathsgames/mx-plus-cannon) |

---

## 🗂️ Repo Structure

```
mathsgames/
├── index.html              ← Landing page (arcade homepage)
├── README.md               ← This file
├── johns-paint-shop/       ← Ratio game (single index.html)
├── quickdraw/              ← Shooting-gallery number game (single index.html)
├── bessies-bakery/         ← Recipe-scaling game (single index.html)
├── functifornia/           ← Six function mini-games (single index.html)
├── hangman/                ← Menu page + igcse/ and year12/ versions
├── flyer-squared/          ← Area flying game, 3 licences + night flight (single index.html)
├── mx-plus-cannon/         ← Human cannonball linear graphs game, 8 stages (single index.html)
├── divisibility-connect/, fractis/, meltdown/, number-blaster/, target-zero/
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

### ➕ Adding a new game

1. Make a new folder named after the game (lower-case, hyphens), e.g. `shipwreck/`.
2. Put the game in it as `index.html` (plus any css/js files it needs).
3. Add a `◀ ARCADE` link back to `../index.html`.
4. Copy a cabinet block in the root `index.html`, change the link, name, colours and description.
5. Add a row to the games table above.
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
John's Paint Shop: https://jakmann86.github.io/mathsgames/johns-paint-shop
```

---

*Built with p5.js, vanilla JS, and a lot of 80s arcade energy.*