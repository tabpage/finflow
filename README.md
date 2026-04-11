Fin Flow - Smart Finance Tracker

Fin Flow is a lightweight, high-performance personal finance management tool built for the modern web. It provides a clean, "glassmorphism" inspired interface to help users track capital, income, expenses, withdrawals, and debts with real-time visual analytics.

🔗 Live Demo

Access the application online here: https://tabpage.github.io/finflow/

✨ Key Features

Comprehensive Tracking: Categorize entries into Capital, Withdrawals, Income, Expenses, and Debt.

Visual Analytics: Real-time bar charts powered by Chart.js provide a breakdown of your financial distribution.

Local Security:

PIN Lock: Secure your data with a 4-digit PIN stored in your local session.

Lock Now: Instantly hide your financial data with a blur-based lock screen.

Data Management:

Persistent Storage: Uses localStorage so your data remains even after refreshing the page.

Filter by Date: Quickly drill down into transactions for a specific day.

History Management: Delete individual entries or clear the entire history.

Export Reports: Generate professional PDF reports of your financial summary and transaction history using jsPDF.

Responsive Design: Fully optimized for mobile and desktop viewing using Tailwind CSS.

🛠️ Technical Stack

Frontend: HTML5, Tailwind CSS

Visuals: Chart.js

PDF Generation: jsPDF & jsPDF-AutoTable

Storage: Browser localStorage (No backend required)

Icons & Fonts: Google Fonts (Noto Sans)

🚀 Getting Started

Since Fin Flow is a client-side application, getting started is simple:

Visit the Live Site: Go to tabpage.github.io/finflow/

Alternative (Local): Download the index.html file and open it in any modern web browser.

Start Tracking: Add your first entry using the "New Entry" form on the left/center panel.

📖 Usage Guide

Setting up a PIN

Click on the Local Storage Mode profile button in the top left.

Select Setup PIN.

Enter a 4-digit code. Your app will now require this code whenever the session expires or the app is locked.

Filtering Transactions

Use the date picker in the History section to view entries for a specific day.

Click Show All to return to the full transaction list.

Exporting Data

Open the profile menu (Top Left).

Click Export Report (PDF). This will generate a document containing your net balance summary and a detailed table of all transactions.

Resetting the App

If you forget your PIN or want to wipe all data, click the Reset App (Delete Data) link on the lock screen. Warning: This action is permanent.

📂 File Structure

index.html
├── HTML5 (Structure)
├── Tailwind CSS (Styling)
├── JavaScript (Application Logic)
│   ├── State Management (localStorage)
│   ├── Chart Initialization
│   ├── PDF Logic
│   └── Security/PIN Handlers
└── External CDN Dependencies



📝 License

This project is open-source. Feel free to modify and adapt it for your personal use.
