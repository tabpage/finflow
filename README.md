<!-- PROJECT HEADER -->
<div align="center">
  <br />
  <img src="https://readme-typing-svg.herokuapp.com?font=Noto+Sans&weight=900&size=40&duration=3000&pause=800&color=6366F1&center=true&vCenter=true&width=500&lines=FINOVA;Smart+Finance+Tracker" alt="FINOVA" />
  
  <p>
    <img src="https://img.shields.io/badge/version-2.0.0-blue?style=for-the-badge&logo=v&logoColor=white" alt="version" />
    <img src="https://img.shields.io/badge/license-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="license" />
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=for-the-badge&logo=github" alt="PRs" />
  </p>
  <br />
  <p><strong>💰 Track every penny. Own your data. Look awesome doing it.</strong></p>
  <br />
  <p>
    <a href="#-key-features"><strong>Features</strong></a> ·
    <a href="#-tech-stack"><strong>Tech Stack</strong></a> ·
    <a href="#-quick-start"><strong>Quick Start</strong></a> ·
    <a href="#-data-management"><strong>Data</strong></a> ·
    <a href="#-security--privacy"><strong>Security</strong></a> ·
    <a href="#-license"><strong>License</strong></a>
  </p>
  <br />
</div>

---

## 🌟 Overview

**Finova** is a **completely local, privacy‑first** personal finance dashboard.  
No servers, no accounts, no tracking — your data stays **in your browser**, under **your control**.

Built with a cutting‑edge, clean aesthetic and fluid micro‑interactions, Finova makes tracking capital, income, expenses, debt, and withdrawals a **delightful experience**.

> ⚡ Pure HTML + Vanilla JS + Tailwind CSS. Open `index.html` and you’re done.

---

## ✨ Key Features

<table>
  <tr>
    <td><img src="https://img.icons8.com/fluency/48/000000/money.png" width="40" /></td>
    <td><strong>Multi‑type Tracking</strong><br/>Capital, Withdrawals, Income, Expenses, Debt, and Repayments – each with dedicated metrics and visual feedback.</td>
    <td><img src="https://img.icons8.com/color/48/000000/combo-chart--v1.png" width="40" /></td>
    <td><strong>Interactive Bar Chart</strong><br/>Real‑time horizontal bar chart powered by Chart.js updates instantly with every entry.</td>
  </tr>
  <tr>
    <td><img src="https://img.icons8.com/color/48/000000/dark-mode.png" width="40" /></td>
    <td><strong>Dynamic Dark/Light Theme</strong><br/>Seamless theme toggle with localStorage persistence and animated icon transitions.</td>
    <td><img src="https://img.icons8.com/color/48/000000/lock--v1.png" width="40" /></td>
    <td><strong>Password Lock Screen</strong><br/>Optional PIN‑based lock to secure the app on shared devices.</td>
  </tr>
  <tr>
    <td><img src="https://img.icons8.com/color/48/000000/export-excel.png" width="40" /></td>
    <td><strong>One‑Click Backup/Restore</strong><br/>Export/import entire dataset as JSON, plus dedicated category export/import.</td>
    <td><img src="https://img.icons8.com/fluency/48/000000/pdf-2.png" width="40" /></td>
    <td><strong>Professional PDF Reports</strong><br/>Generate beautifully formatted, filter‑aware financial reports with jsPDF‑autotable.</td>
  </tr>
  <tr>
    <td><img src="https://img.icons8.com/fluency/48/000000/search--v1.png" width="40" /></td>
    <td><strong>Advanced Filtering</strong><br/>Filter transactions by description, category, date, and type simultaneously.</td>
    <td><img src="https://img.icons8.com/color/48/000000/edit-property.png" width="40" /></td>
    <td><strong>Quick Edit</strong><br/>Right‑click or long‑press any entry to edit – complete with a smooth editing modal and visual highlight.</td>
  </tr>
  <tr>
    <td><img src="https://img.icons8.com/fluency/48/000000/tag.png" width="40" /></td>
    <td><strong>Custom Categories</strong><br/>Create, import, and manage categories. Fill category fields directly from the submenu.</td>
    <td><img src="https://img.icons8.com/color/48/000000/delete-forever.png" width="40" /></td>
    <td><strong>Safe Delete & Clear</strong><br/>Confirm before deleting single entries or clearing entire history.</td>
  </tr>
</table>

---

## 🛠 Tech Stack

| Layer               | Technology                                                          |
| ------------------- | ------------------------------------------------------------------- |
| **Frontend**        | HTML5, CSS3, Vanilla JavaScript                                     |
| **Styling**         | [Tailwind CSS](https://tailwindcss.com/) (CDN + custom config)      |
| **Charts**          | [Chart.js](https://www.chartjs.org/) with dark‑mode‑aware styling   |
| **PDF Generation**  | [jsPDF](https://github.com/parallax/jsPDF) + autotable plugin       |
| **Storage**         | Browser `localStorage` (full offline capability)                    |
| **Icons / UX**      | Custom micro‑animations, glassmorphism cards, long‑press support    |
| **Font**            | Noto Sans – modern, readable, multilingual                          |

---

## 🚀 Quick Start

1. **Clone or download** the repository (or just save the `index.html` file).
2. **Open `index.html`** in any modern browser (Chrome, Edge, Firefox, Safari).
3. **That’s it.** No build step, no npm install, no server required.

> 💡 For a better development experience, run a local server (e.g., `npx serve .`) to avoid CORS warnings when loading external CDN resources if you plan to extend it.

---

## 📖 Usage Guide

### Adding an Entry
- Fill in description, category, amount, date, time, and type.
- Press **Save Entry** – the list, totals, and chart update instantly.

### Editing an Entry
- **Desktop:** Right‑click any transaction.
- **Mobile:** Long‑press (hold down) on any transaction.
- A sleek modal opens where you can modify description, category, or amount.

### Filtering History
- Use the filter toolbar to search by description, category, date, or transaction type.
- Combine multiple filters – the header balance label updates to reflect active filters.

### Exporting Data
- **JSON Backup:** Save your complete transaction history as a `.json` file.
- **PDF Report:** Generate a detailed report (respects active filters) with summary and transaction table.

### Managing Categories
- Open the **Categories** submenu from the profile dropdown.
- View all custom categories, add new ones, or import/export category lists.
- Click any category to instantly fill it in the new‑entry form.

### Security Lock
- Set a PIN from the profile dropdown.
- Once set, the app will lock automatically when you close the tab (session‑based unlock).
- Use **Lock Now** to manually lock the screen at any time.

---

## 🗃 Data Management

All financial data is stored **exclusively** in your browser’s `localStorage`.  
No cookies, no tracking, no backend.  

**Storage keys:**
- `bp_transactions` – transaction array
- `bp_custom_categories` – user‑defined categories
- `bp_pin` – optional password (hash‑like, plain text for this demo)
- `bp_theme` – dark/light preference

**Backup strategy:**
- Use **Export Backup (.json)** to save your data.
- Import it later to restore or migrate between devices.

**Category management:**
- Export categories separately to reuse your organisational structure across different datasets.

---

## 🔐 Security & Privacy

- **100% Client‑Side:** No data ever leaves your browser.
- **Offline‑First:** Works without internet after initial load (CDN scripts may be cached).
- **Lock Screen:** Optional PIN protects the interface – ideal for shared/family computers.
- **Reset App:** A dedicated button wipes **all local data** permanently.

> ⚠️ The PIN is stored **as plain text** in `localStorage` for demo purposes. For a production environment, consider hashing or integrating a more robust authentication method.

---

## 🎨 Theming & Customization

Finova’s design uses Tailwind’s `darkMode: 'class'` strategy.  
- Theme toggle persists via `localStorage`.
- Chart colors and PDF reports adapt to the active theme for a consistent visual experience.

**To change the accent color**, override the `--tw-ring-color` or directly modify the Tailwind config inside the `<script>` tag.  
All UI elements use utility classes, making customisation extremely straightforward.

---

## 🧠 Possible Future Enhancements

- [ ] Recurring transactions (daily/weekly/monthly)
- [ ] Multiple wallets / accounts
- [ ] Budget planning with visual progress bars
- [ ] More chart types (pie, line)
- [ ] CSV import/export
- [ ] Progressive Web App (PWA) manifest & service worker for full offline support
- [ ] Data encryption for the lock screen PIN

---

## 🤝 Contributing

Pull requests are welcome!  
If you have suggestions for improvements or discover a bug, feel free to open an issue.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

<div align="center">
  <br />
  <p>Built with ❤️ and a lot of ☕</p>
  <p>
    <sub>© 2026 Finova. All rights reserved.</sub>
  </p>
</div>
