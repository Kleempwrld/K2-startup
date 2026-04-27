# K2 Startup - Task Rewards Platform

A Firebase-based web app where users can earn K-coins by completing tasks, referring friends, and climbing the leaderboard.

## 🚀 Features

✅ **User Authentication** - Email/Password signup & login  
✅ **Task System** - Earn coins from tasks (Watch ads, Litter picking, Daily login)  
✅ **Referral Program** - Share your code & earn from referrals  
✅ **Leaderboard** - Compete with top earners  
✅ **Withdrawals** - Convert coins to cash (Admin approved)  
✅ **Admin Panel** - Manage withdrawal requests  

## 📱 Live Demo

**Website:** https://Kleempwrld.github.io/k2-startup/

## ⚙️ Setup Instructions

### 1. Get Your Own Firebase Project
- Go to [Firebase Console](https://console.firebase.google.com/)
- Create new project (free tier)
- Enable:
  - **Authentication** → Email/Password
  - **Firestore Database** → Start in test mode

### 2. Update Firebase Config
Edit `index.html` (lines 85-92) with your Firebase credentials:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

### 3. Create Firestore Collections
In Firebase Console, create these collections:
- **users** - Stores user data
- **withdrawals** - Stores withdrawal requests

### 4. Set Admin Email
Change line 98 to your email:
```javascript
const ADMIN_EMAIL = "your-email@gmail.com";
```

### 5. Deploy
Push changes to GitHub - it auto-deploys!

```bash
git add .
git commit -m "Update Firebase config"
git push origin main
```

## 🎮 How to Use

1. **Sign Up** - Create account with email & password
2. **Complete Tasks** - Earn K-coins from available tasks
3. **Invite Friends** - Share your referral code for bonuses
4. **Withdraw** - Request to cash out your balance (admin approval needed)

## 📊 Task Rewards
- Watch Ad: **+K2**
- Litter Picking: **+K3**
- Daily Login: **+K1**

## 🔐 Security Notes
- Use your own Firebase project (never share credentials)
- Set Firestore rules for production
- Keep admin email private

## 📝 License
Free to use and modify

---

**Questions?** Check Firebase docs or GitHub Issues.
