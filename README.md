# Tarkov Arbitrage Scanner

A live market arbitrage tool for Escape from Tarkov. Fetches real-time pricing data and calculates profit opportunities across crafting recipes and barter trades — accounting for flea market fees, trader loyalty levels, and price volatility.

**[Live Demo →](https://lichtspitze.github.io/EFT-arbitrage-calc)**

---

## What it does

- Pulls live item prices and recipe data from the [Tarkov.dev GraphQL API](https://tarkov.dev/api/)
- Calculates net profit for every craft and barter recipe in the game
- Compares flea market vs. trader sell routes and picks the best exit
- Tracks price stability (stable / elevated / spiking / volatile) using recent price history
- Filters and sorts by profit, margin, recipe type, and stability
- Respects your trader loyalty levels so costs are accurate to your account

## Tech

- Vanilla JS, HTML, CSS — no build step, no dependencies
- Tarkov.dev GraphQL API for live pricing and recipe data
- Hosted on GitHub Pages

## Usage

Just open the [live demo](https://lichtspitze.github.io/EFT-arbitrage-calc). Set your trader loyalty levels in the panel at the top, then browse or filter the results. Hit **Recalculate** to refresh prices at any time.

To run locally, clone the repo and open `index.html` in a browser — no server needed.

```bash
git clone https://github.com/lichtspitze/tarkov-arbitrage.git
cd tarkov-arbitrage
open index.html
```
