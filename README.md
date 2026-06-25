# 🌌 Fortnite Sprite Trading Collection Checklist

A high-fidelity, mobile-responsive web utility built for the Fortnite community to track, manage, and seamlessly share their Sprite Trading collection tiers. Designed to look and feel like an authentic in-game digital item locker, this application allows users to effortlessly track item variants and export pixel-perfect progress updates optimized for social sharing.

Live Site: [benitopak96.github.io](https://benitopak96.github.io)

---

## 🚀 Key Features

*   **Digital Locker Layout:** Sleek dark-mode grid UI inspired by Fortnite's aesthetic, complete with dynamic card themes that seamlessly transition using precise, theme-matched tier colors.
*   **Gold Master Tier Badge:** Reaching Level 5 updates the badge to a striking **GOLD MAX** text indicator, ensuring completion stands out across the tracker.
*   **Rapid Management Gestures:**
    *   *Normal Tap:* Increments individual variant styles by single level steps (1-5).
    *   *Press & Hold (0.4s):* Implements custom gesture detection to immediately fast-forward a specific style straight to Level 5 Max.
    *   *MAX ROW Shortcut:* Utility panel buttons built into each item row header to instantly complete all 4 variant slots with one single interaction.
*   **Seamless Camera Roll Integration:** Uses optimized `.webp` file mapping to sync directly with sequential files cleanly exported from mobile operating systems without tedious manual renaming rules.
*   **Smart Social Engine Export:** Driven by a robust client-side implementation of `html2canvas`, tapping "Export PNG Image" temporarily reconstructs the app architecture into a ultra-compact **3-column portrait layout** before saving. This avoids text element clipping and matches the exact dimensional aspect ratios needed for Instagram Stories, TikTok posts, and Discord.
*   **Persistent Client Storage:** Uses native `localStorage` tracking keys to seamlessly save active inventory configurations and customized Epic usernames without requiring server accounts.

---

## 🗂️ Managed Sprite Inventory

The compilation script handles standard and newly released tiers in an ordered structural sequence:

1.  **Water**
2.  **Earth**
3.  **Fire**
4.  **Duck** *(Includes direct target routing for decoupled historical image variants)*
5.  **Ghost**
6.  **Dream**
7.  **Demon**
8.  **Punk**
9.  **King**
10. **Burnt Peanut** *(Standalone item variant style)*
11. **Zero Point**
12. **Fishy** *(v41.10 New Release)*
13. **Striker** *(v41.10 New Release)*
14. **Aura** *(v41.10 New Release)*
15. **Boss** *(v41.10 New Release)*
16. **Grim Reaper** *(v41.10 New Release)*

---

## 📂 Asset Locker Architecture

File image paths are resolved natively based on their digital asset sequence values. To supplement future content drops, maintain raw screenshots inside the primary media tree:

```text
├── index.html              # Core tracking architecture, custom logic script, and styles
└── Images/                 # Capital-mapped image asset directory
    ├── IMG_0383.webp       # Water Normal Base
    ├── IMG_0384.webp       # Water Gold Variant
    ├── IMG_0385.webp       # Water Gummy Variant
    ├── IMG_0386.webp       # Water Galaxy Variant
    └── ...                 # Sequential asset mapping through all 61 locker items
