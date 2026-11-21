# Tamanna's Birthday Website — Cloudflare Workers Static Assets

This project is a self-contained single-page HTML website. No dependencies or build steps are needed.

## Folder layout

```
public/
  index.html
wrangler.toml
```

## Deploy with GitHub connected to Cloudflare Workers

1. Upload `public/` and `wrangler.toml` to the **root** of your GitHub repository.
2. Open Cloudflare > Workers & Pages > your project > Settings > Builds.
3. Set the root directory to the repository root (`/`).
4. Leave **Build command** empty. If the dashboard requires a command, use `echo "No build required"`.
5. Set **Deploy command** to `npx wrangler deploy`.
6. Save, then redeploy the latest commit.

## Deploy from your machine

Run `npx wrangler deploy` from the directory containing `wrangler.toml`.

## Note

To change the Cloudflare worker name, edit `name` in `wrangler.toml`.
