# antonincorinaldi.github.io

Personal website, served by GitHub Pages at https://antonincorinaldi.github.io

## Structure

```
.
├── index.html            # homepage
├── About.html            # pages (names kept so existing links keep working)
├── Research.html
├── Talks.html
├── Teaching.html
├── Outreach.html
├── CV.pdf                # kept at the root: linked from outside
├── assets/
│   ├── css/style.css     # single stylesheet shared by every page
│   ├── images/           # pictures used in the pages
│   └── talks/            # slides and posters (PDF)
├── _config.yml           # GitHub Pages config
└── google…html           # Google Search Console verification, do not delete
```

## Adding a talk

1. Put the PDF in `assets/talks/`, named `YYYY-MM_event_type.pdf`
   (e.g. `2026-11_action_dark_energy_talk.pdf`), so the folder sorts by date.
2. Copy a `<li>` block at the top of the `<ol class="timeline">` list in `Talks.html`:
   ```html
   <li>
     <time>Nov 2026</time>
     <div>
       <h3>Event name</h3>
       <p class="meta">City, Country</p>
     </div>
     <a class="pill" href="assets/talks/YYYY-MM_event_type.pdf" target="_blank" rel="noopener">Talk</a>
   </li>
   ```

## Changing the style

Edit `assets/css/style.css` only: every page uses it.
