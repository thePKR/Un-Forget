<div align="center">

# 🧠 Spaced Repetition Learning System
### Combat the Ebbinghaus Forgetting Curve with Intelligent Review Scheduling

<br>

<img src="https://img.shields.io/badge/HTML-5-E34F26?logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS-3-1572B6?logo=css3&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/LocalStorage-Persistent%20State-blue" />
<img src="https://img.shields.io/badge/Cognitive%20Science-Spaced%20Repetition-purple" />
<img src="https://img.shields.io/badge/License-MIT-black" />

<br><br>

**A zero-backend, browser-native spaced repetition engine  
designed to optimize long-term memory retention.**

</div>

---

## 📚 The Problem

According to the Ebbinghaus Forgetting Curve:

- 50% of newly learned information is forgotten within 1 hour  
- ~70% is forgotten within 24 hours  
- Without structured review, retention collapses  

Most learners:

❌ Reread passively  
❌ Review randomly  
❌ Study without spacing logic  
❌ Forget systematically  

This system solves that.

---

# ⚙️ What This Application Does

Built entirely in **vanilla HTML + CSS + JavaScript**, this system:

- Stores learning items locally
- Automatically schedules review intervals
- Adjusts difficulty-based review spacing
- Tracks review count & mastery status
- Displays due / upcoming / mastered items
- Maintains persistence using `localStorage`

No server.  
No database.  
No login.  
Fully client-side cognitive engine.

---

# 🧠 Review Algorithm

### Adaptive Interval Scheduling

```javascript
if (difficulty === 'hard')
    days = 1.5^reviews
else if (difficulty === 'medium')
    days = 2^reviews
else
    days = 2.5^reviews
```

✔ Hard → Slower expansion  
✔ Medium → Balanced spacing  
✔ Easy → Aggressive interval growth  

Items move through:

```
New → In Progress → Mastered
```

Mastery threshold: ≥ 6 successful reviews

---

# 📊 Feature Overview

### 📌 Learning Management
- Add topic + notes
- Categorize (Math, Language, Science, etc.)
- Instant scheduling upon creation

### 🔄 Review Workflow
- “Due Now” detection
- Modal-based review interface
- Difficulty-based interval recalculation

### 📈 Analytics Dashboard
- Total Items
- Due Today
- Mastered Count
- Streak Days

### 💾 Persistent Storage
All data saved via:

```
localStorage.setItem("spacedRepetitionData", ...)
```

Zero backend dependency.

---

# 🖥 Interface Design

- Gradient modern UI
- Card-based item layout
- Review scheduling visualization
- Filter tabs:
  - All
  - Due
  - Upcoming
  - Mastered
- Modal-based review flow

---

# 🚀 How to Run

No installation required.

1. Download:
   `Combat_Forgetting_Curve.html`
2. Open in browser
3. Start adding learning items

That’s it.

Or host it:

```bash
python -m http.server
```

---

# 🧩 Architecture Overview

```
User Input
    ↓
Item Creation
    ↓
Schedule Generation
    ↓
Review State Machine
    ↓
Adaptive Interval Calculation
    ↓
LocalStorage Persistence
    ↓
Dynamic UI Rendering
```

---

# 🎯 Why This Is Not Just Another Flashcard App

Most flashcard systems:

- Require accounts
- Hide scheduling logic
- Store data remotely
- Are bloated

This system:

✔ Is fully transparent  
✔ Implements clear mathematical spacing logic  
✔ Requires no login  
✔ Runs offline  
✔ Gives complete control to the learner  

---

# 📈 Cognitive Science Alignment

Grounded in:

- Ebbinghaus Forgetting Curve
- Spaced Repetition Theory
- Retrieval Practice
- Adaptive Difficulty Scaling

Designed for:

- Exam preparation
- Language acquisition
- Concept-heavy disciplines
- Long-term knowledge retention

---

# 🧠 Ideal Users

- Students preparing for competitive exams
- Engineers learning frameworks
- Language learners
- Researchers
- Self-directed learners

---

# 🛠 Future Enhancements

<details>
<summary>Planned Upgrades</summary>

- SM-2 algorithm implementation (Anki-style)
- Export/Import JSON
- Visualization of memory decay curve
- Tag-based filtering
- Dark mode toggle
- Performance analytics (retention %)

</details>

---

# 👤 Author

Built as a cognitive performance tool  
by a systems-oriented learner.

---

<div align="center">

### Memory is not about intensity.  
### It is about interval.

</div>
