# 🔐 CipherCheck — Password Security Analyzer

> Real-time password strength analysis with entropy calculation, crack time estimation, and breach detection. Runs 100% in the browser — your password never leaves your device.

![CipherCheck](https://img.shields.io/badge/CipherCheck-v1.0-00e5ff?style=for-the-badge&logo=shield&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![No Backend](https://img.shields.io/badge/No_Backend-Client_Side_Only-39ff14?style=for-the-badge)

---

## 🖥️ Live Demo

👉 **[Try it here](https://https://cipher-check.netlify.app/)**

---

## ✨ Features

- **Real-time analysis** — results update instantly as you type, no button needed
- **Shannon entropy calculation** — mathematically measures true password randomness in bits
- **GPU crack time estimation** — simulates a 100 billion guesses/second attack to estimate how long your password would survive
- **Character map visualizer** — each character color-coded by type (uppercase / lowercase / digit / symbol)
- **8 composition checks** — length, uppercase, lowercase, digits, symbols, repeated chars, sequences, common words
- **Breach database detection** — checks against 200 most commonly breached passwords
- **Security recommendations** — specific, actionable fixes based on what's weak
- **Strong password generator** — generates cryptographically randomized 16-character passwords
- **Zero data transmission** — everything runs locally, nothing is sent to any server

---

## 🧠 How It Works

### Entropy Calculation
Entropy is calculated using the formula:

```
H = L × log₂(N)
```

Where:
- `H` = entropy in bits
- `L` = password length
- `N` = size of character set used (lowercase=26, uppercase=26, digits=10, symbols=32)

Higher entropy = exponentially harder to crack.

### Crack Time Estimation
Assumes a real-world GPU cluster attack at **100 billion guesses/second** — a realistic benchmark for a motivated attacker with modern hardware. Crack time = `2^entropy / (2 × guesses_per_sec)` (average half keyspace traversal).

### Breach Detection
Checks the entered password against a local list of the 200 most commonly used/breached passwords. Runs entirely in-browser using a JavaScript `Set` for O(1) lookup — no API calls, no network requests.

---

## 🚀 Usage

No installation. No dependencies. No server.

```bash
# Just open the file
open passwd-analyzer.html
```

Or deploy to any static host — Netlify, GitHub Pages, Vercel.

---

## 📊 Scoring Breakdown

| Score | Rating | Meaning |
|-------|--------|---------|
| 0–19 | ■ CRITICAL | Crackable in seconds |
| 20–39 | ▲ WEAK | Crackable in minutes/hours |
| 40–59 | ◆ MODERATE | Some resistance, needs improvement |
| 60–79 | ● STRONG | Good password |
| 80–100 | ★ FORTRESS | Excellent — highly resistant |

---

## 🛡️ Security & Privacy

- **No backend** — zero server-side code
- **No API calls** — breach check runs on a local dataset
- **No logging** — nothing is stored or transmitted
- **No dependencies** — pure vanilla HTML/CSS/JS, no npm, no frameworks
- Safe to use with real passwords

---

## 🗂️ Project Structure

```
passwd-analyzer.html   ← entire app in a single file
README.md              ← this file
```

---

## 🔧 Tech Stack

- **Vanilla JavaScript** — all analysis logic
- **HTML5 / CSS3** — UI with terminal/cyberpunk aesthetic
- **No frameworks, no libraries, no build tools**

---

## 👤 Author

**Muhammad Taha Sheikh**
BS Cybersecurity · Karachi, Pakistan

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/tahahahaa)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tahaahmed1877@gmail.com)

---

## 📄 License

MIT — free to use, modify, and distribute.

---

<div align="center">
<sub>// Zero trust. Zero transmission. Pure analysis.</sub>
</div>
