# Secret Santa

Simple static site for running a Secret Santa. The page lives at the repo root and can be served locally or deployed via GitHub Pages in minutes.

## Run Locally (Live Preview)

Use Python's built-in HTTP server:

```bash
python3 -m http.server 8000
$BROWSER http://localhost:8000
```

Notes:
- Any port works; `8000` is common.
- `$BROWSER` opens your default browser in this dev container environment; if it’s not set, just open `http://localhost:8000` manually.

## Deploy (GitHub Pages)

1. Push your changes to `main`.
2. In your GitHub repo: Settings → Pages.
3. Set Source to `Deploy from a branch`, Branch `main`, Folder `/ (root)`.
4. Save; wait a minute for the site to publish.
5. Your site will be available at:
	- `https://nguyen-trinhtk.github.io/secret-santa/`

Requirements for Pages:
- `index.html` must be at the repository root (already is).
- No build step needed; it's a static site.

## Project Structure

```
index.html
README.md
```

## Troubleshooting

- If the page doesn’t load locally, ensure the server is running and that port `8000` isn’t blocked.
- For GitHub Pages 404s right after enabling, wait a couple of minutes and refresh.