# FraudShield — AI-Based Financial Fraud Detection System

![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat&logo=python&logoColor=white)
![PyQt5](https://img.shields.io/badge/PyQt5-5.15-41CD52?style=flat&logo=qt&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.9-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-3-003B57?style=flat&logo=sqlite&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows%2010%2F11-0078D4?style=flat&logo=windows&logoColor=white)
![License](https://img.shields.io/badge/License-Academic-lightgrey?style=flat)

> AI-powered desktop application for real-time financial fraud detection. Built with ensemble machine learning, role-based access control, and professional reporting tools.

---

## ⬇️ Download

**[⬇️ Download FraudShield v1.0.0 for Windows](https://github.com/Zainab157/FraudShield/releases/latest)**

Windows 10/11 • 64-bit • No Python required • Free

---

## Features

| Module | Description |
|--------|-------------|
| 🔐 **Authentication** | Secure login with bcrypt hashing, account lockout, and session timeout |
| 💳 **Transaction Management** | Add, edit, view, and bulk-import transactions via CSV |
| 🤖 **AI Fraud Detection** | 6 ML models + soft-voting ensemble + hybrid OR-gate classifier |
| 🔔 **Real-Time Alerts** | Instant fraud alerts with sound notifications and severity levels |
| 📊 **Analytics Dashboard** | Live charts — fraud trends, risk distribution, monthly comparisons |
| 📁 **Reports & Export** | Professional PDF and Excel reports with date filters |
| 🛡️ **Admin Panel** | User management, AI controls, system logs, database backup/restore |
| 👤 **User Profiles** | Avatar upload, password change, personal settings, theme switcher |

---

## Screenshots

| Dashboard | Alerts |
|-----------|--------|
| *(screenshot — login and run the app to view)* | *(screenshot)* |

| Reports | Admin Panel |
|---------|-------------|
| *(screenshot)* | *(screenshot)* |

---

## How It Works

```
1. Import Transactions          2. Run AI Detection             3. View Alerts & Reports
─────────────────────           ────────────────────────        ────────────────────────
Add manually or upload     →    6 ML models vote on each   →   Flagged transactions
CSV files with thousands        transaction in real time.       appear as alerts.
of transaction records.         Risk score 0–100 assigned.      Export PDF or Excel.
```

---

## Tech Stack

| Layer | Technology | Version |
|-------|-----------|---------|
| GUI Framework | PyQt5 | 5.15.11 |
| Machine Learning | scikit-learn | 1.9.0 |
| Data Processing | pandas, numpy | 2.2.3 / 2.4.6 |
| Visualisation | matplotlib, seaborn | 3.11.0 / 0.13.2 |
| Database | SQLite3 | Built-in |
| PDF Reports | reportlab | 5.0.0 |
| Excel Export | openpyxl | 3.1.5 |
| Encryption | cryptography (Fernet) | 49.0.0 |
| Password Hashing | bcrypt | 5.0.0 |
| Packaging | PyInstaller | 6.21.0 |

### AI Models

| Model | Use Case |
|-------|----------|
| Logistic Regression | Linear baseline classifier |
| Random Forest | High-accuracy ensemble tree model |
| Decision Tree | Interpretable rule-based detection |
| SVM (RBF Kernel) | Non-linear boundary classifier |
| Isolation Forest | Unsupervised anomaly detection |
| K-Means Clustering | Unsupervised grouping of transaction patterns |
| **Soft-Voting Ensemble** | Combined prediction from all 4 supervised models |
| **Hybrid OR-Gate** | Flags if Ensemble **or** Isolation Forest detects fraud |

---

## Installation

### Option A — Windows Installer (Recommended)

1. Go to [Releases](https://github.com/Zainab157/FraudShield/releases/latest)
2. Download `FraudShield_Setup.exe`
3. Double-click to run the installer (admin rights required)
4. Follow the setup wizard
5. Launch FraudShield from the Desktop shortcut or Start Menu
6. Login with: **username:** `admin` / **password:** `admin123`

> ⚠️ Change the default password after first login.

### Option B — Run from Source

**Requirements:** Python 3.12, pip

```bash
git clone https://github.com/Zainab157/FraudShield.git
cd FraudShield
pip install -r requirements.txt
python main.py
```

---

## System Requirements

| Requirement | Minimum | Recommended |
|-------------|---------|-------------|
| OS | Windows 10 (64-bit) | Windows 11 (64-bit) |
| RAM | 4 GB | 8 GB |
| Disk Space | 2 GB | 4 GB |
| Python | Not needed (installer) | 3.12+ (source) |
| Internet | Not required | Not required |

---

## Project Structure

```
FraudShield/
├── main.py                  # Entry point
├── scheduler.py             # Daily backup scheduler
├── gui/                     # PyQt5 windows and views
│   ├── dashboard.py         # Main dashboard
│   ├── admin_panel.py       # Admin panel (users, AI, logs)
│   ├── alerts_view.py       # Alerts module
│   ├── reports_view.py      # Reports & export module
│   └── ...
├── modules/                 # Core business logic
│   ├── fraud_detector.py    # All ML models + ensemble
│   ├── preprocessing.py     # Feature engineering
│   ├── transaction_mgmt.py  # Transaction CRUD
│   └── user_management.py   # User accounts
├── utils/
│   ├── paths.py             # PyInstaller-safe path resolver
│   └── encryption.py        # Fernet account number encryption
├── models/                  # Trained .pkl model files
├── database/                # SQLite database
├── Assests/                 # Sounds and images
├── requirements.txt
└── fraudshield.spec         # PyInstaller build spec
```

---

## Team

| Name | Role |
|------|------|
| **Zainab** | AI Model Development & Backend |
| **Aqsa Nadeem** | Database Design & Desktop UI |
| **Zainab Minahil** | Reporting, Integration & Deployment |

**Project Advisor:** Prof. Muzammil Sadiq  
**University:** University of Central Punjab, Lahore  
**Group ID:** G1F22FYPCS011  
**Completion:** April 2026

---

## Academic Notice

This software was developed as a Final Year Project for academic purposes at the University of Central Punjab, Lahore. It is not intended for commercial use. All rights reserved © 2026.

---

*[🌐 Project Website](https://Zainab157.github.io/FraudShield) • [📦 Releases](https://github.com/Zainab157/FraudShield/releases) • [📋 Issues](https://github.com/Zainab157/FraudShield/issues)*
