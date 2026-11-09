# Article Studio

A single-file HTML dashboard to polish articles with the **Gemini API** and hand them off to **Google NotebookLM**, with a tailored prompt for every task.

- Article library with status, search and word counts (stored in your browser)
- 8 task templates: polish, simplify, restructure, SEO pack, summary, fact-check flags, translate, social posts (all editable, add your own)
- **Build tailored prompt with Gemini**: Gemini reads your article and writes the best prompt for the chosen task
- Run the task, view the result and a word-level diff, then apply it to the article
- NotebookLM hand-off: export selected articles as Markdown sources and copy a source-grounded prompt (NotebookLM has no public API for personal accounts)

## Use
1. Enable GitHub Pages: Settings → Pages → Source: **GitHub Actions** (the included workflow deploys on every push to `main`).
2. Open the site → **Settings** → paste a key from https://aistudio.google.com/apikey.

## Security
The key lives only in your browser's localStorage and is sent only to `generativelanguage.googleapis.com`. Never commit a key. Restrict it to your site's HTTP referrer in Google Cloud.
