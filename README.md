# 💧 Water Leakage and Loss Analyzer

<p align="center">
  <strong>A Python & Oracle Database Project for Smart Water Loss Monitoring</strong>
</p>

<p align="center">
  Tracking Leakage Incidents • Estimating Water Loss • Supporting Smarter Maintenance Decisions
</p>

---

## 🎓 Course-End Project

- **Project Title:** Water Leakage and Loss Analyzer
- **Project Type:** Course-End Project
- **Domain:** Environment
- **Course:** Python Programming Laboratory
- **Technologies:** Python, Oracle Database, SQL

## 🌊 About the Project

Water is one of our most valuable natural resources, and leakage can lead to significant water wastage and maintenance costs.

**Water Leakage and Loss Analyzer** is a Python-based application integrated with Oracle Database that records water leakage incidents, calculates estimated water loss, identifies recurring leakage locations, and generates reports to support maintenance decisions.

Developed as part of our **Python Programming Laboratory Course-End Project**, this application applies programming and database concepts to a practical environmental problem, with a focus on water conservation and efficient leakage monitoring.

## ✨ Key Features

- 📝 **Incident Management** — Record and store water leakage incidents.
- ⏱️ **Duration Calculation** — Calculate leakage duration, including overnight repair times.
- 💧 **Water Loss Estimation** — Estimate water wastage based on duration and leakage rate.
- 🚦 **Priority Classification** — Classify incidents according to priority.
- 📍 **Location Analysis** — Analyze water loss by location.
- 🔁 **Recurring Incident Detection** — Identify locations with repeated leakage incidents.
- 🚨 **High-Priority Reports** — Display incidents requiring urgent attention.
- 🛠️ **Maintenance Recommendations** — Support maintenance planning using incident data.
- 🗄️ **Database Integration** — Store and retrieve records using Oracle Database.
- ✅ **Input Validation** — Validate user input and improve data reliability.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application logic and calculations |
| Oracle Database | Persistent data storage |
| SQL | Database schema and data operations |
| python-oracledb | Python-to-Oracle connectivity |

## 📁 Project Structure

```text
water-leakage-analyser/
├── README.md
├── .gitignore
├── database.sql
└── console/
    ├── water_leakage_pro.py
    ├── requirements.txt
    ├── dashboard.py
    ├── project_report.py
    └── test_dashboard.py
```

## ⚙️ Getting Started

### Prerequisites

Before running the application, ensure you have:

- Python 3.10 or later
- Oracle Database
- An Oracle database user with the required permissions
- The `python-oracledb` Python package

### 1. Clone the Repository

```bash
git clone https://github.com/hasinibantu/water-leakage-analyser.git
cd water-leakage-analyser
```

### 2. Install Dependencies

```bash
python -m pip install -r console/requirements.txt
```

### 3. Set Up the Database

Connect to your Oracle database schema and execute the `database.sql` script.

This script creates the `leakage_records` table used by the application.

### 4. Configure the Database Connection

The application uses the following database settings:

- **Username:** `water_user`
- **Database Service:** `localhost:1521/FREEPDB1`

Ensure the Oracle Database service is running and the database user has the required permissions.

The application prompts for the database password when it starts. Never publish database passwords or other credentials in your repository.

### 5. Run the Application

```bash
python console/water_leakage_pro.py
```

Use the interactive menu to record leakage incidents, view reports, analyze water loss, and review maintenance recommendations.

## 📊 Available Reports

1. View all leakage records
2. Analyze water loss by location
3. Identify recurring leakage locations
4. View high-priority incidents
5. Review maintenance recommendations

## 🧮 Water Loss Calculation

The application estimates water loss using the following formula:

**Water Loss (liters) = Duration (hours) × Leakage Rate (liters/hour)**

**Example:**

If a leakage incident lasts 5 hours and the leakage rate is 200 liters per hour:

`Water Loss = 5 × 200 = 1,000 liters`

The estimated water loss is **1,000 liters**.

## 🗃️ Database Schema

The `leakage_records` table contains the following fields:

| Column | Description |
|---|---|
| `incident_id` | Unique incident identifier |
| `location` | Leakage location |
| `leak_start` | Leakage start timestamp |
| `repair_time` | Repair completion timestamp |
| `duration_hours` | Calculated leakage duration |
| `loss_rate` | Estimated leakage rate in liters per hour |
| `water_loss` | Estimated water loss in liters |
| `leak_type` | Type of leakage |
| `priority` | Incident priority |

## 🔐 Security

- Do not commit database passwords or credentials.
- Use a dedicated database account with appropriate permissions.
- Keep private data and sensitive configuration files out of the repository.
- Review all files before pushing changes to GitHub.

## 🚀 Future Enhancements

- 📈 Interactive dashboard with charts and filters
- 🗺️ Map-based visualization of leakage locations
- 📅 Monthly and yearly water-loss trend analysis
- 🔢 Oracle sequences for safer concurrent incident ID generation
- 🔔 Alerts for recurring and high-priority incidents

## 👩‍💻 Author

**Bantu Hasini**

B.Tech — Computer Science and Engineering

🔗 **GitHub:** [@hasinibantu](https://github.com/hasinibantu)

---

<p align="center">
  💧 <em>Building practical solutions for water conservation through programming and data analysis.</em>
</p>
