# Promod's Chess Academy — Website

A 4-page static site: `index.html`, `gallery.html`, `events.html`, `ratings.html`.
No build tools needed — plain HTML/CSS/JS, ready for GitHub Pages.

## Put this on GitHub Pages

1. Go to your repo `chess-academy` on GitHub.
2. Click **Add file → Upload files**, and drag in every file/folder from this
   package (`index.html`, `gallery.html`, `events.html`, `ratings.html`, the
   `css/`, `js/`, and `images/` folders). Commit directly to `main`.
3. Go to **Settings → Pages** (the page you had open earlier).
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. Wait 1–2 minutes, then refresh the Pages settings page — it will show
   your live URL, something like:
   `https://promodrajmoree.github.io/chess-academy/`

If the page doesn't load:
- Make sure the repo is **public** (private repos need GitHub Pro for Pages).
- Make sure `index.html` sits at the top level of the repo, not inside a
  subfolder — otherwise point the Pages folder setting to wherever it is.

## Editing content

- All real text (address, phone, email, bio, tournament dates) is marked with
  placeholder values like `—`, `DD Mon YYYY`, or `Add your...` — search for
  these and replace with your real details.
- To add real photos: drop image files into `images/`, then in `gallery.html`
  replace a `<div class="gallery-tile">...</div>` block with
  `<img src="images/your-file.jpg" alt="description">`.
- To link your rating and membership tools: open `ratings.html` and change the
  two `<div class="card">` blocks under "Full rating system" into links
  (`<a>` tags) pointing at wherever you host `Gulbarga_Rating_System.html`
  and `aicf-ksca-roster-check.html`.
- Shared header/footer are repeated in each page — if you rename or add
  pages, update the `<nav>` block in every file to match.

## Structure

```
chess-academy-site/
├── index.html
├── gallery.html
├── events.html
├── ratings.html
├── css/
│   └── style.css
├── js/
│   └── main.js
├── images/        (empty — add your photos here)
└── README.md
```
