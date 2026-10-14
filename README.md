# Goal Grove

A calm goal tree for iPhone. Grow your goals from one root, sprout branches for the steps, and let Claude suggest how to get there.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest` | Makes it install as a full-screen app with its own name and icon |
| `sw.js` | Lets it open instantly and work offline |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | Home Screen icons |

## Put it online with GitHub Pages (free)

### Easiest: let Claude Code do it

Open this folder in Claude Code and say:

> Create a public GitHub repo called goal-grove from this folder, push it, and turn on GitHub Pages from the main branch root. Tell me the URL when it's live.

### By hand, on a computer

1. Go to github.com/new, name the repo `goal-grove`, set it to Public, and create it.
2. Click **uploading an existing file**, drag in every file from this folder, and commit.
3. Go to **Settings → Pages**, set Source to **Deploy from a branch**, then pick **main** and **/ (root)**, and save.
4. After a minute, the app is live at `https://<your-username>.github.io/goal-grove/`.

## Install on your iPhone

1. Open the GitHub Pages URL in **Safari**.
2. Tap **Share → Add to Home Screen → Add**.
3. Open **Goals** from your Home Screen. It runs full-screen, like a normal app.

## Turn on Claude

1. Get an API key at console.anthropic.com → API Keys, and add a few dollars of credit.
2. In the app, tap the **settings** button (top right) and paste the key.

Your key is stored only on your phone and is only sent to Anthropic. Each "Suggest steps" costs a fraction of a cent.

## Your data

Your goals are saved on your phone, inside the Home Screen app. Use **Settings → Save a backup** now and then, to Files or iCloud Drive. **Restore a backup** brings everything back, including on a new phone.

## Updating the app

Change `index.html`, push to GitHub, and the app picks up the new version the next time you open it with signal. If you change anything else (icons, `sw.js`), bump `CACHE` in `sw.js` (e.g. `goal-grove-v2`) so phones refresh their saved copy.
