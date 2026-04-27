# Cat's Cradle Neon

`index.html` is a camera + MediaPipe demo. It needs to run from a real web origin:

- Works: `http://localhost`, GitHub Pages, Netlify, Vercel, Cloudflare Pages.
- Usually fails: `file://`, `gist.github.com`, direct raw Gist/GitHub URLs.

## Quick Local Run

```bash
python3 -m http.server 8000
```

Open:

```text
http://localhost:8000/
```

## Deploy

The safest free option is GitHub Pages:

1. Create a normal GitHub repository, not a Gist.
2. Upload `index.html` to the repository root.
3. In GitHub, open `Settings -> Pages`.
4. Select deployment from the `main` branch and `/root`.
5. Open the generated `https://USER.github.io/REPO/` URL.

If you must use a Gist, do not open `gist.github.com` directly. Use a static HTML proxy such as RawGithack by pasting the raw Gist URL into its converter. This is okay for testing, but GitHub Pages or Netlify is more reliable.
