# 📚 Student Task Reminder System

![n8n](https://img.shields.io/badge/Built%20With-n8n-orange)
![Google Sheets](https://img.shields.io/badge/Database-Google%20Sheets-green)
![Gmail](https://img.shields.io/badge/Notifications-Gmail-red)
![Frontend](https://img.shields.io/badge/Frontend-HTML%20%7C%20JavaScript-blue)
![Automation](https://img.shields.io/badge/Automation-Workflow-yellow)
![Status](https://img.shields.io/badge/Project-Active-success)

A simple **automation system for students** to never miss assignments again ⏰📚  

Built during my **n8n learning journey 🚀**

---

# 🌟 Project Overview

Managing assignments can be stressful. Students often forget deadlines or lose track of tasks.

This project solves that problem using **automation**.

Students submit tasks through a **simple webpage**, and the system automatically sends **email reminders** before deadlines.

Everything runs automatically using **n8n workflows** — no backend server required.

---

# 🧠 How It Works

```
Student Form
      │
      ▼
n8n Webhook
      │
      ▼
Google Sheets (Store Tasks)
      │
      ▼
Daily Scheduled Workflow
      │
      ▼
Check Deadlines
      │
      ▼
Send Email Reminders
      │
      ▼
Mark Task Completed via Email Button
```

---

# ✨ Features

✅ Add tasks through a **clean webpage**  
📊 Store tasks automatically in **Google Sheets**  
⏰ **Daily automatic reminder system**

📩 Email reminders for:
- 🚨 Overdue tasks
- 📅 Tasks due today
- 🔔 Tasks due tomorrow

🖱️ **One-click "Mark as Completed" button in email**

🧠 Smart logic:
- No manual **status column**
- Status calculated from **deadline + Completed flag**

🛡️ **Duplicate reminder protection**
- Uses **ReminderSent column**

⚡ Fully automated workflow

---

# 🛠 Tech Stack

| Technology | Purpose |
|-------------|--------|
| ⚙️ n8n | Automation workflows |
| 📊 Google Sheets | Task storage |
| 📧 Gmail | Email notifications |
| 🌐 HTML | Task input form |
| 🧠 JavaScript | Form logic |

---

# 📂 Repository Structure

```
Student-Task-Reminder/
│
├── workflow.json        # n8n automation workflow
├── index.html           # task input webpage + frontend logic
│
├── screenshots/         # project screenshots
│   ├── workflow.png
│   ├── webpage.png
│   ├── email.png
│   └── sheet.png
│
└── README.md
```

---

# 📸 Screenshots

(Add your screenshots in the repository)

### 🧩 n8n Workflow
`screenshots/workflow.png`

### 🌐 Task Submission Webpage
`screenshots/webpage.png`

### 📩 Email Reminder
`screenshots/email.png`

### 📊 Google Sheet Storage
`screenshots/sheet.png`

---

# ⚙️ Setup Guide

## 1️⃣ Import Workflow

Import the provided file into **n8n**

```
workflow.json
```

---

## 2️⃣ Configure Credentials

Add credentials for:

- 📊 Google Sheets
- 📧 Gmail

---

## 3️⃣ Update Webhook URL

Update the webhook URL in your frontend code.

```javascript
const WEBHOOK_URL = "https://trochanteric-gladis-superlaryngeally.ngrok-free.dev/webhook/student-agent";
```

---

## 4️⃣ Deploy n8n

You can deploy n8n using:

- Railway
- Self-hosted server
- Docker
- Ngrok

Make sure the **scheduler workflow stays active**.

---

# 🚧 Challenges Faced

During development I encountered several issues:

⚠️ `row_number null / NaN` errors  
🔀 Query vs body parameter confusion  
🌐 CORS issues  

Solved everything step-by-step through debugging and experimentation.

---

# 🌱 Learning Outcome

Through this project I learned:

- n8n workflow automation
- webhook integrations
- Google Sheets automation
- email notification systems
- debugging automation pipelines

This is my **first real automation project** and I'm excited to keep improving it! 🚀

---

# 🤝 Contributions

Suggestions and improvements are welcome!

You can:

⭐ Star the repository  
🍴 Fork the project  
🐛 Open issues  
💡 Suggest improvements

---

# 🔖 Tags

`#n8n`  
`#Automation`  
`#NoCode`  
`#GoogleSheets`  
`#StudentTools`  
`#LearningInPublic`
