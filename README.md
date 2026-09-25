# 🌌 Fortnite Sprite Trading Collection Checklist

A high-fidelity, mobile-responsive web utility built for the Fortnite community to track, manage, and seamlessly share their Sprite Trading collection tiers across **Chapter 7 Season 3** and **Season 4: Override**. Designed to look and feel like an authentic in-game digital item locker, this application allows users to effortlessly track item variants, claim Lobby Hack Codes, sync progress to Discord, and export pixel-perfect progress updates optimized for social sharing.

Live Site: [https://sprites.tyrantnetworks.com](https://sprites.tyrantnetworks.com)

---

## 🚀 Key Features

*   **Digital Locker Layout:** Sleek dark-mode grid UI inspired by Fortnite's aesthetic, complete with dynamic card themes that seamlessly transition using precise, theme-matched tier colors.
*   **Dual-Season Tracking:** A dedicated season selector switches the entire locker between **Season 3** (18 items) and **Season 4: Override** (20 items), each with its own independently tracked inventory, so progress on one season never overwrites the other.
*   **Gold Master Tier Badge:** Reaching Level 5 updates the badge to a striking **GOLD MAX** text indicator, ensuring completion stands out across the tracker.
*   **Rapid Management Gestures:**
    *   *Normal Tap:* Increments individual variant styles by single level steps (1-5).
    *   *Press & Hold (0.4s):* Implements custom gesture detection to immediately fast-forward a specific style straight to Level 5 Max.
    *   *MAX ROW Shortcut:* Utility panel buttons built into each item row header to instantly complete all variant slots with one single interaction.
*   **Lobby Hack Codes Tracker:** A dedicated tab (Season 4 only) lists every known Admin Panel code — Sprites, Sprite Dust, Gizmos, and Cosmetics rewards — with a tap-to-claim checklist so nothing gets missed, and a live "still unclaimed" summary at a glance.
*   **Discord Account Sync:** Linking a Discord account (OAuth) syncs the active sheet to a companion backend, so progress carries over between devices and can be viewed directly from Discord via the community's Sprite Tracker bot commands.
*   **Multi-Sheet Management:** Track multiple collections side-by-side under one browser — your own progress, a friend's, or a giveaway tracker — with instant switching, renaming, and deletion, all independent of each other.
*   **Seamless Camera Roll Integration:** Uses optimized `.webp` file mapping to sync directly with sequential files cleanly exported from mobile operating systems without tedious manual renaming rules.
*   **Smart Social Engine Export:** Driven by a robust client-side implementation of `html2canvas`, tapping "Export PNG Image" temporarily reconstructs the app architecture into an ultra-compact **3-column portrait layout** before saving. This avoids text element clipping and matches the exact dimensional aspect ratios needed for Instagram Stories, TikTok posts, and Discord.
*   **Persistent Client Storage:** Uses native `localStorage` tracking keys to seamlessly save active inventory configurations and customized Epic usernames without requiring server accounts — Discord sync is entirely optional, layered on top.

---

## 🗂️ Managed Sprite Inventory

### Chapter 7 Season 3 (18 items)
Standard, gem, and holofoil-era tiers in ordered structural sequence:

1.  **Water** *(Supports Gem & Holofoil variants)*
2.  **Earth** *(Supports Gem variant)*
3.  **Fire** *(Supports Holofoil variant)*
4.  **Duck** *(Includes target routing for decoupled historical image variants; supports Gem variant)*
5.  **Ghost** *(Supports Holofoil variant)*
6.  **Dream**
7.  **Demon** *(Supports Gem variant)*
8.  **Punk**
9.  **King** *(Supports Holofoil variant)*
10. **Burnt Peanut** *(Standalone item variant style)*
11. **Zero Point** *(Supports Gem variant)*
12. **Fishy**
13. **Striker** *(Supports Holofoil variant)*
14. **Aura** *(Supports Gem variant)*
15. **Boss**
16. **Grim Reaper**
17. **Air** *(Supports Holofoil variant)*
18. **Seven** *(Supports Holofoil variant)*

*(Plus standalone single-variant collectibles carried over from the broader Season 3 set: John Wick, Batman, Vini Jr, Ironmouse, Pollo, Lootin' Llama, Peeky Peely.)*

### Chapter 7 Season 4: Override (20 items)
Base / Gold / Cheat Master / Loot Hacker tier structure, with a fifth exclusive variant on most items:

1.  **Jonesy** *(+ Bounty Hunter variant)*
2.  **Adventure** *(+ Bounty Hunter variant)*
3.  **Bush** *(+ Bounty Hunter variant)*
4.  **Sonic** *(+ Bounty Hunter variant)*
5.  **Tails** *(+ Bounty Hunter variant)*
6.  **Shadow** *(+ Bounty Hunter variant)*
7.  **8-Bit** *(+ Bounty Hunter variant)*
8.  **Jackrabbit** *(+ Bounty Hunter variant)*
9.  **Crown** *(+ exclusive Bounty Hacker variant)*
10. **Kill Switch** *(+ Bounty Hunter variant)*
11. **Klombo** *(+ Bounty Hunter variant)*
12. **Mega Man** *(Base variant only)*
13. **Overshield** *(+ Bounty Hunter variant)*
14. **X-Ray** *(+ Bounty Hunter variant)*
15. **Onigiri** *(+ Bounty Hunter variant)*
16. **Storm Scout** *(+ Bounty Hunter variant)*
17. **Blinky** *(+ Bounty Hunter variant)*
18. **Crash Bandicoot** *(+ Bounty Hunter variant)*
19. **Pond** *(+ Bounty Hunter variant)*
20. **Morgana** *(Base / Gold / Cheat Master / Loot Hacker / Bounty Hunter — full 5-variant set)*

### Lobby Hack Codes (39 total)
Tracked across four reward categories — Sprites, Sprite Dust, Gizmos, and Cosmetics — covering every known active Admin Panel code for the season, kept current as Epic adds new ones.

---

## 📂 Asset Locker Architecture

File image paths are resolved natively based on their digital asset sequence values or advanced static mapping arrays. Season 3 and Season 4 assets live in separate directories to keep each season's sequential numbering independent. To supplement future content drops, maintain raw screenshots inside the primary media tree:

```text
├── index.html              # Core tracking architecture, custom logic script, and styles
├── Images/                  # Season 3 image asset directory
│   ├── IMG_0383.webp        # Water Normal Base
│   ├── IMG_0384.webp        # Water Gold Variant
│   ├── IMG_0466.webp        # Water Gem Variant
│   ├── IMG_0472.webp        # Water Holofoil Variant
│   └── ...                  # Full Season 3 structural asset mapping
└── Images2/                 # Season 4: Override image asset directory
    ├── IMG_2613.webp        # Jonesy Base (original 19-sprite batch starts here)
    ├── ...                  # Sequential through IMG_2686.webp (original batch, 74 images)
    ├── IMG_2905.webp        # Bounty Hunter variant batch starts here (17 images)
    ├── ...                  # Sequential through IMG_2921.webp
    ├── IMG_2922.webp        # Morgana Base (5-image batch)
    └── IMG_2926.webp        # Morgana Bounty Hunter (batch ends here)
