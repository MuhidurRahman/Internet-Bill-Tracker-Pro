# 🌐 Personal Internet Bill Tracker

> A fully offline, self-hosted, single-page web app to track your internet bill payments, plans, and payment history. Built with HTML, CSS, JavaScript, TailwindCSS, Font Awesome, Dexie.js (IndexedDB), and optional animation libraries like AnimeJS for a smooth, modern interface.

---

## ✨ Features

- **Smart Bill Reminder** – Countdown for the next due date with alerts.  
- **Automatic Next Due Date Calculation** – Calculates your next expected payment.  
- **Monthly Summary** – Shows latest payment details: date, amount, plan, method, and cashier.  
- **Animated Charts** – Yearly and monthly spending visualizations.  
- **Payment Streak Tracker** – Track consecutive months of on-time payments.  
- **Offline-First Functionality** – Fully client-side using Dexie.js + IndexedDB.  
- **Quick-Add Button** – Floating button to instantly add new payments.  
- **Plan History Log** – Track plan changes and upgrades/downgrades.  
- **Export & Import JSON Backup** – Save or restore payment history.  
- **Animated Notifications** – Smooth alerts for adding, editing, or deleting payments.  
- **Dashboard Widgets** – Overview of total payments, averages, highest/lowest payments.  
- **Search & Filter System** – Quickly search by month, cashier, plan, or payment method.  
- **Editable ISP Profile** – Update ISP name, connection date, and more.  
- **Auto Backup** – Optional automatic local backup whenever a new payment is added.  
- **Theme System** – Dark mode + customizable accent color for a professional feel.  
- **Responsive & Modern UI** – Clean design using TailwindCSS, Font Awesome, and optional AnimeJS animations.

---

## 💾 Data Storage

The app uses **Dexie.js (IndexedDB)** for offline storage. All records are persistent in your browser.

### Example Backup JSON (Safe Dummy Data)

```json
{
  "settings": {
    "id": 1,
    "isp": "Demo ISP",
    "startDate": "2025-01-01",
    "monthlyAmount": "500"
  },
  "payments": [
    {
      "date": "2025-12-06",
      "amount": "500",
      "method": "Online",
      "note": "Cashier 1",
      "isp": "Demo ISP",
      "id": 11
    },
    {
      "date": "2025-11-06",
      "amount": "500",
      "method": "Cash",
      "note": "Cashier 2",
      "isp": "Demo ISP",
      "id": 12
    },
    {
      "date": "2025-10-06",
      "amount": "600",
      "method": "Online",
      "note": "Cashier 1",
      "isp": "Demo ISP",
      "id": 13
    }
  ],
  "userPrefs": {
    "id": 1,
    "theme": "dark",
    "accentColor": "236, 72, 153",
    "accentSecondary": "219, 39, 119"
  },
  "exportDate": "2025-12-07T08:22:05.719Z"
}
