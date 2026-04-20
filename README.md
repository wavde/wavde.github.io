# wavde.github.io

Source for my personal site — [wavde.github.io](https://wavde.github.io).

Plain HTML + CSS, no build step. Edit `index.html` or `styles.css` and
push; GitHub Pages serves it automatically.

## Local preview

Open `index.html` directly in a browser, or run a one-liner server:

```powershell
python -m http.server 8000
# then visit http://localhost:8000
```

## Custom domain (later)

If/when a domain is registered (e.g., `wavde.dev`):

1. Add a `CNAME` file at the repo root containing just the domain.
2. Add DNS records at the registrar:
   - `A` records for `185.199.108.153`, `.109.153`, `.110.153`, `.111.153`
   - `CNAME` for `www` pointing at `wavde.github.io`
3. In repo settings → Pages → Custom domain, paste the domain and tick
   "Enforce HTTPS" once the certificate is issued.
