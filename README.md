# 🏴‍☠️ Fortnite Treasure Hunters — Chest & Pirate Token Simulator

An interactive, single-file web simulator and probability calculator built for **Fortnite Chapter 7: Treasure Hunters**. Open animated Treasure Hunters Chests, test real Epic Games published drop rates (including **Saturday Treasure Hour** multipliers), simulate hundreds of thousands of chest rolls in seconds, and calculate your squad's exact cumulative odds of unlocking a **Pirate Shop Access Token** or **Solid Gold Weekly Outfit**.

![HTML5](https://img.shields.io/badge/HTML5-Single_File-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-CDN-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/Vanilla_JS-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Zero Dependencies](https://img.shields.io/badge/Build-Zero_Dependencies-10B981?style=for-the-badge)

---

## ✨ Key Features

### 1. Authentic Fortnite Treasure Chest Arena
* **Interactive Chest Opening**: Click the chest (or press `Space`) to trigger an anticipation shake, glowing lid reveal, custom SVG reward cards, particle bursts, and synthesized Web Audio sound effects.
* **Jackpot Celebration Fanfare**: Hitting a **Pirate Shop Access Token**, **Weekly Gold Outfit**, or **Legendary Supercar** triggers a full-screen *"New Treasure Unlocked!"* modal with rotating sunbeams, screen shake, and synthesized brass victory fanfare.
* **Duplicate Protection**: Mirrors official event rules where major unique cosmetic treasures and tokens can only be unlocked once per session (rerolling into standard loot thereafter).

### 2. Official Epic Games Drop Rates & Weekly Captains
Pre-configured with Epic Games' published Treasure Hunters chest odds, plus full support for customizing any `1 in N` denominator on the fly:

| Treasure Reward | Rarity Tier | Normal Match (`1x`) | Saturday Treasure Hour | Repeatable? |
| :--- | :--- | :---: | :---: | :---: |
| **Weekly Solid Gold Outfit** | Mythic Gold | `1 in 1,562,500` | `1 in 208,333` *(7.5x)* | No (Unique) |
| **Pirate Shop Access Token** | Pirate Token | `1 in 137,500` | `1 in 91,667` *(1.5x)* | No (Unique) |
| **Weekly Supercar + Golden Llama Decal** | Legendary | `1 in 7,813` | `1 in 781` *(10x)* | No (Unique) |
| **Weekly Back Bling / Pickaxe** | Epic | `1 in 568` | `1 in 568` | No (Unique) |
| **Weekly Festival Jam Track** | Rare | `1 in 391` | `1 in 391` | No (Unique) |
| **Treasure Hunters Loading Screen** | Rare | `1 in 272` | `1 in 272` | No (Unique) |
| **Treasure Extraction Gizmos** | Uncommon | `1 in 127` | `1 in 127` | Yes (In-Match) |

* **Weekly Captain Presets**: Switch between all 5 Weekly Captains (**Week 3: Hatsune Miku**, **Week 1: A$AP Rocky**, **Week 2: Lil' Uzi Vert**, **Week 4: Oscar**, and **Week 5: Buccaneer Brigand Jones**) to dynamically update reward names and collection items.

### 3. Squad & Match Grind Probability Calculator
Plan your real in-game grind using cumulative binomial probability:

$$P(\text{at least 1 drop}) = 1 - (1 - p)^N$$

* **Party Mode Selector**: Choose **Solo (1)**, **Duos (2)**, **Trios (3)**, or **Squads (4)**—automatically accounting for shared squadmate chest rolls.
* **Custom Grind Inputs**: Adjust **Chests Opened per Player per Match** and **Matches Played/Planned** to view:
  * Total combined team chest rolls ($N$)
  * Cumulative odds for the **Pirate Shop Token**, **Weekly Gold Outfit**, and **Any Cosmetic Treasure**
  * Exact chest targets required for a **50%** and **90%** shot at a Pirate Token
  * **One-Click Grind Simulation**: Automatically runs a batch simulation matching your exact squad chest count.

### 4. High-Speed Auto-Simulation & Live Telemetry
* **Visual & Instant Turbo Modes**: Simulate up to `500,000` chests at once with an optional toggle to automatically pause when a Pirate Token or Gold Outfit drops.
* **Live Telemetry & Collection Gallery**: Tracks total chests opened, tokens found, treasures unlocked (`0 / 7` collection progress), dry streaks, and a live drop history log.

---

## 🚀 Quick Start & Deployment

Because this project is built as a **zero-dependency, single-file HTML application**, no build tools, Node.js, or bundlers are required.

### Run Locally
1. Clone or download this repository.
2. Rename `loot_chest_simulator.html` to `index.html` (if not already renamed).
3. Double-click `index.html` to open it directly in any modern web browser.

### Deploy on GitHub Pages
1. Push `index.html` and `README.md` to your GitHub repository's `main` branch.
2. Navigate to **Settings → Pages** in your repository.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, select `main` and `/ (root)`, then click **Save**.
4. Your live simulator will be published at `https://<your-username>.github.io/<repository-name>/`.

---

## 🛠️ Tech Stack
* **HTML5 & Vanilla JavaScript (ES6+)** — Self-contained state management, binomial probability math, and high-throughput `requestAnimationFrame` batch simulation.
* **Tailwind CSS (via CDN)** — Responsive Fortnite-inspired Item Shop & Lobby UI with diagonal rarity gradients and skewed CTA buttons.
* **Custom Inline SVGs & HTML5 Canvas** — Scalable vector reward illustrations, animated chest rigging, and physics-based confetti/sparkle particle bursts.
* **Web Audio API** — Zero-asset procedural sound synthesizer for chest clicks, rarity chimes, and victory fanfare.

---

## ⚠️ Disclaimer
This is a fan-made probability simulator and statistical tool created for educational and entertainment purposes. It is not affiliated with, endorsed, sponsored, or specifically approved by Epic Games, Inc.
