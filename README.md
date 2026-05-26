# PFL & MyPrize — 2026 Extension · Utility Folder

This folder contains all the supporting files for the **PFL & MyPrize 2026 Extension** microsite. It pairs with `index.html` (provided separately) to form the complete deployable site.

---

## How to deploy on GitHub Pages

### Step 1 — Set up your repo

1. Create a new repository on GitHub (e.g. `pfl-myprize-2026`)
2. Place **`index.html`** at the **root** of the repo
3. Place the **contents of this utility folder** alongside it, preserving the folder structure

Your repo should look exactly like this:

```
your-repo/
├── index.html                          ← the page (separate file)
├── .nojekyll                           ← from this utility folder
├── .gitignore                          ← from this utility folder
├── assets/
│   ├── logos/
│   │   ├── pfl-logo.png
│   │   └── myprize-logo.png
│   └── images/
│       ├── led-hero-crowd.jpg
│       └── led-product-detail.jpg
└── downloads/
    └── PFL_x_MyPrize_Terms_2026.pdf
```

### Step 2 — Enable GitHub Pages

1. In your GitHub repo, go to **Settings → Pages**
2. Under **Source**, choose **Deploy from a branch**
3. Branch: **`main`** · Folder: **`/ (root)`**
4. Click **Save**
5. Wait ~30 seconds. Your site goes live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

### Command-line alternative

If you prefer the terminal:

```bash
# In the folder containing index.html and the utility files
git init
git add .
git commit -m "Initial commit: PFL & MyPrize 2026 Extension"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then enable Pages from Settings as above.

---

## What's inside

| Path | Purpose |
|---|---|
| `.nojekyll` | Tells GitHub Pages to serve files as-is (skip Jekyll processing) |
| `.gitignore` | Standard ignore patterns for OS / editor files |
| `assets/logos/pfl-logo.png` | PFL logo with transparent background |
| `assets/logos/myprize-logo.png` | MyPrize logo with transparent background |
| `assets/images/led-hero-crowd.jpg` | LED activation hero — wide crowd shot at the barrier |
| `assets/images/led-product-detail.jpg` | LED activation detail — product close-up showing branding |
| `downloads/PFL_x_MyPrize_Terms_2026.pdf` | One-page A4 PDF terms sheet (linked from the page) |

---

## Editing later

**Swap an image or logo** — replace the file at the same path with the same filename. No code changes needed.

**Update the PDF** — replace `downloads/PFL_x_MyPrize_Terms_2026.pdf` keeping the filename.

**Update text or layout** — edit `index.html` directly. All copy is inline; search for the text you want to change.

---

## Brand notes

Built to PFL 2026 brand guidelines:
- **PFL Blue** `#052383`
- **PFL Red** `#ff0404`
- **PFL Grey** `#4d4d4d`
- **Display type** — Oswald (closest free web-font to PFL's licensed Druk)
- **Body type** — Saira (closest free web-font to PFL's licensed Eurostile)

Fonts are loaded from Google Fonts over the network — no font files bundled.

---

*Confidential — Draft for Discussion.*
