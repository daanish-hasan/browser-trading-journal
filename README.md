# Browser-Based Trading Journal

A private, single-file trading journal that runs entirely in your web browser. No sign-up, no server, no tracking — your data never leaves your computer.

Inspired by the look of tools like TradeZella, but free, open source, and local-first.

## Live demo

**[Try it here](https://daanish-hasan.github.io/browser-trading-journal/)**

## Features

- **Dashboard** — net P&L, win rate, profit factor, avg win/loss, open trades; a monthly P&L calendar with per-day dollar and percentage returns; and performance charts with a date-range filter.
- **Log trades** — stocks or options (Call/Put, strike, expiration, x100 contract math), entry/exit, position size, stop/target, a live risk meter, emotion tags, pre/post-trade notes, and pasteable chart screenshots.
- **Auto-updating balance** — set a starting balance once; your current balance updates itself after every closed trade.
- **Trade history** — grouped by day with a running balance and end-of-day totals, search + date filter, and quick edit/delete. Built to reconcile against your broker.
- **Notes** — a Markdown document library with folders and subfolders, Write/Preview, and autosave.
- **Backup** — one-click Export / Import so you never lose your data.

## How your data is stored (and why it is private)

Everything lives in your browser's **localStorage**, on your own machine. There is no backend, no account, and nothing is uploaded anywhere. Because the data is tied to your browser:

- It persists across sessions on the same browser and computer.
- It does **not** sync to other devices or browsers.
- Clearing your browser's site data will erase it — so use **Export backup** to save a file, and **Import backup** to restore it.

The only external request the app makes is loading the Chart.js charting library from a CDN the first time you open it, so the very first load needs an internet connection. Everything else works offline.

## Use it

**Online (easiest):** open the live demo link above. It runs right in your browser and your data saves locally — you can bookmark it, no download needed.

## Download your own copy (no git or terminal required)

- **The whole project:** click the green **`< > Code`** button near the top of this page, then **Download ZIP**. Unzip it and double-click **`index.html`**.
- **Just the app file:** open **`index.html`** in the file list above, then click the **Download raw file** icon on that file's toolbar. Double-click the saved file to open it.

Either way it works exactly the same — one self-contained file, with your data stored privately in your own browser.

> Sharing tip: send people the live-demo **link**, not the `.html` file. Some chat apps (Discord, etc.) flag HTML attachments as unsafe, even though this one isn't.

## Is it safe? (open source, on purpose)

It is a single HTML file with the CSS and JavaScript inline — you can read every line. No obfuscation, no network calls except the chart library, no data collection. Fork it, audit it, change it.

## Tech

- Plain HTML + CSS + vanilla JavaScript, in one file.
- [Chart.js](https://www.chartjs.org/) for charts (loaded from a CDN).
- Data persistence via the browser `localStorage` API.

## Set up your shareable link (GitHub Pages)

1. Push this repo to GitHub (steps below).
2. In the repo, open **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/ (root)**, then **Save**.
5. Wait about a minute and refresh — GitHub shows your live URL: `https://daanish-hasan.github.io/browser-trading-journal/`
6. Paste that URL into the Live demo link near the top of this README.

## Disclaimer

This is a personal hobby project provided **as-is, with no warranty**. It is a journaling tool, **not financial advice**, and it does not execute trades or connect to any broker. Use at your own risk and keep your own backups.

## License

MIT — see [LICENSE](LICENSE). Free to use, modify, and share.
