# Mathematicoo — Math Game

A web-based math game where players sign up, answer timed maths questions, and compete on a global leaderboard — built with **Next.js** and **Firebase**.

![demo](./Images/demo.gif)

Built by **Chelsi Patel**.

---

## ✨ Features
- **User accounts** — register and log in with Firebase Authentication.
- **The game** — answer maths questions and rack up a score.
- **Global leaderboard** — scores saved to Firestore and ranked across all players.
- **Animated, responsive UI** — built with Tailwind CSS and Framer Motion.

## 🛠️ Tech stack
| Layer | Technology |
|-------|------------|
| Framework | Next.js (React 17) |
| Auth & Database | Firebase Authentication + Cloud Firestore |
| Styling | Tailwind CSS |
| Animation | Framer Motion |
| Forms | react-hook-form |

## 📂 Key files
```
Pages/
├── index.js        # home
├── register.js     # sign up
├── login.js        # sign in
├── game.js         # the math game
└── ladderboard.js  # leaderboard
Components/
├── fb.js           # Firebase initialisation (web config)
├── LadderboardTable.js / TableRow.js
└── Button.js / Logo.js / Background.js
providers/
└── authprovider.js # auth context
```

## 🚀 Running locally
Requires Node.js and your own Firebase project (Auth + Firestore enabled).
```bash
npm install
npm run dev
```
Then open **http://localhost:3000**.

> Note: the Firebase **web** config in `Components/fb.js` is a public client identifier (not a secret). Access is controlled by Firebase security rules.
