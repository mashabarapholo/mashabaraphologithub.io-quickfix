# 🔧 QuickFix — Service Request Tracker

A lightweight, browser-based service request management app built for the QuickFix home appliance repair startup. No frameworks, no databases, no install — just open and run.

---

## 📸 Features

- ✅ **Submit** service requests with customer name, appliance type, priority, and issue description
- ✅ **View** all requests in a live, searchable dashboard
- ✅ **Update** request status — Pending → In Progress → Completed
- ✅ **Delete** requests with confirmation
- ✅ **Filter** by status and search by name or appliance in real time
- ✅ **Live stats** — total, pending, in-progress, and completed counts update instantly

---

## 🚀 Getting Started

### Option 1 — Open directly (simplest)
Just double-click `quickfix_app.html` in your file explorer. It opens straight in your browser — no setup needed.

### Option 2 — Local server via Python
```bash
# Navigate to the project folder
cd path/to/quickfix

# Start a local server
python -m http.server 8000
```
Then visit: [http://localhost:8000/quickfix_app.html](http://localhost:8000/quickfix_app.html)

### Option 3 — VS Code Live Server
1. Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Right-click `quickfix_app.html`
3. Click **"Open with Live Server"**

---

## 🗂️ Project Structure

```
quickfix/
├── quickfix_app.html       # The full application (single file)
├── QuickFix_Project_Report.docx  # Technical report & code review
└── README.md               # You are here
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | HTML5, CSS3, Vanilla JavaScript (ES6+) |
| Architecture | IIFE module pattern (RequestStore + UI) |
| Storage | In-memory array (session-scoped) |
| Fonts | Syne, JetBrains Mono, Inter (Google Fonts) |
| Dependencies | None |

---

## 💡 Design Decisions

- **No framework** — Vanilla JS keeps the app dependency-free and instantly deployable as a single file
- **Module pattern** — `RequestStore` separates data logic from UI; swap storage backends without touching the UI
- **DRY principles** — `buildCard()`, `validate()`, and `getField()` eliminate repetition across the codebase
- **XSS protection** — `escapeHtml()` sanitizes all user input before rendering to the DOM

---

## 📋 Assignment Context

Built as part of a software development case study for **QuickFix**, a fictional on-demand appliance repair startup. The goal was to demonstrate clean, modular code, feature implementation, and deployment — simulating a real team development environment.

---

## 👤 Author

**Mashaba Rapholo**  
https://github.com/mashabarapholo/
