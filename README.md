# Birthday-flyer (Gyanna's Birthday Invite)

This repository contains a single-page invite with background video and music.

Want this repo to be a public website?

Option A — GitHub Pages (recommended, easy)

- Make sure this repository is pushed to GitHub (it already is).
- In your repository, go to Settings → Pages and set the source to the `gh-pages` branch (if using the Actions workflow below it will be created automatically) or to the `main` branch `/ (root)`.
- If you enable Pages from the `main` branch, the site will be published at `https://<your-username>.github.io/<repo-name>/` (may take a minute to publish).

Option B — Automatic deploy using GitHub Actions (this repo includes a workflow)

- The included workflow (in `.github/workflows/pages-deploy.yml`) will:
  - Build and deploy the repo root to the `gh-pages` branch whenever you push to `main`.
  - The site will then be available under `https://<your-username>.github.io/<repo-name>/`.

How to confirm the site is live

1. After pushing, go to the repository's Actions tab to ensure the `pages-deploy` workflow ran successfully.
2. Go to Settings → Pages and check the published site URL.

Optional: custom domain

- Add a `CNAME` file at the repo root containing your custom domain (one line).
- Configure DNS for your domain to point to GitHub Pages (A records or CNAME as GitHub docs describe).

Troubleshooting

- If audio/video don't autoplay on load, browsers may block autoplay with sound. Click the visible "Play Music" button on the page to start playback.
- If the site doesn't publish, check the workflow logs in Actions and ensure `gh-pages` branch has been created.

If you'd like, I can:
- Add a `CNAME` file and help configure DNS.
- Make the site use the main branch directly (no `gh-pages` branch), which is an alternative setup.
