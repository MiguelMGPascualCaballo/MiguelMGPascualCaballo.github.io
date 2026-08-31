# Pascual-Caballo — personal website

Static academic website (plain HTML/CSS, no frameworks) meant to be published on GitHub Pages.

## Structure

```
.
├── index.html            Home / bio
├── research.html         Research areas
├── publications.html     List of publications
├── cv.html                Summary CV + download link
├── contact.html           Contact and links (ORCID, arXiv, Scholar...)
├── assets/
│   ├── css/style.css
│   ├── cv/                Put your CV PDF here
│   └── img/                Photos or other images
└── .nojekyll
```

All current content (university name, publications, awards, links) is **placeholder content**.
Edit the `.html` files directly and replace it with your real information.

## Publishing on GitHub Pages

1. Create a GitHub repository named exactly `YOUR-USERNAME.github.io`
   (replace `YOUR-USERNAME` with your actual GitHub username).
2. From this folder:

   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Source → Deploy from a branch → main / (root)**.
4. Your site will be published at `https://YOUR-USERNAME.github.io/` (may take 1-2 minutes).

## Before publishing

- [ ] Replace `YOUR-USERNAME` in `contact.html` with your real GitHub username.
- [ ] Fill in `assets/cv/cv-pascual-caballo.pdf` with your actual CV.
- [ ] Edit bio, research, publications and CV with your real data.
- [ ] Update the contact email in `contact.html`.
- [ ] (Optional) Add a real photo in `assets/img/` and replace the initials avatar
      in `index.html` with an `<img>` tag.
- [ ] (Optional) Set up a custom domain under **Settings → Pages → Custom domain**.

## Local development

No build step required. To preview:

```bash
python3 -m http.server 8000
```

then open `http://localhost:8000`.
