# silver-trading

# 🪙 Silver Investment Tracker (Premium Dashboard)

### **Overview**
This is a single-page, real-time financial dashboard designed specifically for **Silver Investors** using the **Trading 212** platform. It categorizes silver assets by risk level, provides live technical analysis, and offers direct "Deep Links" to buy the assets immediately.

The interface features a premium "Silver Bullion" aesthetic with a cinematic video background, glassmorphism cards, and automated trading logic.

---

### **🌟 Key Features**

#### **1. Live "Auto-Strategy" Engine**
Instead of static advice (e.g., "Buy at $20"), the dashboard uses **TradingView's Technical Analysis Widget**.
* **What it does:** It aggregates dozens of real-time indicators (Moving Averages, Oscillators, Pivots).
* **The Output:** A live speedometer gauge showing **Strong Sell**, **Sell**, **Neutral**, **Buy**, or **Strong Buy**.
* **Timeframes:**
    * *Long-term Assets:* 1-Day Interval (Swing Trading focus).
    * *CFD/Day Trading:* 15-Minute Interval (Intraday focus).

#### **2. Smart Market Status & Timer**
The header contains a dynamic status bar driven by custom JavaScript:
* **Auto-Detection:** Automatically calculates if the US Market (NYSE/Nasdaq) is currently **OPEN** or **CLOSED**.
* **Countdown:**
    * If Closed: Shows time remaining until Open (e.g., *"Opens in 04h 12m"*).
    * If Open: Shows time remaining until Close (e.g., *"Closes in 02h 30m"*).
* **Local Time:** Automatically adjusts to the user's local timezone.

#### **3. Risk-Segmented Asset Tracking**
The dashboard tracks 4 distinct asset classes to create a balanced portfolio:
* 🟢 **#1 Safer (SSLN):** *iShares Physical Silver.* Tracks spot price. Low volatility. Wealth preservation.
* 🔵 **#2 Growth (WPM):** *Wheaton Precious Metals.* Streaming company. Safer than miners, higher yield than spot.
* 🟠 **#3 Aggressive (AG):** *First Majestic Silver.* Pure-play miner. High volatility (moves 2x faster than spot).
* 🔴 **Day Trade Only (CFD):** *Spot Silver.* Leveraged derivative. High fee risk (Swap fees).

#### **4. Deep-Link "Bullion Buttons"**
* The "Buy on T212" buttons are custom-styled silver bars.
* **Function:** Clicking a button does not just go to the homepage; it opens the **specific instrument's trading page** inside Trading 212, saving you search time.

---

### **🛠 Technical Details**

* **Tech Stack:** Pure HTML5, CSS3, and Vanilla JavaScript. No framework (React/Angular) required.
* **External Libraries:** `TradingView Lightweight Widgets` (loaded via CDN).
* **Background:** A looped, high-definition MP4 video of rotating silver bullion, hosted via raw GitHub user content for speed.
* **Responsiveness:** CSS Grid layout (`grid-template-columns: repeat(auto-fit...)`) ensures the dashboard scales perfectly from Mobile Phones to 4K Desktop Screens.

---

### **🚀 How to Deploy / Update**

Since this is a static HTML file, you can host it for free on almost any platform.

**Option A: Netlify Drop (Easiest)**
1.  Save your code as `index.html`.
2.  Drag that file into the drop zone at [app.netlify.com/drop](https://app.netlify.com/drop).
3.  Your site is live instantly.

**Option B: GitHub Pages (Best for Version Control)**
1.  Upload `index.html` to a GitHub Repository.
2.  Go to **Settings > Pages**.
3.  Select `main` branch and click Save.
4.  Your site will be live at `yourname.github.io/repo-name`.

---

### **⚠️ Important Disclaimer**
* **Not Financial Advice:** The "Buy/Sell" gauges are generated mathematically by TradingView algorithms and should not be blindly followed.
* **Data Latency:** While charts are "real-time," free data feeds may have slight delays compared to professional paid terminals.
* **Trading 212:** This dashboard is an independent tool and is not affiliated with Trading 212.
