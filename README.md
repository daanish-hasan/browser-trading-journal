# Browser-Based Trading Journal

A private, single-file trading journal that runs entirely in your web browser. Works on your phone, tablet, or computer. No sign-up, no server, no tracking.

> **The catch:** your data lives in that browser's local storage, on that one device. It doesn't sync between your phone and your laptop, and clearing your browser data wipes it for good. Back it up with Export if you want to keep it. That's the tradeoff for zero servers and zero accounts, and honestly, it's the only real downside here.

Inspired by the look of tools like TradeZella, but free, open source, and local-first.

## Live demo

**[Try it here](https://daanish-hasan.github.io/browser-trading-journal/)**

## Features

- **Dashboard:** net P&L, win rate, profit factor, avg win/loss, open trades, a monthly P&L calendar with per-day dollar and percentage returns, and four charts with a date-range filter (Today, This week, This month, or custom): cumulative P&L (equity curve), win rate by strategy, P&L by day of week, and emotion vs. average P&L.
- **Log trades:** stocks or options (Call/Put, strike, expiration, x100 contract math), entry/exit, position size, stop/target, auto-calculated risk amount (contracts × fill price × multiplier), a live risk meter, emotion tags, pre/post-trade notes, and pasteable chart screenshots.
- **Auto-updating balance:** set a starting balance once. Your current balance updates itself after every closed trade.
- **Trade history:** grouped by day with a running balance and end-of-day totals, search and date filter, quick edit and delete. Built to reconcile against your broker.
- **Strategies:** a dedicated page for each strategy, with markdown notes, stats (trade count, win rate, net P&L), and every trade linked to it. Rename a strategy and everything tied to it updates automatically.
- **Notes:** a markdown document library with folders and subfolders, Write/Preview, and autosave.
- **Backup:** one-click Export and Import so you never lose your data.
- **Works on your phone too:** on narrow screens the sidebar tucks behind a menu button, so you can log a trade from your phone in portrait, not just on a desktop or in landscape.

## How your data is stored (and why it's private)

Everything lives in your browser's **localStorage**, right on the device you're using. No backend, no account, nothing uploaded anywhere. Because of that:

- It persists across sessions, on that same browser and device.
- It does **not** sync to your other devices or browsers. Log a trade on your phone and it stays on your phone.
- Clearing your browser's site data erases it. Use **Export backup** to save a file, and **Import backup** to bring it back on the same device or a new one.

The only external request the app makes is loading the Chart.js charting library from a CDN, the first time you open it. So the very first load needs an internet connection. After that, everything works offline.

## Use it

**Online (easiest):** open the live demo link above. It runs in your browser and your data saves locally. Bookmark it, no download needed.

## Download your own copy (no git or terminal required)

- **The whole project:** click the green **`< > Code`** button near the top of this page, then **Download ZIP**. Unzip it and double-click **`index.html`**.
- **Just the app file:** open **`index.html`** in the file list above, then click the **Download raw file** icon on that file's toolbar. Double-click the saved file to open it.

Either way it works the same: one self-contained file, with your data stored privately in your own browser.

> Sharing tip: send people the live-demo **link**, not the `.html` file. Some chat apps (Discord, etc.) flag HTML attachments as unsafe, even though this one isn't.

## Is it safe? (open source, on purpose)

It's a single HTML file with the CSS and JavaScript inline, so you can read every line yourself. No obfuscation, no network calls besides the chart library, no data collection. Fork it, audit it, change it.

## Tech

- Plain HTML, CSS, and vanilla JavaScript, in one file.
- [Chart.js](https://www.chartjs.org/) for charts (loaded from a CDN).
- Data persistence via the browser `localStorage` API.

## Disclaimer

This is a personal hobby project, provided as-is with no warranty. It's a journaling tool, not financial advice, and it doesn't execute trades or connect to any broker. Use at your own risk and keep your own backups.

## License

MIT. See [LICENSE](LICENSE). Free to use, modify, and share.

## A note from Daanish

Hey! Thanks for downloading the journal. I really appreciate you giving this a try. I get a lot of fulfillment from trying to help others in this journey we call life.

What I learned in trading is that the market is a mirror of yourself. When you look out into that chart, what you're seeing is yourself. What I mean by that is that your psychology is what will get you across the line. Identifying how you think, what you feel, emotionally charged beliefs, pain you've suffered, how that all ties into your moment-to-moment existence, and how that influences your trading: once you start getting the answers to this deep self-awareness, you will be able to become consistent and trade a system (like a machine). The consistency is where profitability becomes possible. The money is the byproduct of your execution. Your execution ties to your psychology and how well you abide by your rules and your system. And this will be how you track yourself.

Trade well,
**Daanish**
