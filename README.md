# AKROO BM - Modern Budget & Personal Finance Manager 💰📊

A sleek, responsive personal finance and budget manager built with **Vanilla HTML5, CSS3, and JavaScript**. Designed for speed, rich glassmorphic aesthetics, zero external runtime dependencies, and full **Progressive Web App (PWA)** mobile installation.

![AKROO BM Preview](icons/icon-192.png)

---

## ✨ Features

- 💵 **Multi-Currency Support**: Defaults to Indian Rupee (**INR ₹**), with instant conversion to USD ($), EUR (€), GBP (£), JPY (¥), CAD (CA$), and AUD (AU$).
- 📊 **Interactive SVG Visualizations**:
  - **Category Donut Chart**: Hover highlights, percentages, and center totals.
  - **6-Month Cash Flow Trend**: Side-by-side comparison of income and expenses.
- 🎯 **Category Budget Ceilings**: Set monthly targets per category with real-time visual progress bars (Safe <75%, Warning 75-99%, Exceeded ≥100%).
- ⚡ **Quick-Add Presets**: 1-click presets for common Indian daily expenses (Chai & Snacks ₹40, Lunch Thali ₹160, DMart Groceries ₹750, Petrol ₹500, Salary ₹72,000).
- 📱 **Mobile & Android PWA**:
  - Installable directly to your phone's home screen.
  - Runs in standalone fullscreen mode like a native APK.
  - Complete offline functionality via Service Worker caching (`sw.js`).
- 💾 **Data Privacy & Portability**:
  - All data is stored locally in your browser (`localStorage`).
  - Export to **CSV** (spreadsheet format).
  - Full **JSON Backup & Restore** with 1-click import.
- 🌓 **Obsidian Dark & Clean Light Themes**: Toggleable anytime with preserved preference.

---

## 📁 Project Structure

```
akroo-bm/
├── index.html          # Main HTML structure & modals
├── manifest.json       # Web App Manifest for mobile installation
├── sw.js               # Service worker for offline caching
├── .gitignore          # Git ignore rules
├── README.md           # Project documentation
├── css/
│   └── styles.css      # CSS variables, glassmorphism & responsive design
├── js/
│   ├── storage.js      # LocalStorage layer, initial seed data & backups
│   ├── charts.js       # Native zero-dependency SVG charts
│   └── app.js          # App state, filters, search & event handling
└── icons/
    ├── icon-192.png    # PWA Android icon (192x192)
    ├── icon-512.png    # PWA Android splash icon (512x512)
    └── qr-code.png     # QR code for instant mobile Wi-Fi installation
```

---

## 🚀 Live Demo / Local Run

No build step or node installation required!

### Option 1: Direct File
Simply open `index.html` in any web browser.

### Option 2: Local HTTP Server (Python)
```bash
python -m http.server 8080
```
Then visit `http://localhost:8080` in your browser.

---

## 📱 Mobile Installation (Android / iOS)

1. Connect your phone to the same Wi-Fi as your computer.
2. Open **Google Chrome** on your phone.
3. Visit `http://<your-computer-ip>:8080` (or scan the QR code in the app).
4. Tap Chrome menu **(⋮)** -> **"Install app"** or **"Add to Home screen"**.
5. AKROO BM will be added to your mobile home screen with full offline access!

---

## 🌐 Free Deployment to GitHub Pages

1. In your GitHub repository, go to **Settings** -> **Pages**.
2. Under **Build and deployment**, select:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` / `root`
3. Click **Save**. Within 1 minute, your app will be live at `https://<your-username>.github.io/<repo-name>/`!

---

## 📄 License
MIT License. Free for personal and commercial use.
