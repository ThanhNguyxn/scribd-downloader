<div align="center">

# 📚 Scribd Downloader

### 🚀 Download any document from Scribd as PDF — for free!

<br/>

[![GitHub stars](https://img.shields.io/github/stars/ThanhNguyxn/scribd-downloader?style=for-the-badge&logo=github&color=yellow)](https://github.com/ThanhNguyxn/scribd-downloader/stargazers)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Greasy Fork](https://img.shields.io/badge/Greasy%20Fork-Install-670000?style=for-the-badge&logo=greasyfork&logoColor=white)](https://greasyfork.org/en/scripts/557768-scribd-downloader)
[![GitHub Sponsors](https://img.shields.io/badge/Sponsor-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/ThanhNguyxn)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/thanhnguyxn)

<br/>

<img src="https://img.shields.io/badge/Chrome-Supported-success?style=flat-square&logo=googlechrome&logoColor=white"/>
<img src="https://img.shields.io/badge/Firefox-Supported-success?style=flat-square&logo=firefox&logoColor=white"/>
<img src="https://img.shields.io/badge/Edge-Supported-success?style=flat-square&logo=microsoftedge&logoColor=white"/>

---

**✨ Fully automated • 🎯 One-click download • 🧹 Clean PDF output**

</div>

<br/>

---

## 🎯 Two Methods

| Method | Best For | Difficulty |
|:-------|:---------|:-----------|
| 🌐 **Tampermonkey** | Quick & easy browser use | ⭐ Easy |
| 🐍 **Python Script** | Developers, automation | ⭐⭐ Medium |

---

<br/>

## 🌐 Method 1: Tampermonkey (Recommended)

### Step 1: Install Tampermonkey Extension

| Browser | Install Link |
|:-------:|:------------:|
| <img src="https://img.shields.io/badge/Chrome-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white"/> | [Install](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) |
| <img src="https://img.shields.io/badge/Firefox-FF7139?style=for-the-badge&logo=firefox&logoColor=white"/> | [Install](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/) |
| <img src="https://img.shields.io/badge/Edge-0078D7?style=for-the-badge&logo=microsoftedge&logoColor=white"/> | [Install](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd) |

### Step 2: Install the Script

[![Install Script](https://img.shields.io/badge/Install%20Script-Greasy%20Fork-670000?style=for-the-badge&logo=greasyfork&logoColor=white)](https://greasyfork.org/en/scripts/557768-scribd-downloader)

Or manually: [**`userscript.js`**](https://raw.githubusercontent.com/ThanhNguyxn/scribd-downloader/main/userscript.js)

### Step 3: Use It!

1. 🌐 Go to any **Scribd document** page
2. 📥 Click the purple **"Download PDF"** button (top-right corner)
3. 🚀 A new tab will open automatically
4. ⬇️ Click the green **"Download PDF"** button on that page
5. ⏳ Wait for all pages to load
6. 🖨️ In print dialog → **Save as PDF**

> 💡 **Tip:** If it redirects to login, click **"Manual (Incognito)"** and follow the instructions!

<br/>

---

## 🐍 Method 2: Python Script

> For developers who prefer command line or need automation

### Requirements

- ![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat-square&logo=python&logoColor=white) [Download Python](https://www.python.org/downloads/)
- ![Chrome](https://img.shields.io/badge/Chrome-Browser-4285F4?style=flat-square&logo=googlechrome&logoColor=white) [Download Chrome](https://www.google.com/chrome/)

### Installation

```bash
# Clone the repository
git clone https://github.com/ThanhNguyxn/scribd-downloader.git
cd scribd-downloader

# Install dependencies
pip install -r requirements.txt

# Run the script
python scribd-downloader.py
```

### Usage

```
Input link Scribd: https://www.scribd.com/document/123456789/Document-Name
```

The script will automatically:
1. 🔗 Convert URL to embed format
2. 🌐 Open Chrome browser
3. 📜 Scroll through all pages
4. 🧹 Remove toolbars & overlays
5. 🖨️ Open print dialog → Save as PDF

<br/>

---

## 🖨️ Print Settings (Important!)

> For best PDF quality, use these settings:

| Setting | Value |
|:--------|:------|
| **Destination** | `Save as PDF` |
| **Margins** | `None` |
| **Background graphics** | `✅ Enabled` |

<br/>

---

## 📂 Project Files

```
📦 scribd-downloader
 ┣ 📜 userscript.js          ← Tampermonkey script
 ┣ 🐍 scribd-downloader.py   ← Python script
 ┗ 📋 requirements.txt       ← Python dependencies
```

<br/>

---

## ⚠️ Disclaimer

> [!CAUTION]
> **Legal Notice:** This tool is provided for **personal and educational purposes only**.

- 📚 **Educational Use:** Intended for students, researchers, and educators who need offline access to study materials
- ⚖️ **Copyright:** Please respect intellectual property rights and Scribd's Terms of Service
- 🚫 **No Redistribution:** Do not redistribute downloaded content commercially or publicly
- 👤 **Your Responsibility:** You are solely responsible for how you use this tool

**By using this tool, you agree that:**
1. You will only download content you have legitimate access to
2. You will not use it to infringe on any copyrights
3. The authors are not liable for any misuse of this tool

<br/>

---

<details>
<summary><h2>🔧 How It Works (For Developers)</h2></summary>

> Understanding the technical mechanism behind this tool

### 🎯 Core Concept

Scribd uses an **embed URL format** (`/embeds/{document_id}/content`) that renders the full document content **without requiring authentication**. This tool leverages this behavior to extract and save documents.

> [!IMPORTANT]
> **Tab Behavior:** When you click "Download PDF", a new tab opens with the embed page. The original Scribd page **stays open** in the background — you won't lose your place!

> [!WARNING]
> **Browser Popup Blocker:** If the new tab doesn't open, your browser may be blocking popups. Allow popups for `scribd.com` or use the "Manual (Incognito)" option instead.

> [!NOTE]
> **Why Incognito?** If you're logged into Scribd, the embed page might redirect to login. Using Incognito mode bypasses this since there's no active session.

### 📊 Technical Flow

```
┌─────────────────────────────────────────────────────────────────────────┐
│  STEP 1: URL TRANSFORMATION                                            │
│  ─────────────────────────────                                          │
│                                                                         │
│  Original:  https://www.scribd.com/document/123456/document-title       │
│                              ↓                                          │
│  Embed:     https://www.scribd.com/embeds/123456/content                │
│                                                                         │
│  ✨ The embed URL displays full content without login restrictions      │
└─────────────────────────────────────────────────────────────────────────┘
                                  ↓
┌─────────────────────────────────────────────────────────────────────────┐
│  STEP 2: CONTENT LOADING                                                │
│  ───────────────────────────                                            │
│                                                                         │
│  • Scribd uses lazy-loading (pages load only when scrolled into view)  │
│  • Script automatically scrolls through ALL pages                       │
│  • Each page element with class="page" is scrolled into viewport       │
│  • Small delay (500ms) ensures content fully renders                    │
│                                                                         │
│  📜 Result: All document pages are now loaded in the DOM                │
└─────────────────────────────────────────────────────────────────────────┘
                                  ↓
┌─────────────────────────────────────────────────────────────────────────┐
│  STEP 3: UI CLEANUP                                                     │
│  ──────────────────                                                     │
│                                                                         │
│  Removes unnecessary elements for clean PDF output:                     │
│                                                                         │
│  ❌ .toolbar_top      →  Top navigation bar                            │
│  ❌ .toolbar_bottom   →  Bottom action bar                             │
│  ❌ .document_scroller →  Scroll container (reset for proper layout)   │
│                                                                         │
│  🧹 Result: Clean document ready for printing                           │
└─────────────────────────────────────────────────────────────────────────┘
                                  ↓
┌─────────────────────────────────────────────────────────────────────────┐
│  STEP 4: PDF GENERATION                                                 │
│  ─────────────────────                                                  │
│                                                                         │
│  • Triggers browser's native print dialog (window.print())             │
│  • User selects "Save as PDF" as destination                           │
│  • Browser renders all loaded pages into a single PDF file             │
│                                                                         │
│  📄 Result: Complete document saved as PDF                              │
└─────────────────────────────────────────────────────────────────────────┘
```

### 🔍 Code Breakdown

| Component | Function |
|:----------|:---------|
| `convert_scribd_link()` | Extracts document ID and builds embed URL |
| `scrollIntoView()` | Forces each page to load by scrolling |
| `removeChild()` | Cleans up toolbar elements |
| `window.print()` | Triggers native browser print/save dialog |

### ⚡ Why This Works

1. **Embed endpoint** — Scribd's embed feature is designed for third-party websites to display documents, so it doesn't enforce the same restrictions as the main viewer
2. **Lazy loading bypass** — By scrolling through all pages, we force the browser to fetch and render every page
3. **Native print** — Using the browser's built-in print function ensures high-quality PDF output with proper formatting

</details>

<br/>

---

<div align="center">

### ⭐ Star this repo if it helped you!

<br/>

[![Made with ❤️](https://img.shields.io/badge/Made%20with-❤️-red?style=for-the-badge)](https://github.com/ThanhNguyxn)
[![GitHub](https://img.shields.io/badge/ThanhNguyxn-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThanhNguyxn)
[![GitHub Sponsors](https://img.shields.io/badge/💖%20Sponsor-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/ThanhNguyxn)
[![Buy Me a Coffee](https://img.shields.io/badge/☕%20Buy%20Me%20a%20Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/thanhnguyxn)

</div>
