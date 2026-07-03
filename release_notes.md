## FraudShield v1.0.0 — Initial Release 🎉

**Release Date:** April 2026  
**Platform:** Windows 10 / Windows 11 (64-bit)

---

### What's New

Complete 8-module AI fraud detection desktop application, released as a standalone Windows installer. No Python installation required.

**Core System**
- Full PyQt5 desktop application with dark and light theme support
- Session-based authentication with bcrypt password hashing and account lockout
- SQLite3 database with Fernet-encrypted account numbers
- Role-based access control: Admin and Analyst roles

**AI & Machine Learning**
- 6 trained ML models: Logistic Regression, Random Forest, Decision Tree, SVM, Isolation Forest, K-Means
- Soft-voting ensemble model combining all 4 supervised classifiers
- Hybrid OR-gate model: flags fraud if Ensemble **or** Isolation Forest detects it
- Risk scoring (0–100) on every transaction
- AI controls in Admin Panel: configurable threshold (60–90%), model retraining

**Transaction Management**
- Manual transaction entry with account number encryption
- Bulk CSV import supporting 100,000+ records
- Edit and review transactions with real-time fraud status

**Alerts System**
- Real-time alerts generated for transactions above risk threshold
- Severity levels: Low, Medium, High
- Sound notifications (WAV) with toggle control
- Alert resolution and audit trail

**Analytics Dashboard**
- Live stat cards: total transactions, fraud count, revenue, risk score
- Trend comparison vs. previous period
- Charts: fraud trend line, risk score distribution, monthly bar comparison
- Animated splash screen on startup

**Reports & Export**
- Professional PDF reports via ReportLab with header, summary table, and charts
- Excel export via openpyxl
- Date range and status filters
- Downloadable directly from the Reports tab

**Admin Panel**
- User management: create, view, delete users
- System activity logs and login history
- Database backup and restore
- AI model controls and threshold configuration

---

### System Requirements

| | Minimum | Recommended |
|-|---------|-------------|
| OS | Windows 10 (64-bit) | Windows 11 (64-bit) |
| RAM | 4 GB | 8 GB |
| Disk | 2 GB free | 4 GB free |
| Python | Not required | Not required |

---

### Installation

1. Download `FraudShield_Setup.exe` from the assets below
2. Right-click → **Run as administrator**
3. Follow the setup wizard (default install: `C:\Program Files\FraudShield`)
4. Launch from the Desktop shortcut or Start Menu → FraudShield

---

### Default Login Credentials

```
Username: admin
Password: admin123
```

> ⚠️ Change the default password immediately after first login via Profile → Change Password.

---

### Key Capabilities

- AI fraud detection result in under 3 seconds per transaction
- Supports 100,000+ transaction records without performance degradation
- Fully offline — no internet connection required after installation
- Dark and light theme, switchable per user account
- All sensitive account numbers encrypted at rest with Fernet symmetric encryption

---

### Known Limitations

- **Windows only** — macOS and Linux are not supported in this release
- **Large CSV imports (50,000+ rows)** may take 2–3 minutes to process
- **First model training** after a fresh database requires 5–10 minutes
- Sound notifications use `winsound` and require a Windows audio device

---

### Files in This Release

| File | Description |
|------|-------------|
| `FraudShield_Setup.exe` | Windows installer — run this to install |

---

### Team

| Name | Contribution |
|------|-------------|
| Zainab | AI Model Development & Backend |
| Aqsa Nadeem | Database Design & Desktop UI |
| Zainab Minahil | Reporting, Integration & Deployment |

**Project Advisor:** Prof. Muzammil Sadiq  
**University:** University of Central Punjab, Lahore  
**Group ID:** G1F22FYPCS011  
**Academic Year:** 2025–2026

---

*This software was developed as a Final Year Project for academic purposes only. All rights reserved © 2026.*
