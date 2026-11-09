# Film Market Live
A satirical, film-industry-tabloid style news website (filmmarketlive.com) with joke articles about the short film MOOCH and the Rejecta Film Festival.

The owner isn't a developer: explain in plain language, keep steps short, and do the work rather than handing over commands where you can.

## What's here
- `index.html`: the homepage, with the article list and its own inline styles.
- One `.html` file per article (for example `mooch-wins-big.html`, `bond-casting.html`).
- `global-header.html`: the breaking-news banner shown at the top of every page.
- `sidebar.html`: the sidebar ads and "Trending" links shown on every page.
- `style.css`: shared styles for the article pages.
- `images/`: all pictures, plus the favicon and web-app icon files.
- `README.md`: the owner's personal git cheat sheet (not project docs). The README PDFs are copies of it.

## Run, build, deploy
- Static files, no build step.
- Every page loads `global-header.html` and `sidebar.html` with JavaScript `fetch()`. Opening a page by double-clicking the file won't show them; preview with a small local web server instead (for example `python3 -m http.server` in this folder, then open http://localhost:8000).
- The README mentions Netlify for publishing; the live site is filmmarketlive.com.

## Working on it
- Default branch: main. This repo is public: never commit keys, passwords, or private files. Keys go in a local .env, which stays out of git.
- Phone/cloud sessions work on a fresh copy from GitHub and hand back a branch to merge. Commit and push finished work.
- New article: copy an existing article page, rename it, update its title and social-share (`og:` and `twitter:`) tags, and add a link to it from `index.html`.
- To change the banner or sidebar on every page at once, edit `global-header.html` or `sidebar.html`, not each article.
- Social-share tags use full https://www.filmmarketlive.com/... image links, so new share images must be in `images/` and pushed before they show up in previews.
- Some image filenames contain spaces (for example `Best Lead 2.jpeg`); prefer simple lowercase-dash names for new ones.
- Don't commit `.DS_Store` files (Mac clutter).
