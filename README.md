```markdown
## 🎮 CS2 Case Bot for Streamer.bot

[![Ko-fi](https://img.shields.io/badge/Ko--fi-Support%20Me-FF5E5B?style=flat-square&logo=kofi&logoColor=white)](https://ko-fi.com/mk4gtiguy)
[![License](https://img.shields.io/badge/License-MIT%20%2B%20Disclaimer-yellow.svg?style=flat-square)](LICENSE)

A complete CS2 case opening bot for Streamer.bot with inventory, economy, jackpot, and leaderboards. Perfect for CS2 streamers who want to add interactive gambling-style engagement without real money.

---

## ⚠️ Disclaimer

> This bot is a **fan project for entertainment purposes only**. All CS2 skin names, case names, and trademarks are property of **Valve Corporation**. This bot is not affiliated with, endorsed by, or sponsored by Valve. No real money or actual CS2 items are involved — everything is simulated with fake currency and emoji-based items.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| **6 Cases** | Dreams, Recoil, Kilowatt, Revolution, Fracture, Clutch |
| **Realistic Skins** | 120+ skin names from actual CS2 cases |
| **Case Costs** | $0.50 – $3.00 (simulated currency) |
| **Inventory System** | Collect, sell, and trade up items |
| **Daily Rewards** | Claim $5-$25 every 24 hours |
| **Trade-Up System** | Trade 10 Blues for 1 Purple |
| **Jackpot System** | Enter with random item, winner takes all |
| **Leaderboards** | Top money, inventory value, gold pulls, case opens |
| **20+ Commands** | Full chat interaction |

---

## 📋 Commands

| Command | Description |
|---------|-------------|
| `!setcase [name]` | Switch your active case |
| `!case` | Open your selected case |
| `!inv` | View your inventory counts |
| `!sell` | Sell a random item |
| `!balance` | Check your balance |
| `!daily` | Claim daily reward ($5-$25) |
| `!tradeup` | Trade 10 Blues for a Purple |
| `!jackpot` | Enter jackpot with a random item |
| `!jackpotinfo` | See current jackpot status |
| `!jackpotdraw` | Draw jackpot winner (Mods only) |
| `!mystats` | Your personal case stats |
| `!casestats` | Total opens per case |
| `!caseinfo` | List available cases with prices |
| `!odds` | Show drop rates |
| `!inventoryvalue` | Show your inventory value |
| `!topmoney` | Top 5 balances |
| `!topinventory` | Top 5 inventory values |
| `!topgolds` | Top 5 gold pullers |
| `!topopens` | Top 5 most cases opened |
| `!help` | Show all commands |

---

## 💰 Case Costs

| Case | Cost |
|------|------|
| Recoil | $0.50 |
| Dreams | $1.50 |
| Revolution | $1.50 |
| Kilowatt | $2.00 |
| Fracture | $2.00 |
| Clutch | $3.00 |

---

## 🎲 Drop Rates & Values

| Rarity | Emoji | Chance | Sell Value |
|--------|-------|--------|-------------|
| Gold (Knife/Gloves) | 🟡 | 2.6% | $50.00 |
| Red (Covert) | 🔴 | 2.5% | $5.00 |
| Pink (Classified) | 💗 | 2.5% | $1.50 |
| Purple (Restricted) | 🟣 | 5.0% | $0.50 |
| Blue (Mil-Spec) | 🔷 | 87.4% | $0.10 |

---

## 🚀 Quick Setup

### Prerequisites
- [Streamer.bot](https://streamer.bot) v1.0.4 or higher
- Twitch, YouTube, or Trovo account

### Step 1: Import Persisted Globals
1. Open Streamer.bot → **Services** → **Global Variables** → **Persisted Globals**
2. Copy all skin lists from [`persisted-globals.txt`](persisted-globals.txt)
3. Add each as a new persisted global variable

### Step 2: Create Actions
1. Create a new Action for each command in the list above
2. Paste the corresponding C# code from [`V1.3-Complete-Code-Reference.md`](V1.3-Complete-Code-Reference.md)
3. Set the trigger command (e.g., `!case`, `!inv`)

### Step 3: Link Sub-Actions
- For `!case` command: Add Sub-Action → **Run Action** → `CS2_OpenCase`

### Step 4: Set Mod Permissions
- Set `!jackpotdraw` permission to **Mods Only**

### Step 5: Test
- Type `!help` in your chat to see all commands
- Type `!setcase Dreams` then `!case` to open your first case

For detailed setup instructions, see [`setup-guide.md`](setup-guide.md)

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `V1.3-Complete-Code-Reference.md` | All action C# code |
| `persisted-globals.txt` | Skin lists for copy/paste |
| `setup-guide.md` | Step-by-step installation |
| `LICENSE` | MIT License + IP Disclaimer |

---

## 🔧 Commands Cheat Sheet for Viewers


## 📦 CASE COMMANDS
!setcase [Dreams/Recoil/Kilowatt/Revolution/Fracture/Clutch] - Switch cases
!case - Open your selected case
!caseinfo - See all cases and prices
!odds - See drop rates

## 💰 ECONOMY COMMANDS
!balance - Check your balance
!daily - Claim free 25
!inv - View inventory
!sell - Sell a random item
!tradeup - Trade 10 Blues for 1 Purple
!inventoryvalue - Total inventory worth

## 🎰 JACKPOT COMMANDS
!jackpot - Enter with a random item
!jackpotinfo - See current pot

## 📊 STATS & LEADERBOARDS
!mystats - Your personal stats
!casestats - Total case opens
!topmoney - Richest users
!topinventory - Highest inventory value
!topgolds - Most gold pulls
!topopens - Most cases opened

##❓ HELP
!help - Show this list

```

---

## 🤝 Support the Project

If this bot brings entertainment to your stream, consider supporting continued development:

[![Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/mk4gtiguy)

Your support helps keep the project maintained and updated!

---

## 📝 License

This project is licensed under the **MIT License** with an **IP Disclaimer** — see [LICENSE](LICENSE) file for details.

- ✅ Free to use, modify, and share
- ✅ Donations accepted
- ❌ Not for commercial resale
- ❌ Not affiliated with Valve Corporation

---

## 🙏 Credits

- Created by **Mk4gtiguy**
- Skin names from Counter-Strike 2 © Valve Corporation
- Built for [Streamer.bot](https://streamer.bot)

---

## ⚠️ Legal Note

This software is a **fan project** and does not contain any actual gambling or real money transactions. All currency and items are simulated for entertainment purposes only.
```

---
