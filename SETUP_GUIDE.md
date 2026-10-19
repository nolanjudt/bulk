# Bulk Plan — Setup Guide

A **separate app** from Recomp: orange icon with one up arrow. It keeps its own
storage, so the two apps can't overwrite each other.

## 1. Host it at its own path

Put all 7 files in a **new folder** next to the Recomp one, for example
`.../bulk/`, and deploy the same way you deployed Recomp (GitHub Pages or Netlify
Drop). Don't put it in the Recomp folder, or one app replaces the other.

## 2. Install on iPhone

1. Open the new URL in **Safari**
2. Share → **Add to Home Screen**
3. Name it **Bulk** → Add

## 3. Bring your history over (once)

1. Open the **Recomp** app → History → **Export All Sessions to CSV** → save to Files
2. Open the **Bulk** app → History → **Import Recomp CSV** → pick that file

Every session comes across, and each exercise's newest session becomes its
"last time" reference. Importing the same file again doesn't duplicate anything.
Per-gym standing notes don't travel in the CSV; re-enter any you still want.

Keep Recomp installed until you've checked the import, then delete it whenever.

## Updating later

Replace `index.html`, bump `CACHE_NAME` in `service-worker.js`
(for example `'v2'` → `'v3'`), redeploy, then tap **Check for update** in the app.
