# StockVault 

A modern, full-featured web trading platform for simulated stock trading, portfolio management, and financial learning. StockVault offers a beautiful, responsive UI, robust user/admin flows, and innovative features for both beginners and advanced users.

---

## 🚀 Features

- **User & Admin Authentication**: Secure login, registration, and admin access with session management.
- **Modern Dashboard**: Realistic, visually appealing dashboard with portfolio summary, top performers, and personalized greeting/tips.
- **Trading Glossary**: Built-in glossary modal for trading terms and concepts.
- **Stock Market Simulation**: Browse, search, and trade stocks with real-time price updates.
- **Portfolio Management**: Track holdings, profit/loss, and performance at a glance.
- **Wallet**: Deposit/withdraw funds, view balance, and manage transactions.
- **Transaction History**: Full record of all trades, deposits, and withdrawals.
- **Profile Management**: Update profile info and upload a profile picture.
- **Admin Panel**: Manage users, stocks, and platform data with a dedicated admin dashboard.
- **Responsive Design**: Works beautifully on desktop and mobile.
- **UI/UX Enhancements**: Clean navigation, modern cards, modals, tooltips, and animated login page.

---

## 📸 Screenshots

### Login & Registration
![Login](screenshots/login.png) ![Register](screenshots/register.png)

### Dashboard & Home
![Dashboard](screenshots/dashboard.png) ![Home](screenshots/home.png)

### Trading & Portfolio
![Stocks](screenshots/stocks.png) ![Stock Info](screenshots/stock%20info.png) ![Portfolio](screenshots/portfolio.png)

### Wallet & Transactions
![Wallet](screenshots/wallet.png) ![Transactions](screenshots/transactions.png)

### Profile & Admin
![Profile Settings](screenshots/profile%20settings.png)
![Admin Dashboard](screenshots/admin%20dashboard.png) ![Manage User](screenshots/manage%20user.png) ![Add Stocks](screenshots/add%20stocks.png) ![Manage Stocks](screenshots/manage%20stocks.png)

---

## 🛠️ Technology Stack

- **Frontend**: HTML, CSS (custom + admin.css), JavaScript, EJS templates
- **Backend**: Node.js, Express.js
- **Database**: MySQL (schema in `db/schema.sql`)
- **Authentication**: Session-based, bcrypt password hashing
- **File Uploads**: Multer (for profile pictures)
- **UI Libraries**: FontAwesome, Chart.js

---

## 📁 Project Structure

```
TradePro/
├── app.js                  # Main application file
├── db.js                   # Database connection
├── db/                     # SQL schema and setup scripts
│   ├── schema.sql
│   ├── create_tables.sql
│   └── admin_schema.sql
├── public/                 # Static assets
│   ├── css/                # style.css, admin.css
│   ├── img/                # Branding/media
│   ├── js/                 # main.js
│   └── uploads/profile/    # User profile pictures
├── routes/                 # Express route handlers
│   ├── admin.js
│   ├── auth.js
│   ├── portfolio.js
│   ├── profile.js
│   ├── stocks.js
│   ├── transactions.js
│   └── wallet.js
├── views/                  # EJS templates
│   ├── admin/              # Admin panel views
│   ├── auth/               # Login/register
│   ├── layouts/            # Layouts
│   ├── partials/           # Header/footer
│   ├── portfolio/
│   ├── profile/
│   ├── stocks/
│   ├── transactions/
│   └── wallet/
├── package.json            # Dependencies & scripts
└── README.md
```

---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js (v14+ recommended)
- MySQL (v5.7+)

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd TradePro
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment Variables
Create a `.env` file in the root:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=trading_new
SESSION_SECRET=your_secret_key
PORT=3000
```

### 4. Set Up the Database
- Create a MySQL database named `trading_new`.
- Run the SQL in `db/schema.sql` to create tables and sample data.

### 5. Create Uploads Directory
```bash
mkdir -p public/uploads/profile
```

### 6. Start the Application
```bash
npm start
```
Visit [http://localhost:3000](http://localhost:3000) in your browser.

---

## 👤 User & Admin Flows

- **User:** Register → Login → Dashboard → Trade stocks, manage portfolio, wallet, and profile.
- **Admin:** Use the "Test Admin Login" button on the login page to access the admin dashboard and manage users/stocks.

---

## 💡 Notable UI/UX Features
- Animated login page with user/admin tabs (admin via separate button)
- Personalized dashboard greeting and random trading tips
- Trading glossary modal for beginners
- Clean, modern navigation and footer
- All links and buttons contextually shown/hidden based on user/admin status
- No broken or placeholder links—everything is either functional or clearly described

---

## 📝 License
This project is for educational/demo purposes. Feel free to use, modify, or extend it for your own learning or non-commercial projects. 