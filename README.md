# 🏥 Bed Slot Booking System

A comprehensive pandemic-era bed management solution built with Python and SQL, enabling hospitals to efficiently manage and book available bed slots during healthcare crises.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Database Schema](#database-schema)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

The **Bed Slot Booking System** is a web-based application designed to streamline hospital bed allocation during pandemics. It provides a centralized platform for healthcare administrators to manage bed availability, track patient admissions, and optimize resource utilization in real-time.

### Problem Statement
During health emergencies, hospitals face critical challenges in managing limited bed capacity and ensuring fair allocation of resources. This system provides an automated solution to address these challenges.

### Solution
A user-friendly platform that enables:
- Real-time bed availability tracking
- Efficient slot booking and cancellation
- Patient information management
- Resource optimization and reporting

## ✨ Features

- ✅ **Real-time Bed Management** - Track bed availability across multiple wards
- ✅ **Smart Slot Booking** - Automated allocation of beds to patients
- ✅ **User Authentication** - Secure login for hospital staff
- ✅ **Patient Records** - Comprehensive patient information management
- ✅ **Booking History** - Complete audit trail of all transactions
- ✅ **Responsive UI** - Works seamlessly on desktop and mobile devices
- ✅ **Data Analytics** - Generate insights on bed utilization rates
- ✅ **Cancellation Management** - Easy cancellation with rebooking options

## 🛠️ Tech Stack

| Technology | Purpose | Percentage |
|-----------|---------|-----------|
| **HTML** | Frontend Structure | 56.1% |
| **CSS** | Styling & Layout | 21.2% |
| **Python** | Backend Logic & API | 18.6% |
| **JavaScript** | Client-side Interactivity | 4.1% |

### Backend Framework
- Python 3.x
- Flask/Django (Framework)
- SQLAlchemy (ORM)

### Database
- SQL (MySQL/PostgreSQL)
- SQLite (for development)

### Frontend Libraries
- Bootstrap/CSS Framework
- JavaScript (Vanilla/jQuery)

## 📦 Installation

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)
- MySQL/PostgreSQL/SQLite
- Git

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Gokul-2004-cm/Bed_Slot_Booking-.git
   cd Bed_Slot_Booking-
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure database**
   - Update database credentials in `config.py`
   - Run migrations: `python migrate.py`

5. **Initialize database**
   ```bash
   python init_db.py
   ```

6. **Run the application**
   ```bash
   python app.py
   ```

   The application will be available at `http://localhost:5000`

## 🚀 Usage

### For Hospital Administrators
1. Log in with your credentials
2. Navigate to the **Dashboard** to view bed availability
3. Manage bed slots and ward assignments
4. View detailed reports and analytics

### For Medical Staff
1. Access the booking portal
2. Search for available beds by ward or specialization
3. Submit booking requests
4. Track booking status and receive confirmations

### For Patients/Admissions Team
1. Register in the system
2. Request bed slots based on requirements
3. Receive booking confirmation and ward details
4. Manage cancellations if needed

## 📁 Project Structure

```
Bed_Slot_Booking-/
├── app.py                 # Main application entry point
├── config.py              # Configuration settings
├── requirements.txt       # Python dependencies
├── init_db.py             # Database initialization
├── migrate.py             # Database migrations
│
├── backend/
│   ├── models.py          # Database models
│   ├── routes.py          # API routes
│   ├── auth.py            # Authentication logic
│   └── utils.py           # Helper functions
│
├── frontend/
│   ├── index.html         # Home page
│   ├── login.html         # Login page
│   ├── dashboard.html     # Admin dashboard
│   ├── booking.html       # Booking page
│   ├── css/
│   │   └── style.css      # Stylesheets
│   └── js/
│       └── script.js      # Client-side scripts
│
└── database/
    └── schema.sql         # Database schema
```

## 🗄️ Database Schema

### Core Tables

**Users Table**
```sql
users (user_id, name, email, phone, role, password_hash, created_at)
```

**Beds Table**
```sql
beds (bed_id, ward_id, bed_number, status, patient_id, created_at)
```

**Bookings Table**
```sql
bookings (booking_id, patient_id, bed_id, check_in, check_out, status, created_at)
```

**Wards Table**
```sql
wards (ward_id, ward_name, total_beds, available_beds, specialization)
```

## 🤝 Contributing

We welcome contributions to improve this project! 

### Steps to Contribute
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m 'Add YourFeature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a Pull Request

### Guidelines
- Follow PEP 8 for Python code
- Add comments for complex logic
- Test your changes before submitting
- Update documentation as needed

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📞 Support & Contact

For questions, issues, or suggestions:
- **GitHub Issues**: [Report an issue](https://github.com/Gokul-2004-cm/Bed_Slot_Booking-/issues)
- **Email**: gokul2004cm@example.com

---

<div align="center">

**Made with ❤️ to help healthcare systems during critical times**

![Python](https://img.shields.io/badge/Python-3.7+-blue?style=flat-square&logo=python)
![SQL](https://img.shields.io/badge/SQL-Database-green?style=flat-square&logo=database)
![HTML5](https://img.shields.io/badge/HTML5-Frontend-orange?style=flat-square&logo=html5)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

</div>
