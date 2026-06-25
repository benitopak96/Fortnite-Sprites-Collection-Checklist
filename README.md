# 🌌 Fortnite Sprite Trading & Level Checklist

An elegant, mobile-friendly checklist web app designed to track your Fortnite Sprite collection, individual variant styles, and custom levels (1–5). Easily see your level completion progress, toggle your inventory, and customize your trading username.

🔗 **Live Link:** [View My Sprite Checklist](https://benitopak96.github.io/Fortnite-Sprites-Collection-Checklist/)

---

## ✨ Features

* **Multi-Tier Level System:** Instead of a simple checkmark, tap any sprite variant tile to cycle beautifully through its development stages:
  `Need It ✕` → `Lvl 1` → `Lvl 2` → `Lvl 3` → `Lvl 4` → `🏆 Max Lvl 5` → back to `Need It ✕`.
* **Custom Epic Username:** Edit your username dynamically at the top of the page, which instantly updates your Call to Action (CTA) at the bottom for quick sharing.
* **Precise Progress Tracking:** Visual gradient progress bar calculates your overall completion percentage based on the total leveling points earned across all styles.
* **Auto-Save Natively:** Powered by `localStorage`—your current levels and custom username persist natively inside your web browser. No log-ins or database connections required.
* **Reset Functionality:** Want to clean the slate or start your tracking fresh? Reset back to max level defaults with a single click.

---

## 🛠️ Built With

* **HTML5** - Structure & semantics
* **CSS3** - Modern custom properties (variables), custom UI theme styling, and responsive layout grids
* **Vanilla JavaScript** - State management cycling arrays, browser data persistence, and dynamic micro-rendering

---

## 🚀 How to Customize or Use Locally

If you want to tweak the code or run it locally:

1. Clone or download this repository.
2. Open the `index.html` file in any modern web browser.
3. If you want to change the default starting inventory levels or change trackable sprites, update the `SPRITES` array or `DEFAULT_STATE` object inside the `<script>` tags.
