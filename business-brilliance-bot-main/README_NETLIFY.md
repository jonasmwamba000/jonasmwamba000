# Deploying to Netlify (free tier)

Follow these steps to deploy this Vite + React app to Netlify.

1) Prepare the repo

If your project is not yet in a Git repo, run:

```bash
git init
git add .
git commit -m "Initial commit"
# create a GitHub repo and add it as remote, then:
git remote add origin <your-git-url>
git push -u origin main
```

2) Create a Netlify site (recommended: connect to GitHub)

- Go to https://app.netlify.com/sites/new
- Choose "Import from Git" and connect your GitHub account.
- Select the repository you pushed above.
- Set the **Build command** to `npm run build` and **Publish directory** to `dist`.

3) Set Environment Variables in Netlify (Site settings → Build & deploy → Environment)

Add at minimum:

- `VITE_SUPABASE_URL` = your Supabase project URL
- `VITE_SUPABASE_PUBLISHABLE_KEY` = your Supabase anon/public key
- `VITE_ENABLE_GOOGLE` = `true` (optional — only if you have configured Google OAuth in Supabase and Google Cloud)

4) (Optional) Deploy using Netlify CLI (useful if you don't want to push to Git)

Install the CLI and run a one-off deploy:

```bash
npm i -g netlify-cli
npm run build
netlify deploy --prod --dir=dist
```

The CLI will guide you to link or create a site and will provide a Netlify URL for your app.

5) Verify

- Open your Netlify site URL. The app should load and API calls will use the `VITE_SUPABASE_URL` env var set in Netlify.
- If using Google OAuth, ensure the Netlify site origin (for example `https://your-site.netlify.app`) is added to:
  - Supabase Auth → Settings → External OAuth Providers → Google (Authorized redirect URLs)
  - Google Cloud Console OAuth 2.0 Client ID → Authorized redirect URIs

Troubleshooting
- If you see "Unsupported provider: provider is not enabled", verify:
  - The Google provider is enabled in your Supabase project
  - The Google OAuth client ID/secret are entered in Supabase
  - The redirect URI(s) exactly match the deployed origin
- Check Netlify build logs for build errors and the browser console / network tab for runtime errors.
