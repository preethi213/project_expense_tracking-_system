

# Expense Tracking System

## Project Overview
The **Expense Tracking System** is a web application designed to help users manage and track their daily expenses efficiently. The system allows users to input expenses, categorize them, and generate detailed reports for better financial management.

This project was developed using a combination of **Streamlit** for the frontend, **FastAPI** for the backend, and **MySQL** for data storage. The system is fully tested using **Pytest**, ensuring that all functionalities work as expected.

## Features
- **User-Friendly Interface**: Developed using Streamlit for a simple and interactive UI.
- **Expense Tracking**: Users can add, update, and delete expense records.
- **Categorization**: Expenses can be categorized (e.g., Food, Travel, Bills, etc.).
- **Expense Reports**: Detailed reports of total expenses within a selected date range.
- **Backend**: API-driven backend using FastAPI, handling requests efficiently.
- **Database**: MySQL database used to store user expenses.
- **Testing**: Comprehensive testing using Pytest for backend functionalities.
  
## Technologies Used
- **Frontend**: Streamlit (Python)
- **Backend**: FastAPI (Python)
- **Database**: MySQL
- **Testing**: Pytest
- **Languages**: Python, SQL

## Installation and Setup

### Prerequisites
- Python 3.8+
- MySQL server
- Pip (Python package manager)

### Step-by-Step Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/expense-tracking-system.git
   cd expense-tracking-system
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the MySQL database**:
   - Create a MySQL database named `expense_tracker`.
   - Import the `schema.sql` file to create necessary tables:
     ```sql
     mysql -u root -p expense_tracker < schema.sql
     ```

4. **Configure the database**:
   - Update the `config.py` file with your MySQL credentials:
     ```python
     MYSQL_HOST = 'localhost'
     MYSQL_USER = 'your_username'
     MYSQL_PASSWORD = 'your_password'
     MYSQL_DB = 'expense_tracker'
     ```

5. **Run the FastAPI backend**:
   ```bash
   uvicorn main:app --reload
   ```

6. **Run the Streamlit frontend**:
   ```bash
   streamlit run app.py
   ```

## Usage
1. Open the Streamlit web app in your browser:
   ```
   http://localhost:8501
   ```

2. Add, update, or delete your expense records through the interface.

3. View detailed reports on your expenses filtered by category and date.

## Testing
To run the tests, use Pytest:
```bash
pytest
```
This will run the backend tests and ensure that all API endpoints are functioning correctly.

## Future Enhancements
- User authentication for multiple users.
- Expense visualization using graphs.
- Integration with mobile apps for better accessibility.

## License
This project is licensed under the MIT License. See the (LICENSE) file for details.

