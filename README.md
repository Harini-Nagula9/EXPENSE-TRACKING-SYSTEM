![WhatsApp Image 2025-06-16 at 13 11 56_5bbeb4ec](https://github.com/user-attachments/assets/0b97f383-9a16-436b-9012-569a056ce470)

# Expense Tracking System

## Overview
The **Expense Tracking System** is a web-based application designed to help users manage their expenses efficiently. It features **FastAPI for backend**, **MySQL for data storage**, **Streamlit for frontend visualization**, and **Postman for API testing**.

## Project Structure
 Expense-Tracking-System ┣ 📂 backend      # FastAPI-based backend ┣ 📂 frontend     # Streamlit-based frontend ┣ 📂 tests        # API testing setup ┣ 📜 README.md    # Project documentation ┣ 📜 requirements.txt # Dependencies

---

## Tech Stack
- **Backend:** FastAPI (Python)
- **Database:** MySQL
- **Frontend:** Streamlit
- **Testing:** Postman

---

##  Setup & Installation

### **Backend (FastAPI)**
1. Install dependencies:
    ```bash
    pip install fastapi uvicorn pymysql
    ```
2. Run the server:
    ```bash
    cd backend
    uvicorn main:app --reload
    ```
3. Access API docs: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

### **Frontend (Streamlit)**
1. Install Streamlit:
    ```bash
    pip install streamlit
    ```
2. Run the app:
    ```bash
    cd frontend
    streamlit run app.py
    ```

### **Database (MySQL)**
1. Install MySQL and create the database:
    ```sql
    CREATE DATABASE expense_tracker;
    ```
2. Import the schema from `backend/db_config.py`.

---

## 🔌 API Endpoints
### **Expense Operations**
```bash
GET /expenses         # Retrieve all expenses
POST /expenses        # Add a new expense
PUT /expenses/{id}    # Update an expense
DELETE /expenses/{id} # Remove an expense


Analytics
GET /expenses/category-breakdown
GET /expenses/monthly-summary


##Monthly Summary Response Example
{
    "August": 5172.00,
    "September": 4790.00
}



## Expense Analytics in Streamlit
Category Breakdown
- Visualizes expenses per category using bar charts and tables.
- Data dynamically updates based on user input.
Monthly Expense Comparison
- Displays monthly spending trends with comparative insights.
- Users can analyze habits and adjust spending accordingly.






