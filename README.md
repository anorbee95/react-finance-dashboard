# 💰 React Finance Dashboard

A modern, mobile-first personal finance dashboard built with **React**, **Vite**, and **Firebase**. Track your income, expenses, savings goals, and view insightful monthly breakdowns — all stored securely in the cloud.

> Built and maintained by **Norbert Augusztin** ([anorbee95](https://github.com/anorbee95))

---

## 🚀 Features

- 📥 Add and manage income, expenses, savings, and debts
- 📊 Real-time totals, net balance, and visual summaries
- 📈 Interactive charts with Chart.js
- 📅 Monthly breakdown with filters
- 🎯 Savings goal tracking with % progress
- 🔔 Push notification when a goal is achieved
- 📤 Export transactions to CSV
- 🔒 (Optional) Firebase Authentication
- ☁️ Firebase Firestore for real-time data sync
- 📱 Fully responsive & optimized for mobile

---

## 🛠️ Tech Stack

- [React](https://react.dev/)
- [Vite](https://vitejs.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Firebase](https://firebase.google.com/) (Firestore, optional Auth)
- [Chart.js](https://www.chartjs.org/) + [`react-chartjs-2`](https://react-chartjs-2.js.org/)

---

## 📁 Project Structure

```
src/
├── components/
│   ├── TransactionForm.jsx
│   ├── TransactionList.jsx
│   ├── Summary.jsx
│   ├── Goals.jsx
│   ├── MonthSelector.jsx
│   ├── ChartSection.jsx
│   └── ExportCSV.jsx
├── firebase.js
├── App.jsx
└── main.jsx
```

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/anorbee95/react-finance-dashboard.git
cd react-finance-dashboard
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up Firebase

- Go to [Firebase Console](https://console.firebase.google.com/)
- Create a project → Enable **Firestore Database**
- Get your Firebase config and paste into `firebase.js`

```js
// firebase.js
import { initializeApp } from "firebase/app";
import { getFirestore } from "firebase/firestore";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID",
};

const app = initializeApp(firebaseConfig);
export const db = getFirestore(app);
```

### 4. Run the development server

```bash
npm run dev
```

---

## 🎨 Tailwind Setup

Tailwind is preconfigured using the default Vite setup:

- `tailwind.config.js` for theming
- `index.css` includes Tailwind base/styles/utilities

---

## 📤 Deployment (Optional)

You can deploy this app to Firebase Hosting or Vercel:

### Firebase Hosting:

```bash
npm run build
firebase init hosting
firebase deploy
```

### Or deploy to [vercel.com](https://vercel.com/) with one click.

---

## 🌱 Ideas for Future Development

- Budget limits & warnings
- Multi-currency support
- Dark mode toggle
- Recurring expenses
- Sync with Google Sheets

---

## 📄 License

MIT License — Free to use, adapt, or expand. Attribution is appreciated.

---

Made with ❤️ by **Norbert Augusztin**  
[GitHub](https://github.com/anorbee95)
