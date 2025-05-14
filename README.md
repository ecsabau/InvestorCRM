# InvestorCRM
InvestorCRM is an intelligent, self-hosted Customer Relationship Management (CRM) platform designed for investment professionals, VC firms, and private investors. It blends classic CRM features with AI-driven lead analysis, deal tracking, and client interaction insights—all hosted privately on your own server infrastructure.

# 🚀 Features
```
✅ Lead Management – Add, score, and track potential investors or clients.

🧠 AI-Powered Insights – Automatic lead scoring, email summarization, and smart recommendations.

🔐 Private Hosting – Secure deployment on your own AWS EC2 instance.

📅 Activity Tracking – Log meetings, calls, and deal milestones.

📈 Deal Flow Pipeline – Visual Kanban board for tracking the progress of investment opportunities.

🌙 Dark Mode Support – User-friendly dark/light theme toggle.

🧩 Modular Backend – Built with Flask and SQLAlchemy for flexible API expansion.

📁 Firebase Frontend – Responsive, modern UI deployed using Firebase.
```

# 🏗️ Tech Stack
``` 
Layer	Technology
Frontend	React (or HTML/CSS + Firebase Hosting)
Backend	Python Flask + SQLAlchemy
Database	PostgreSQL (hosted on AWS EC2)
AI Engine	DeepSeek, OpenAI APIs
Deployment	Nginx + Gunicorn on EC2
```

# 📂 Project Structure
```
InvestorCRM/
├── app/
│   ├── models.py        # SQLAlchemy models for users, leads, clients, deals
│   ├── routes.py        # Flask routes (API endpoints)
│   ├── ai/
│   │   └── scorer.py    # AI lead scoring logic
│   └── ...
├── static/              # Frontend assets (optional)
├── templates/           # HTML files if using Jinja
├── run.py               # App entry point
├── requirements.txt
├── config.py
└── README.md
```

# ⚙️ Installation
```
Backend (Flask + PostgreSQL)
```
1. Clone the repo:
```
git clone https://github.com/yourusername/InvestorCRM.git
cd InvestorCRM
```
2.Create virtual environment & install dependencies:
```
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
3.Configure database:
```
Edit config.py or set environment variables for your PostgreSQL connection.
```
4.Create tables:
```
from app import db
db.create_all()
```
5.Run the app:
```
python run.py
```

# ☁️ Deployment (EC2 Server + Gunicorn + Nginx)
```
Make sure:

Your Flask app is reachable through gunicorn.

Nginx is reverse proxying to your Flask server.

PostgreSQL is accessible and configured with appropriate user credentials.

You can follow this deployment guide or ask me for a tailored step-by-step setup.
```

# 📬 Contact
```
Built with 💼 by NextGen AI Solutions
Need support or custom features? Reach out at: support@nextgenaisolutions.co.uk
```

# 📝 License
```
This project is under the MIT License – see the LICENSE file for details.
```
