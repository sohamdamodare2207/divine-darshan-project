Divine Darshan — Deploy to Vercel

Quick options to deploy this static site:

1) Deploy with Vercel CLI (recommended)

- Install (if you don't have it):

```bash
npm i -g vercel
```

- Login and deploy from the project root:

```bash
vercel login
vercel --prod
```

The CLI will detect the static `index.html` and use the provided `vercel.json`.

2) Deploy via Vercel dashboard (GitHub/GitLab/Bitbucket)

- Push this repository to GitHub.
- In Vercel, click "Import Project" → select the repo.
- Set the root to the repository root (no build command; output directory empty).
- Deploy.

Notes:

- Static assets live in the `images/` and `audio/` folders. Ensure they are committed to the repo.
- If the mantra audio uses an external URL, confirm the remote host allows serving to your deployed domain.
- If you'd like, I can create a `package.json` and a GitHub repo for you and run the CLI steps locally (you'll need to authorize and provide access).
