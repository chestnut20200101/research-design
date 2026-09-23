# Research × Design

Final static website for the course project.

## Files

- `index.html` — website entry file
- `assets/` — images extracted from the original self-contained HTML for cleaner hosting and caching
- `.gitignore` — ignores common OS metadata files

## Deploy with Cloudflare Pages

1. Push this folder to a GitHub repository.
2. In Cloudflare Dashboard, open **Workers & Pages** → **Create application** → **Pages**.
3. Choose **Import an existing Git repository** and select the repository.
4. Use:
   - Production branch: `main`
   - Framework preset: None / no framework
   - Build command: `exit 0` (or leave empty if the UI permits)
   - Build output directory: `.`
5. Deploy. The site root must contain `index.html`.

## Deploy with Vercel

1. Import the same GitHub repository into Vercel.
2. Set Framework Preset to **Other**.
3. Leave the Build Command empty.
4. Use the repository root (`.`) as the output/static directory if Vercel asks for one.
5. Deploy.

Every future push to the production branch can trigger a new deployment after the Git integration is connected.
