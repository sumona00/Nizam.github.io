# Personal website

Static single-page academic site. No build step, no dependencies.

## Deploy on GitHub Pages

1. Create a repository named `nusratnizam.github.io` (replace with your GitHub username — this exact name gives you `https://username.github.io`).
2. Put `index.html` at the repository root, alongside an `assets/` folder.
3. Push to the `main` branch.
4. Repository → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
5. The site is live in about a minute.

If you'd rather keep it in a repo named something else (e.g. `website`), the same steps work and the URL becomes `https://username.github.io/website`.

## Files to add

```
index.html
assets/
  profile.jpg        # square photo, at least 400×400
  Nusrat_CV.pdf      # your CV
```

## Before publishing

- `assets/profile.jpg` — the header image currently points here and will show an empty circle until you add it.
- `assets/Nusrat_CV.pdf` — the CV link.
- The GitHub link in the header is a placeholder (`https://github.com/`); swap in your profile URL.
- Every publication has a `<a href="#">Paper</a>` placeholder. Replace `#` with the DOI or arXiv URL, or delete the `<span class="pub-links">...</span>` for papers without a public link.

## Editing

- Accent color, text color, and content width are the CSS variables at the top of `index.html` (`--accent` is a deep carnelian).
- News: add a `<li>` to `#newsList`. Items with `class="hidden-item"` stay collapsed behind the toggle button — keep the six most recent visible.
- Sections are plain `<section>` blocks; delete one and remove its matching link in the `<nav>`.
