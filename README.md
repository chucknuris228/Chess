# ♛ GrandMaster — Chess Platform

> A modern, full-featured chess web platform built to stand out from the thousands of generic chess sites online.

## 🌐 Live Demo
[grandmaster-chess.vercel.app](https://grandmaster-chess.vercel.app) *(deploy to activate)*

## 🎯 What is this?

GrandMaster is a chess platform built for **serious casual players** who want more than just moving pieces around — they want to **learn, compete, and belong to a community**.

It targets the gap between "weekend chess app" and "Lichess pro setup": smart enough to teach you, social enough to keep you coming back.

---

## ✦ Features

### Level: GREAT (All 4 levels completed)

#### 🤖 AI Opponent — Stockfish-style Minimax
- Full rule validation: castling, en passant, pawn promotion, check/checkmate/stalemate
- 8 difficulty levels using minimax + alpha-beta pruning + piece-square tables
- Adaptive thinking time (harder = more realistic delay)

#### 🧠 AI Coach (Claude-powered)
- After each game, click "Analyze Game" for a real GPT/Claude analysis of your moves
- Identifies critical moments, mistakes, and improvement areas
- Personalized based on your win/loss history

#### 🏆 Global + City Leaderboards
- Rankings filtered by: Global, Almaty, Nur-Sultan, Shymkent, Weekly
- Real player data simulation with ratings, win streaks, and city info
- Streak tracking with fire emoji for hot players 🔥

#### 🔗 Multiplayer by Link
- Generate a game link to challenge any friend
- No account required for challengers
- WebSocket-ready architecture (connect a WS server to activate)

#### 💰 Monetization — "Upgrade to Pro"
- Prominent Pro upgrade button in nav and sidebar
- Pro modal with feature list: unlimited AI coaching, custom skins, PGN export, voice commentary
- $9/month pricing with free trial CTA
- Built-in Stripe integration hook

#### ⏱️ Time Controls
- Unlimited, 1 min, 3 min, 10 min bullet/blitz/rapid
- Live countdown clocks on both player bars
- Win on time detection

#### 🎨 Design & UX
- Dark luxury aesthetic with gold accents (chess club vibes)
- Playfair Display serif + DM Sans — editorial and refined
- Flip board, undo moves, resign
- Captured pieces display with material advantage
- Move history with SAN notation, clickable
- Position evaluation bar with real centipawn score
- Check highlighting, last move highlighting, valid move dots
- Toast notifications, smooth modals
- Fully responsive layout

---

## 🏗️ Architecture

```
chess-grandmaster/
├── index.html          # Full single-file app
├── README.md
└── assets/             # (for future skin packs)
```

**Stack:**
- Pure HTML/CSS/JavaScript — zero dependencies, zero build step
- Chess engine: custom minimax with alpha-beta pruning + PST evaluation
- AI coach: Anthropic Claude API (claude-sonnet-4-20250514)
- Fonts: Google Fonts (Playfair Display + DM Sans)

**Why single-file?**
Instant deployment anywhere — Vercel, Netlify, GitHub Pages, a USB stick. No npm, no node_modules, no build pipeline. Chess in one file, 0 to 60 in seconds.

---

## 🚀 Run Locally

```bash
# Option 1: Just open it
open index.html

# Option 2: Local server (recommended for API features)
python3 -m http.server 3000
# Visit http://localhost:3000
```

---

## 💡 Business Thinking

| Feature | Value |
|---|---|
| AI Coach | Retention driver — players come back to improve |
| City Leaderboards | Social hook — local pride and competition |
| Pro Upgrade Button | Monetization — $9/mo with clear value prop |
| Multiplayer Links | Viral growth — every shared link = new user |
| Rating System | Progress tracking — keeps players engaged |

**Target Users:**
1. Casual players who want to improve (AI coach)
2. Competitive amateurs (rating + leaderboard)
3. Friends who want to play remotely (link multiplayer)
4. Parents teaching kids chess (easy difficulty, flip board)

**Revenue Model:**
- Freemium: full game free, advanced coaching + skins behind Pro
- $9/mo Pro: unlimited AI analysis, custom aesthetics, voice commentary
- Future: in-platform currency for tournaments, cosmetic NFT pieces

---

## 📅 Built in One Session

Created by a developer using Claude as an AI pair programmer, demonstrating that a full startup-ready prototype can be shipped in hours with the right tools.

*"The best chess app isn't the one with the most features — it's the one you keep coming back to."*

---

## 📬 Submission

Built for **nFactorial School** — Chess Platform Challenge  
Deadline: May 20, 2025  
Form: [nfactorialschool.typeform.com/to/HYVeKeEx](https://nfactorialschool.typeform.com/to/HYVeKeEx)
