<img width="1122" height="1402" alt="image" src="https://github.com/user-attachments/assets/53ae86e2-af65-49c9-a786-19245d7b4a01" /># Expense Management System

A full-stack Expense Management System built using FastAPI, Streamlit, and MySQL for efficient expense tracking and financial analytics.

The application enables users to record daily expenses, manage transactions, and analyze spending patterns through category-wise and monthly expense reports.

---

## Overview

This project demonstrates the development of a complete expense management application consisting of:

- A FastAPI backend exposing REST APIs
- A Streamlit frontend for an interactive user interface
- A MySQL database for persistent storage
- Analytics modules for category-wise and monthly expense summaries

## Features

- Add and update daily expenses
- View expenses for a selected date
- Category-wise expense analytics
- Monthly expense summary
- RESTful APIs using FastAPI
- Interactive Streamlit dashboard
- MySQL database integration
- Dynamic data retrieval and updates
- Backend logging
- Unit testing using Pytest

## System Architecture


<p align="center">
  <img src="assets/system_architecture.png"
       alt="System Architecture"
       width="900">
</p>


---
## Technology Stack

| Category | Technology |
|----------|------------|
| Language | Python 3 |
| Backend | FastAPI |
| Frontend | Streamlit |
| Database | MySQL |
| Data Processing | Pandas |
| API Communication | Requests |
| Testing | Pytest |
| Logging | Python Logging |


## Project Structure

- **frontend/**: Contains the Streamlit application code.
- **backend/**: Contains the FastAPI backend server code.
- **tests/**: Contains the test cases for both frontend and backend.
- **requirements.txt**: Lists the required Python packages.
- **README.md**: Provides an overview and instructions for the project.

## REST API Endpoints

### Get Expenses

```
GET /expenses/{expense_date}
```

Returns all expenses for the specified date.

---

### Add or Update Expenses

```
POST /expenses/{expense_date}
```

Creates or updates expenses for the specified date.

---

### Expense Analytics

```
POST /analytics/
```

Returns category-wise expense totals and percentage distribution for a given date range.

---

### Monthly Summary

```
GET /monthly_summary/
```

Returns aggregated monthly expense statistics.

---

## Installation

### Clone the repository

```bash
git clone https://github.com/Joshitha12734/Expense-management-system.git

cd Expense-management-system
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Configure the database

Create the MySQL database using:

```
database/expense_db_creation.sql
```

Update the database credentials inside:

```
backend/db_helper.py
```

### Run the FastAPI backend

```bash
uvicorn backend.server:app --reload
```

The backend will start at:

```
http://127.0.0.1:8000
```

### Run the Streamlit frontend

```bash
streamlit run frontend/app.py
```


## Future Enhancements

- User authentication
- Expense deletion
- Budget planning and alerts
- Export reports to CSV and PDF
- Interactive visualizations using Plotly
- Docker support
- Cloud deployment
- Role-based access control
- Advanced filtering and search

---

## Learning Outcomes

This project demonstrates practical experience in:

- Full-stack Python application development
- REST API development using FastAPI
- CRUD operations with MySQL
- Frontend-backend integration
- Data aggregation and analytics
- Interactive dashboard development
- Software testing using Pytest
- Logging and exception handling
- Modular project architecture
