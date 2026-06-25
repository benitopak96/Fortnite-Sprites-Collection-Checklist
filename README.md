# 🌌 Fortnite Sprite Trading Collection Checklist

A modern, mobile-responsive web utility built for the Fortnite community to track, manage, and share their Sprite Trading collection levels. This web application acts as a digital locker grid, enabling players to log their variant styles from Level 1 to Max Level 5 and instantly export their progress in a social-media-friendly layout.

Live Site: [benitopak96.github.io](https://benitopak96.github.io)

---

## 🚀 Key Features

*   **Locker Grid Architecture:** Beautiful dark-mode UI inspired by Fortnite's interface, using customized item cards for each distinct sprite.
*   **Sequential Variant Mapping:** Tailored to read `.webp` formats natively exported by mobile devices (`IMG_XXXX.webp`), sorting variants chronologically without requiring manual file renames.
*   **Persistent Tracking:** Leverages local browser storage (`localStorage`) to automatically remember your username and exact progress tiers—no registration required.
*   **One-Click Social Media Export:** Powered by `html2canvas`, users can click a single button to dynamically rearrange the sprawling list into a sleek, high-resolution **2-column portrait grid** built perfectly for Instagram Stories, TikTok, or Discord sharing.

---

## 🗂️ Sprite Inventory Sequence

The checklist precisely tracks all base sprites and late-breaking updates in their proper game layout sequence:

1.  **Water**
2.  **Earth**
3.  **Fire**
4.  **Duck**
5.  **Ghost**
6.  **Dream**
7.  **Demon**
8.  **Punk**
9.  **King**
10. **Burnt Peanut** *(Standalone item variant)*
11. **Zero Point**
12. **Fishy** *(v41.10 New Release)*
13. **Striker** *(v41.10 New Release)*
14. **Aura** *(v41.10 New Release)*
15. **Boss** *(v41.10 New Release)*
16. **Grim Reaper** *(v41.10 New Release)*

---

## 📂 Asset Folder Architecture

The image compilation script matches folder graphics based on their raw chronological capture structure. To manage or append newly discovered item styles, drop screenshots cleanly into the root media directory:

```text
├── index.html              # Main application architecture, tracking engine, and styles
└── Images/                 # Targeted asset locker directory
    ├── IMG_0383.webp       # Water Normal
    ├── IMG_0384.webp       # Water Gold
    ├── IMG_0385.webp       # Water Gummy
    ├── IMG_0386.webp       # Water Galaxy
    ├── IMG_0387.webp       # Earth Normal
    └── ...                 # Incremental numerical mapping through all 61 styles
