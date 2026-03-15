
# Jane Du Personal Site (Static GitHub Pages)

This repository was generated with the help of GPT-5.3-Codex and Claude Code, March 14, 2026.

## Site Structure

- `index.html`: About page
- `publications.html`: Publications list
- `talks.html`: Talks list
- `teaching.html`: Teaching list
- `files.html`: Downloadable files page
- `data/content.json`: Main editable content source
- `assets/css/styles.css`: Site styles
- `assets/js/site.js`: Data loading and rendering logic
- `files/`: PDFs and downloadable documents

## Edit Content

Most updates happen in `data/<x>.json`:

- Update name, email, and biography in `profile`
- Add or edit publications in `publications`
- Add or edit talks in `talks`
- Add or edit teaching items in `teaching`
- Add downloadable files in `files`

Publication links support local and external hosting:

- `paperUrl`: primary link (local like `files/paper.pdf` or external URL)
- `localPaperUrl`: optional explicit local file link (preferred when set)
- `externalUrl`: optional conference/journal URL shown as an additional link

Use relative paths like `files/cv.pdf` for downloadable documents.

## Local Preview

From the repository root:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy on GitHub Pages

Use branch-based static hosting:

1. Go to GitHub repository `Settings` -> `Pages`.
2. Under `Build and deployment`, select `Deploy from a branch`.
3. Choose your main branch and `/ (root)` folder.
4. Save.

*Note:* to build correctly, ensure that `.nojekyll` is found in the root directory.

GitHub Pages will publish the root static files directly.
