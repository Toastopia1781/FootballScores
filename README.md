
# RJ Soccer Scoreboard

A self-updating scoreboard for your soccer clubs. It auto-refreshes every 60 seconds and shows LIVE/UPCOMING/FINAL with local times.

## How to host (GitHub Pages — free)

1. Create a GitHub account (if you don't have one).
2. Click **New repository**. Name it e.g. `rj-scoreboard` and make it **Public**.
3. Upload the two files from this ZIP: `index.html` and `README.md`.
4. In your repo, go to **Settings → Pages**.
5. Under **Build and deployment**, choose:
   - **Source**: *Deploy from a branch*
   - **Branch**: `main` and `/ (root)`
6. Click **Save**. Wait ~1 minute.
7. Your live URL will be shown at the top of the Pages section. It will look like:
   `https://<your-username>.github.io/rj-scoreboard/`

## How to host (Netlify — free)

1. Go to https://www.netlify.com/ and sign up.
2. Click **Add new site → Deploy manually**.
3. Drag-and-drop the folder (or the ZIP contents) onto Netlify.
4. Netlify will give you a live URL like `https://rj-scoreboard.netlify.app/`.

## Local quick preview (no hosting)

If you prefer to run it locally without CORS issues:
- On your computer, open a terminal in the folder containing `index.html`, then run:

```
python -m http.server 8000
```

- Open your browser to `http://localhost:8000`

## Editing teams

- The team list and aliases are inside `index.html` near the top of the script, in `TEAM_ALIASES`.
- You can add/remove teams or change names there and re-upload the file.

## Notes

- The page fetches public data from TheSportsDB. If you see "Network/CORS error", host it using one of the methods above.
- Badges are added to a subtle wallpaper behind the cards as they load.
