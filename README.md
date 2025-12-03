<div align="center">

# 📚 Scribd Downloader

### 🚀 Download any document from Scribd as PDF — for free!

<br/>

[![GitHub stars](https://img.shields.io/github/stars/ThanhNguyxn/scribd-downloader?style=for-the-badge&logo=github&color=yellow)](https://github.com/ThanhNguyxn/scribd-downloader/stargazers)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Greasy Fork](https://img.shields.io/badge/Greasy%20Fork-Install-670000?style=for-the-badge&logo=greasyfork&logoColor=white)](https://greasyfork.org/en/scripts/557768-scribd-downloader)
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

> This tool is for **personal & educational use only**.  
> Please respect copyright and Scribd's terms of service.

<br/>

---

<div align="center">

### ⭐ Star this repo if it helped you!

<br/>

[![Made with ❤️](https://img.shields.io/badge/Made%20with-❤️-red?style=for-the-badge)](https://github.com/ThanhNguyxn)
[![GitHub](https://img.shields.io/badge/ThanhNguyxn-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThanhNguyxn)
[![Buy Me a Coffee](https://img.shields.io/badge/☕%20Buy%20Me%20a%20Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/thanhnguyxn)

</div>
