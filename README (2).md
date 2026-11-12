# 🌌 Fortnite Sprite Trading Collection Checklist

A high-fidelity, mobile-first web app for the Fortnite community to track, manage, trade and share their Sprite collection across **Chapter 7 Season 3: Runners**, **Season 4: Override** and **Season 5: Treasure Hunters**. It looks and feels like an in-game item locker and adds Discord sync, a community leaderboard, a trade finder, a live Item Shop and news feed, and pixel-perfect share images.

Live Site: [https://sprites.tyrantnetworks.com](https://sprites.tyrantnetworks.com)

---

## 🚀 Key Features

### Checklist
*   **Digital Locker Layout:** Dark, Fortnite-inspired card grid with tier-matched colours per style (Gold, Fortune, Cursed, Cheat Master, Loot Hacker and more).
*   **Three-Season Tracking:** A season selector switches the whole locker between **Season 3: Runners**, **Season 4: Override** and **Season 5: Treasure Hunters**. Each season keeps its own inventory, so progress on one never touches another.
*   **Fast Tapping:**
    *   *Tap:* raises a style one level (1-5).
    *   *Press & hold (0.4s):* jumps straight to Level 5 (GOLD MAX).
    *   *MAX ROW:* maxes every style on a sprite in one tap.
    *   *Undo:* a mis-tap button reverts the last change.
*   **Tile-Level Filters:** *All*, *Need* (level 0), *In progress* (levels 1-4) and *Maxed* (level 5). Filters work per style, so Need only shows the styles you are missing. They combine with search and a style dropdown. Tiles stay put while you tap so rows never jump.
*   **Fortnite's Order:** Seasons 4 and 5 can be sorted in the in-game sprite order (default) or the original *Organize* order, so tracking matches what you see in the game.
*   **Progress Dashboard:** Overall and per-season completion bars plus a "still leveling" summary.
*   **Multi-Sheet Management:** Track several collections (your own, a friend's, a giveaway) with instant switching, renaming and deletion.
*   **Lobby Hack Codes Tracker (Season 4):** Every known Admin Panel code (57) grouped by reward type with tap-to-claim and a live "still unclaimed" count.
*   **Themes & Display:** Dark, Light or Auto theme, comfortable/compact density, and an option to hide MAX ROW buttons.
*   **Install as an App:** Can be added to a phone home screen and loads fast.

### Community
*   **Discord Sync:** Sign in with Discord to save your sheets to the companion backend and keep progress across devices. Sessions use signed tokens, so nobody can read or change someone else's checklist, and the previous save is backed up automatically.
*   **Opt-In Privacy:** Public profile, leaderboard and trade-finder visibility are all off until you switch them on.
*   **Leaderboard:** Ranks opted-in players by completion for each season (Season 5 by default).
*   **Public Profiles:** A shareable page with a player's Season 5 collection and season stats.
*   **Trade Finder (Season 5):** Matches you with other opted-in players on what each of you still needs, and posts trade requests to the Discord Trade Board.
*   **Discord Bot Integration:** The Sprite Tracker bot shows a member's sheet in Discord with a season picker, runs Trade Match between two members and posts to the Trade Board.

### Live Content
*   **Item Shop:** Today's Fortnite Item Shop pulled live from the Fortnite API.
*   **News:** The latest Battle Royale news feed with optional push alerts when new items appear.
*   **Share Images:** "Export PNG Image" rebuilds the page into a compact 3-column portrait layout using `html2canvas`, sized for Instagram Stories, TikTok and Discord.
*   **Local-First Storage:** Progress is saved on your device first; Discord sync is optional.

---

## 🗂️ Managed Sprite Inventory

### Chapter 7 Season 3: Runners (25 items)
Standard, Gem and Holofoil era tiers:

1.  **Water** *(Gem & Holofoil)*
2.  **Earth** *(Gem)*
3.  **Fire** *(Holofoil)*
4.  **Duck** *(Gem; separate historical image routing)*
5.  **Ghost** *(Holofoil)*
6.  **Dream**
7.  **Demon** *(Gem)*
8.  **Punk**
9.  **King** *(Holofoil)*
10. **Burnt Peanut**
11. **Zero Point** *(Gem)*
12. **Fishy**
13. **Striker** *(Holofoil)*
14. **Aura** *(Gem)*
15. **Boss**
16. **Grim Reaper**
17. **Air** *(Holofoil)*
18. **Seven** *(Holofoil)*

Plus single-style collectibles: John Wick, Batman, Vini Jr, Ironmouse, Pollo, Lootin' Llama and Peeky Peely.

### Chapter 7 Season 4: Override (27 items)
Base / Gold / Cheat Master / Loot Hacker structure, with a Bounty Hunter variant on most sprites:

Jonesy, Adventure, Bush, Sonic, Tails, Shadow, 8-Bit, Jackrabbit, Crown *(Bounty Hacker)*, Kill Switch, Klombo, Mega Man *(base only)*, Overshield, X-Ray, Onigiri, Storm Scout, Blinky, Crash Bandicoot, Pond, Morgana, Birthday, plus the Fortnitemares batch: Spooky Dash, Vampire, The Deer, Dumpster Dive, Honey and One Wish Willow *(these add a Trick or Treat variant)*.

### Chapter 7 Season 5: Treasure Hunters (17 items)
Normal / **Fortune** / **Cursed** / **Gold** styles. Listed in the in-game (Fortnite) order, with in-game slot numbers shown where known:

| Sprite | Styles |
|---|---|
| Halfpeel'd (#1) | Normal, Fortune, Cursed, Gold |
| Re-Pete (#5) | Normal, Fortune, Cursed, Gold |
| Barry O'Fish (#9) | Normal, Fortune, Cursed, Gold |
| Wayfinder (#13) | Normal, Fortune, Cursed, Gold |
| Chester (#17) | Normal, Fortune, Cursed, Gold |
| Kelper (#21) | Normal, Fortune, Cursed, Gold |
| Exmarks (#25) | Normal, Fortune, Cursed, Gold |
| Lil' Squibbly (#29) | Normal, Fortune, Cursed, Gold |
| Squiplash (#33) | Normal, Fortune, Cursed, Gold |
| Lil' Flacko (#37) | Normal, Fortune, Cursed, Gold |
| Lil' Uzi Vert Jr. (#41) | Normal, Fortune, Cursed, Gold |
| Sir Oscar The Second (#45) | Normal, Fortune, Cursed, Gold |
| Plundarrgh (#49) | Normal, Fortune, Cursed, Gold |
| Mini Miku (#53) | Normal, Fortune, Cursed, Gold |
| Transponder Snail (#57) | Normal only |
| Sweet Dreams | Normal only *(in-game slot not announced yet)* |
| Zee Sprite | Normal only *(in-game slot not announced yet)* |

**Gold styles** are scheduled for **November 22, 2026 (4:00 AM ET)** and unlock on the site automatically at that time. 

---

## 📂 Asset Locker Architecture

Each season keeps its images in its own folder. Seasons 3 and 4 use sequential camera-roll names; Season 5 uses Epic's own icon filenames.

```text
├── index.html              # The app
├── Images/                 # Season 3 (IMG_0383.webp ...)
├── Images2/                # Season 4: Override (IMG_2613.webp ... IMG_2945.webp)
└── Images3/                # Season 5: Treasure Hunters
    ├── T_Icon_BR_Creature_Sprite_PeelyBones_L.webp                  # Halfpeel'd (Normal)
    ├── T_Icon_BR_Creature_Sprite_PeelyBones_Jeweled_L.webp          # Fortune
    ├── T_Icon_BR_Creature_Sprite_PeelyBones_Cursed_L.webp           # Cursed
    ├── T_Icon_BR_Creature_Sprite_PeelyBones_LiquidGold_L.webp       # Gold
    └── ...                                                          # One set per sprite
```

Season 5 naming: `T_Icon_BR_Creature_Sprite_<Name>[_Jeweled|_Cursed|_LiquidGold]_L.webp`. 

---
