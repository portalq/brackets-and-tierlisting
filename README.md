# Brackets and Tierlisting

Run head-to-head brackets and tier lists yourself — no chat voting needed. Works with images, YouTube videos and Twitch clips.

**Use it:** https://portalq.github.io/brackets-and-tierlisting/

## Features

- **Brackets:** two options at a time; click a card or press `1` / `2` to pick. Byes are handled automatically, and you can view the full bracket tree at any point.
- **Tier lists:** one option at a time; click a tier to place it. Drag tiles between tiers at the end (or tap a tile, then a tier label).
- **Videos:** YouTube links play inside the cards (`Q` / `E` in brackets, `V` in tier lists). Timestamps like `&t=1m30s` are respected.
- **Import:** paste JSON, a list of `Name | image URL | link` lines, or a list of YouTube/image links, or add image files from your computer.
- **Export:** each bracket can be exported as JSON to back it up or share it.
- `Z` undoes the last pick in either mode.

Brackets are saved in your own browser, so each person keeps their own library. To share a bracket, use **Export** and send the JSON; the other person pastes it into **Import**.

## OBS

Add a **Browser** source pointing at the link above.

## Running it offline (Windows)

YouTube won't play videos in a page opened straight from your disk. To use the app without the website, keep `index.html`, `serve.ps1` and `Start Brackets and Tierlisting.bat` in one folder and double-click the `.bat` file. It serves the app at `http://localhost:8642/` using Windows' built-in PowerShell; keep its window open while you use the app.

On Mac or Linux, run `python3 -m http.server 8642` in the folder and open `http://localhost:8642/`.
