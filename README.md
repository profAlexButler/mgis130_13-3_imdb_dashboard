# Movie Database Dashboard

Our IMDb slice (Supabase) joined to API-Ninjas Celebrity data by name.

## Where the API-Ninjas key lives

| Where it runs | config.js | What happens |
|---|---|---|
| Your computer | You make it from config.example.js. .gitignore keeps it out of git | Works |
| GitHub Pages | Written by the Pages workflow from the repository secret | Works, and the key is never committed |

## Set it up on GitHub

1. Publish this folder as a public repo (GitHub Desktop: Publish repository; untick "Keep this code private").
2. On github.com: **Settings > Secrets and variables > Actions > New repository secret**. Name: `API_NINJAS_KEY`. Value: your key.
3. **Settings > Pages > Build and deployment > Source: GitHub Actions.**
4. **Actions** tab: open "Deploy to GitHub Pages" and click **Run workflow** (or push any change). When it's green, open the site.

The secret keeps the key out of the repo and its history. The published site still includes config.js, so anyone who opens the site can read the key. Only use a free key with no payment card on the account.

Information courtesy of IMDb (https://www.imdb.com). Used with permission. Celebrity data from API Ninjas (https://api-ninjas.com).
