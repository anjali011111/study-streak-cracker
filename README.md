# 🎓⚡ Study Streak Cracker

> **A gamified learning platform for CAI-A (Batch 24–28)**  
> Turn your study grind into an RPG — earn XP, level up, and crack the streak!

  deployed link: https://anjali011111.github.io/study-streak-cracker/
---

## 📸 Overview

**Study Streak Cracker** is a single-file, browser-based gamified study dashboard designed for students. It wraps everyday academic activities — attending class, completing tasks, tracking work — inside an RPG-style progression system with XP, levels, streaks, and mini-games.

No backend. No install. Just open the HTML file and start playing.

---

## ✨ Features

### 🗺️ Level Map
- Visual RPG-style progression map with **8 unlockable levels**
- Levels include: Daily Mission → Class Notes → Task Quest → Notifications → Talents → Opportunities → Govt Jobs → Person of Week
- Completed nodes glow gold; active nodes pulse red; locked nodes are dimmed

### 📊 Stats & Ranking
- Real-time **XP bar** with rank titles (Rookie Scholar → ...)
- Stat pills tracking: Total XP ⚡ · Stars ⭐ · Day Streak 🔥 · Level 🔮
- XP and level persist across navigation within the session

### 📚 Class Notes
- Study material organized by subject
- Earn **+20 XP** for visiting the notes section

### 📋 Work Tracker
- Attendance grid showing Present / Absent / Skip days
- Weekly stats: Hours studied, Tasks completed, Streak, Sessions

### ⚔️ Tasks
- Mission-style task list with XP rewards per task
- Priority indicators and owner tags

### 🔔 Notifications
- In-app alert system with unread badge counter
- Blinking alert bar on the home screen

### 🏆 Person of Week
- Hall of Fame spotlight for top-performing students

### ✨ Talents
- Showcase section for student skills and achievements

### 🔓 Opportunities
- Listings for Hackathons, Internships, Scholarships
- Color-coded by type (purple = hackathon, teal = internship, gold = scholarship)

### 🎮 Mini-Games (earn XP by playing!)
| Game | Mechanic | Max XP |
|------|----------|--------|
| 🧠 Quiz Blitz | 5-question MCQ quiz | +50 XP |
| 🃏 Memory Match | Flip-card emoji pairs (4×4 grid) | +25 XP |
| 👆 Tap Frenzy | Tap as fast as possible in 10 seconds | +30 XP |

---

## 🚀 Getting Started

### Option 1 — Just open it
```bash
# Clone the repo
git clone https://github.com/your-username/study-streak-cracker.git

# Open in browser
open study-streak-cracker-v2.html
```
No server needed. Works in any modern browser.

### Option 2 — Serve locally (optional)
```bash
# Python 3
python -m http.server 8080

# Then visit
http://localhost:8080/study-streak-cracker-v2.html
```

---

## 🗂️ Project Structure

```
study-streak-cracker/
├── study-streak-cracker-v2.html   # Entire app — HTML + CSS + JS in one file
└── README.md
```

Everything lives in a single self-contained HTML file — no dependencies to install, no build step required.

---

## 🎨 Tech Stack

| Layer | Technology |
|-------|-----------|
| Structure | HTML5 |
| Styling | CSS3 (custom properties, animations, flexbox/grid) |
| Logic | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts — Creepster, Rajdhani, Share Tech Mono |

**Zero external dependencies** beyond Google Fonts (loaded via CDN).

---

## 🧩 Customization Guide

### Change the batch name
Find and replace `CAI-A (24–28)` in the HTML:
```html
<div class="hero-sub">CAI-A (24–28) · Gamified Learning Platform</div>
```

### Add quiz questions
Locate the `Qs` array in the `<script>` section and add objects following this pattern:
```js
{ q: 'Your question here?', opts: ['A', 'B', 'C', 'D'], ans: 0 }
// ans = index of the correct option (0-based)
```

### Add opportunities
Find the opportunities section in the HTML and add entries using the existing `.opp` card structure:
```html
<div class="opp hack">
  <span class="opp-tag tag-open">OPEN</span>
  <div class="opp-title">Opportunity Name</div>
  <div class="opp-meta">
    <span>📅 Deadline</span>
    <span>🏢 Organizer</span>
  </div>
</div>
```

### Adjust XP thresholds
Find the `ranks` array in the script and edit level names and XP breakpoints:
```js
const ranks = [
  { name: 'Rookie Scholar', xpNeeded: 100 },
  ...
];
```

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

1. Fork the repo
2. Create your feature branch: `git checkout -b feature/cool-new-thing`
3. Commit your changes: `git commit -m 'Add cool new thing'`
4. Push to the branch: `git push origin feature/cool-new-thing`
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">
  Made with ❤️ for the CAI-A batch &nbsp;·&nbsp; Study hard, streak harder 🔥
</div>
