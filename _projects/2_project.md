---
layout: page
title: "Finance App – Stock Portfolio Tracker"
description: "A modern Python-based desktop application for managing and tracking stock investments with real-time data and user profiles"
img: assets/img/neonapp.png
importance: 1
category: fun
related_publications: false
---

**Finance App** is a desktop application for managing stock portfolios locally. It supports multiple user profiles, live stock data, real-time chart visualization, and a user-friendly GUI built with `customtkinter`. The goal is to empower personal investors with full control over their investment records without relying on cloud services.

> 🔗 GitHub Repository (coming soon): [zyrkio/finance_app](https://github.com/zyrkio/Finance_App)

---

### 💡 Project Overview

This app enables the management of multiple users and their respective investment sessions. Stocks can be searched and added dynamically, including price, purchase date, and number of units. Data is fetched live using `yfinance` and stored persistently in a local SQLite database.

---

### 🛠️ Technical Components

| Component          | Description                                                            |
|--------------------|------------------------------------------------------------------------|
| **Python 3.12**     | Programming language used for all backend/frontend logic              |
| **customtkinter**   | Modern GUI framework for tkinter with dark mode and styling support   |
| **SQLite**          | Local database to manage users, sessions, and portfolio data          |
| **yfinance**        | Real-time stock data (price, charts, volume, etc.)                    |
| **matplotlib**      | Visual chart rendering inside the GUI                                 |
| **Threading**       | Non-blocking background data updates                                  |
| **Scrollbar widget**| Scrollable UI for large dynamic stock lists                           |

---

### 🔍 Features

- **User Management**
  - Dropdown to select and switch user profiles
  - Create and manage multiple users
  - Persistent storage of user sessions and investments

- **Stock Search & Add**
  - Search bar with auto-suggestions (e.g., AAPL, GOOGL, MSFT)
  - Add stocks with quantity, purchase date, and per-session budget
  - Visual list of all added stocks in the current session

- **Live Data**
  - Fetches real-time prices from Yahoo Finance
  - Shows key data: last price, change %, high/low, volume
  - Automatically updates in background

- **Interactive UI**
  - Sidebar with navigation to Home, Stocks, and Profile sections
  - Two dynamic frames in Home screen (budget input and stock session overview)
  - Expandable charts under each stock entry for detailed performance

---

### 🖼️ GUI Preview

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/gui1.png" title="Home Screen with Profile Dropdown" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/gui2.png" title="Add Stocks to Session" class="img-fluid rounded z-depth-1" %}
  </div>

</div>


---

### 🎯 Development Context

This app was developed as a hands-on finance and UI/UX project. It combines real-time APIs, custom-styled GUI, local data storage, and investment logic in a single tool. The system runs fully offline after installation and is ideal for personal use.

---

### 📦 Status

- 🔜 Fully working user and stock management system
- 🔜 Real-time charting and price data
- 🔜 GUI with sidebar and scrollable content
- 🔜 Planned: Time range filter for charts (1M, 3M, YTD)
- 🔜 Planned: CSV/PDF export for sessions and portfolios

---

**Built With:** `Python`, `customtkinter`, `SQLite`, `yfinance`, `matplotlib`, `Pillow`, `tkinter`

**Platform:** Desktop (Ubuntu / Windows)

---

### 🙋‍♂️ Want to contribute or give feedback?

Feel free to reach out via GitHub or [LinkedIn](https://www.linkedin.com/in/dein-profil). Feedback and contributions are always welcome!
