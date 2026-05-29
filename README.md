Fin Flow - Smart Finance Tracker

Fin Flow is a lightweight, high-performance personal finance management tool built for the modern web. It features a sophisticated "glassmorphism" interface designed to help users track capital, income, expenses, withdrawals, and debts with real-time visual analytics and robust local security.

🔗 Live Demo

Access the application online here: https://tabpage.github.io/finflow/


✨ Key Features

📊 Real-Time Analytics

Dynamic Bar Chart: Powered by Chart.js, providing an instant visual breakdown of your financial distribution (Capital, Withdraw, Income, Expense, Debt).

Live Summaries: Total Balance, Income, and Expense cards update instantly with every transaction.

🛡️ Enhanced Security

PIN Protection: Secure your financial data with a custom 4-digit PIN.

Privacy Lock: Toggle "Privacy Mode" to blur your sensitive balances or use "Lock Now" to protect the entire application session.

Session Management: The app intelligently handles login states to keep your data private.

🌓 Modern UI/UX

Adaptive Theme: Toggle between Light and Dark modes with a single click.

Mobile First: Fully responsive layout using Tailwind CSS, optimized for both desktop and mobile touch interactions.

Glassmorphism Design: A premium look with blurred backgrounds, smooth transitions, and Noto Sans typography.

📑 Data & Portability

Transaction History: Filterable history by date with the ability to delete individual entries.

PDF Export: Generate professional, structured reports of your financial summary and transaction history using jsPDF and AutoTable.

Local Persistence: Data is stored locally in your browser (localStorage), meaning no account is required and your data never leaves your device.

🛠️ Technical Stack

Framework: Vanilla HTML5 & JavaScript

Styling: Tailwind CSS (Custom Dark Mode & Glassmorphism)

Charts: Chart.js

PDF Generation: jsPDF & jsPDF-AutoTable

Typography: Google Fonts (Noto Sans)

🚀 Getting Started

Since Fin Flow is a client-side application, setup is instant:

Visit the Live Site: tabpage.github.io/finflow/

Local Setup: - Clone this repository or download the index.html.

Open index.html in any modern web browser.

Setup Security: Click the profile icon in the top-left to "Setup PIN" and secure your local storage.

📖 Usage Guide

1. Setting up Security

Open the Sidebar Menu (Top-Left Profile Icon).

Select Setup PIN.

Enter a 4-digit code. You will now be prompted for this code whenever you revisit the site.

2. Managing Transactions

Use the New Entry form to add data.

Categories:

Capital: Your starting or base funds.

Income/Expense: Daily flow of money.

Withdraw/Debt: Tracking specific transfers or liabilities.

3. Exporting Reports

Click Export Report (PDF) in the sidebar.

The app generates a clean PDF document including your current balance overview and a detailed table of all logged transactions.

4. Resetting the App

If you wish to wipe all data or reset your PIN, use the Reset App link on the Lock Screen.

Note: This action is permanent and clears all browser local storage for this app.

📂 File Structure

finflow/
├── index.html          # Core Application (Logic, UI, and Styles)
└── README.md           # Documentation


📝 License

This project is open-source. Feel free to fork, modify, and adapt it for your personal use.
