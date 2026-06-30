# RE Pro Time Logger — Install as a Real App (GitHub Pages)

This turns your time-tracking app into something installable on your phone's
home screen, just like an app from the Play Store — no app store needed.

## Step 1 — Create a GitHub account (skip if you have one)
Go to https://github.com/join and sign up (free).

## Step 2 — Create a new repository
1. Go to https://github.com/new
2. Repository name: `re-time-logger` (or anything you like)
3. Set it to **Public** (required for free GitHub Pages)
4. Do NOT check "Add a README" — leave it empty
5. Click **Create repository**

## Step 3 — Upload the files
1. On your new repo page, click **"uploading an existing file"** (or the
   "Add file" → "Upload files" button)
2. Drag in ALL these files from this folder:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. Scroll down, click **"Commit changes"**

## Step 4 — Turn on GitHub Pages
1. In your repo, click **Settings** (top tab)
2. Click **Pages** in the left sidebar
3. Under "Build and deployment" → Source: select **Deploy from a branch**
4. Branch: select **main**, folder: **/ (root)** → click **Save**
5. Wait about 1 minute, then refresh the page — you'll see a green box with
   your live URL, something like:
   `https://yourusername.github.io/re-time-logger/`

## Step 5 — Install on your Motorola phone
1. Open that URL in **Chrome** on your phone
2. Tap the **three-dot menu** (top right)
3. Tap **"Install app"** or **"Add to Home screen"**
4. Confirm — the app icon now appears on your home screen
5. Opening it from the home screen launches full-screen, no browser bar,
   just like a normal app

## Step 6 — Set up Google Sheets sync
1. Open the installed app
2. Tap the ⚙ settings icon (bottom right)
3. Tap **"Google Sheets sync"**
4. Tap **"Sign in with Google"**
   - First time only: it will ask for a Google OAuth Client ID. Follow the
     on-screen instructions to create a free one at
     https://console.cloud.google.com (APIs & Services → Credentials →
     Create OAuth 2.0 Client ID → Web application → add your GitHub Pages
     URL to "Authorized JavaScript origins")
5. Once signed in, paste your Google Sheet ID (or tap "Create a new sheet
   for me") and tap **Save & test connection**

That's it — every time entry you log will now automatically back up to
your Google Sheet.

## Updating the app later
If you ever want changes/updates, just re-upload the changed file(s) on
GitHub (Add file → Upload files → same filenames will overwrite). Your
phone's installed app will pick up the update automatically next time
you open it.
