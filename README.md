[README.md](https://github.com/user-attachments/files/26494362/README.md)
# 🐝 Funny Bee — Learn English for Kids!

A fun, interactive English learning app designed for children aged 3–6. Learn vocabulary through colorful flashcards, games, and sounds — all in your browser!

![Funny Bee](https://img.shields.io/badge/Funny%20Bee-Learn%20English-f582ae?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0naHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmcnIHZpZXdCb3g9JzAgMCAxMDAgMTAwJz48dGV4dCB5PScuOWVtJyBmb250LXNpemU9JzkwJz7wn5CdPC90ZXh0Pjwvc3ZnPg==)
![PWA](https://img.shields.io/badge/PWA-Supported-6bcb77?style=for-the-badge)
![React](https://img.shields.io/badge/React-19-61dafb?style=for-the-badge&logo=react)

## ✨ Features

### 📖 Learn Words
Browse 40 vocabulary words across 4 categories — **Animals**, **Fruits**, **Colors**, and **Numbers**. Each word comes with:
- Emoji visual
- IPA phonetic transcription
- Example sentence
- Text-to-Speech pronunciation

### 🧩 Memory Match
Flip cards and match emoji–word pairs. Tracks moves and pairs found.

### ❓ Quiz Time
Listen to a word and choose the correct picture from 4 options. 8 questions per round with star scoring (⭐/🌟/🏆).

### 🎨 Word Builder
Spell words by tapping letter tiles. Includes distractor letters to add challenge.

### 🖼️ Puzzle
Jigsaw-style puzzle game with 9 difficulty levels (2×2 → 10×10).
- Easy levels (2×2 – 4×4): emoji-based puzzles
- Hard levels (5×5+): Vietnamese landmarks 🇻🇳 (Hạ Long Bay, Hội An, Golden Bridge...)

### 🎉 Encouragement System
- Motivational messages on every correct answer
- Special celebration for 3-win streaks
- Confetti animation on victories

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | React 19 + Vite 6 |
| Routing | react-router-dom 7 (HashRouter) |
| Styling | Vanilla CSS with custom design system |
| Font | [Quicksand](https://fonts.google.com/specimen/Quicksand) (Google Fonts) |
| Audio | Web Speech API (TTS) + AudioContext (SFX) |
| PWA | Service Worker + Web App Manifest |
| Deploy | GitHub Pages via `gh-pages` |

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v18+)

### Install & Run
```bash
npm install
npm run dev
```
Open http://localhost:5173/funny-bee-english/ in your browser.

### Build for Production
```bash
npm run build
```
Static files will be generated in the `dist/` folder.

### Deploy to GitHub Pages
```bash
npm run deploy
```

## 📁 Project Structure

```
├── index.html              # Entry HTML
├── public/
│   ├── manifest.json       # PWA manifest
│   ├── sw.js               # Service worker
│   └── images/             # Word & landmark images
├── src/
│   ├── App.jsx             # Root component with routing
│   ├── main.jsx            # React entry + SW registration
│   ├── index.css           # Full design system
│   ├── components/
│   │   ├── Navigation.jsx  # Sidebar nav
│   │   ├── Confetti.jsx    # Win animation
│   │   └── Encouragement.jsx # Motivational messages + streak hook
│   ├── pages/
│   │   ├── Home.jsx        # Landing page
│   │   ├── LearnWords.jsx  # Flashcard module
│   │   ├── MemoryGame.jsx  # Card matching game
│   │   ├── QuizGame.jsx    # Listen & pick quiz
│   │   ├── WordBuilder.jsx # Letter spelling game
│   │   └── PuzzleGame.jsx  # Jigsaw puzzle
│   ├── data/
│   │   └── words.js        # 40 words, 4 categories
│   └── utils/
│       └── speech.js       # TTS + sound effects
└── vite.config.js          # Vite config (base path)
```

## 📱 PWA Support

Funny Bee works offline as a Progressive Web App. Install it on your phone's home screen for a native app experience!

## 📄 License

MIT

---

Made with 💛 for little learners everywhere.
