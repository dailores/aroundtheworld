# aroundtheworld
Restaurant picker
# 🍽️ Tonight's Table — Cuisine Restaurant Finder

A beautiful single-page web app that lets you pick a cuisine and find a real local restaurant near you, powered by the Google Places API.

## Features

- 18 cuisines to choose from (Italian, Japanese, Mexican, and more)
- Real restaurant data via Google Places API
- Shows rating, price level, phone number, open/closed status, and website
- "Try another" button to shuffle results
- Works entirely in the browser — no backend needed

## Setup

### 1. Get a Google Places API Key

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a project (or use an existing one)
3. Enable the **Places API**
4. Go to **APIs & Services → Credentials** and create an API key
5. (Recommended) Restrict the key to the Places API and your domain

### 2. Run locally

Just open `index.html` in your browser — or use a local server to avoid CORS issues:

```bash
npx serve .
# or
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

### 3. Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your app will be live at `https://yourusername.github.io/repo-name`

> **Note:** The Google Places API blocks direct browser requests (CORS) when running from `file://`. It works fine on a proper domain like GitHub Pages or localhost with a server.

## Usage

1. Paste your Google Places API key into the field
2. Enter your city
3. Pick a cuisine
4. Click **Find a restaurant**
5. Hit **Try another** to get a different pick

## Files

```
index.html   ← the entire app, one file
README.md    ← this file
```

## License

MIT — do whatever you like with it.
