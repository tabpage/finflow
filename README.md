# Finova

A sleek, client-side personal finance tracker that runs entirely in your browser.  
Track income, expenses, capital, withdrawals, debts, and repayments — all with a clean UI and powerful filtering, right-click editing, PDF reports, and local data protection.

🌐 **Live demo:** [tabpage.github.io/finova](http://tabpage.github.io/finova/)


---

## ✨ Features

- **Add & categorise transactions**  
  Description, category, amount, date, time, and transaction type (Capital, Withdrawal, Income, Expense, Debt, Repayment).

- **Real‑time dashboard**  
  See totals for each category, net balance, and a horizontal bar chart.

- **Powerful history filtering**  
  Search by description, category, date, or type — in any combination. The balance label updates dynamically to reflect your active filters.

- **Easy editing**  
  Right‑click (desktop) or long‑press (mobile/tablet) any entry to edit its description, category, or amount.  
  Delete entries instantly with the × button.

- **Dark / light theme**  
  Toggle between modes with a single click. Your preference is saved locally.

- **Local security lock**  
  Set a password to protect your financial data. After locking, you must enter the password to regain access.  
  *Data is never sent anywhere — everything lives in your browser.*

- **Export & import**  
  - **JSON backup** – export all transactions to a .json file and import it later.  
  - **PDF report** – generate a professional report with summary totals and the filtered transaction list. The PDF respects your active filters.

- **Fully responsive**  
  Designed to work on desktops, tablets, and phones.

- **Zero dependencies on a server**  
  Works offline once loaded. All assets are delivered via CDN.

---

## 🛠️ Technology Stack

| Component         | Technology                                 |
| ----------------- | ------------------------------------------ |
| Frontend          | Vanilla HTML, CSS, JavaScript              |
| Styling           | [Tailwind CSS](https://tailwindcss.com/) (CDN) |
| Charts            | [Chart.js](https://www.chartjs.org/) (CDN) |
| PDF generation    | [jsPDF](https://github.com/parallax/jsPDF) + [AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) (CDN) |
| Data persistence  | `localStorage` & `sessionStorage`          |

---

## 🚀 Getting Started

1. **Download or clone** the repository.
2. Open `index.html` in any modern web browser.
3. That’s it! No build tools, no server, no installation.

> **Note:** If you open the file directly (`file://` protocol) some browser security features (like certain import/export behaviours) may be slightly restricted. For the best experience, serve the file using a simple HTTP server (e.g., `python -m http.server 8000` or the **Live Server** extension in VS Code).

---

## 📖 Usage

### Adding a Transaction
1. Fill in **Description**, **Category** (e.g., “Groceries”, “Freelance”), **Amount**.
2. Adjust the date and time if needed (defaults to now).
3. Choose a **Type** from the dropdown.
4. Click **Save Entry**. The new transaction appears in the history list and stats update instantly.

### Filtering & Searching
- **Search description** – type in the “Search description…” field.
- **Filter by category** – use the “Filter category…” input.
- **Filter by date** – pick a date; only transactions from that day will be shown.
- **Filter by type** – select a specific type (e.g., only expenses).
- All filters combine. The balance label will reflect the active filters.  
- Click **Show All** to clear all filters.

### Editing an Entry
- **Desktop:** right‑click an item in the history.
- **Mobile/tablet:** long‑press (hold for ~600ms) the item.
- A modal will open where you can change the description, category, or amount. Click **Save Changes**.

### Exporting Data
- **JSON Backup** – click the profile menu (top left, “Local Storage Mode”), then **Export Backup (.json)**.
- **PDF Report** – click the **Export PDF** button in the same menu. The report respects your current filters.

### Importing Data
- Click **Import Backup (.json)** in the profile menu and select a previously exported .json file.

### Security
- **Set a password** – click the profile menu → **Setup Password**.
- **Lock the app** – click **Lock Now** or simply refresh the page (the lock screen will appear).
- To unlock, enter the password you set.  
  *If you forget the password, you can use the **Reset App** button on the lock screen to erase all data and start fresh.*

---

## 🗄️ Data Storage & Privacy

All transactions and settings are stored in your browser’s `localStorage` under the keys `bp_transactions`, `bp_pin`, and `bp_theme`.  
The unlock status is held in `sessionStorage` and cleared when the browser tab is closed.

No data is ever sent to any server. This makes Fin Flow **100% private** — but also means that if you clear your browser storage or use a different device, your data will be gone unless you’ve exported a backup.

---

## ⚙️ Customisation

You can easily tweak the app:

- **Colours & theme** – edit the Tailwind classes directly in the HTML.  
- **Chart appearance** – modify the `initChart()` function in the `<script>` tag.  
- **PDF report design** – adjust the `exportPdfBtn.onclick` handler.

Everything is self‑contained, so changes take effect immediately.

---

## 📄 License

This project is provided as open‑source. Feel free to use, modify, and distribute it.  
*(Consider adding a formal license like MIT if you wish.)*

---

## 🙏 Acknowledgements

- [Tailwind CSS](https://tailwindcss.com/)
- [Chart.js](https://www.chartjs.org/)
- [jsPDF](https://github.com/parallax/jsPDF)
- [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable)
- Font: [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) from Google Fonts

---

**Enjoy tracking your finances with Fin Flow!** 🚀
