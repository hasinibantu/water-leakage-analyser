# 💧 Water Leakage and Loss Analyzer

<p align="center">
  <strong>A Python & Oracle Database Project for Smart Water Loss Monitoring</strong>
</p>

<p align="center">
  Tracking leakage incidents • Estimating water loss • Supporting smarter maintenance decisions
</p>

---

## 🌊 About the Project

Water is one of our most valuable natural resources, and leakage can lead to significant water wastage and maintenance costs.

**Water Leakage and Loss Analyzer** is a Python-based application integrated with Oracle Database that records water leakage incidents, calculates estimated water loss, identifies recurring leakage locations, and generates reports to support maintenance decisions.

This project aims to make leakage monitoring more organized, data-driven, and efficient.

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
- ✅ **Input Validation** — Handle user input and improve data reliability.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application logic and calculations |
| Oracle Database | Persistent data storage |
| SQL | Database schema and data operations |
| python-oracledb | Python-to-Oracle connectivity |

## 📁 Project Structure

```text
water-leakage-analyzer-console/
├── README.md
├── database.sql
└── console/
    ├── water_leakage_pro.py
    ├── requirements.txt
    └── .gitignore
```

## ⚙️ Getting Started

### Prerequisites

- Python 3.10 or later
- Oracle Database
- An Oracle database user with the required permissions
- `python-oracledb` package

### 1. Clone the Repository

Replace `YOUR_USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR_USERNAME/water-leakage-analyzer-console.git
cd water-leakage-analyzer-console
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
- **Database service:** `localhost:1521/FREEPDB1`

Ensure the database service is running and the database user has the required permissions. The application prompts for the database password when it starts.

> 🔐 Never upload database passwords, credentials, or other secrets to GitHub.

### 5. Run the Application

```bash
python console/water_leakage_pro.py
```

Use the interactive menu to record leakage incidents, view reports, analyze water loss, and access maintenance recommendations.

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
