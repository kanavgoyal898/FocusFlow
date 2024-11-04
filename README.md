# FocusFlow

FocusFlow is a user-friendly task management application developed using Flask, a popular web framework for Python, combined with SQLAlchemy, an ORM (Object-Relational Mapping) library that simplifies database interactions. The application is designed to help users efficiently manage their tasks, enabling them to focus on their priorities without the hassle of complex interfaces.

<div style="text-align: center;">
  <img src="./demo.png" alt="Preview" style="width: 100%;">
</div>

## Features

- **Add Tasks:** Easily create new tasks.
- **View Tasks:** See all tasks listed with their creation dates.
- **Update Tasks:** Modify existing tasks.
- **Delete Tasks:** Remove tasks that are no longer needed.

## Technologies Used

- **Flask:** A lightweight WSGI web application framework for Python.
- **Flask-SQLAlchemy:** A SQL toolkit for Flask that simplifies database operations.
- **SQLite:** A lightweight database for storing tasks.
- **Bootstrap:** A front-end framework for developing responsive web pages.

## Installation

### Prerequisites

- Python 3.6+
- pip (Python package installer)

### Clone the Repository

```bash
git clone https://github.com/kanavgoyal898/FocusFlow.git
cd FocusFlow
```

### Set Up a Virtual Environment (Optional)

```bash
python -m venv venv
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Initialize the Database

Before running the application, create the database by executing:

```bash
from app import app, db
with app.app_context():
    db.create_all()
```

## Usage

### Run the Application

```bash
python app.py
```

The application will run on `http://127.0.0.1:5000/` by default. Open this URL in your web browser to access FocusFlow.

## File Structure

```
FocusFlow/
│
├── app.py 
├── init.py 
├── templates/
│   ├── base.html
│   ├── index.html 
│   └── update.html
└── static/ 
    └── css/
        └── base.css
```

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.