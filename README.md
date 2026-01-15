# Projet_Django - FinanceViz

## What is Django?

**Django** is a high-level Python web framework that encourages rapid development and clean, pragmatic design. Built by experienced developers, it takes care of much of the hassle of web development, so you can focus on writing your app without needing to reinvent the wheel. It's free and open source.

### Key Features of Django:
- **Fast**: Django was designed to help developers take applications from concept to completion as quickly as possible
- **Secure**: Django helps developers avoid many common security mistakes, such as SQL injection, cross-site scripting, cross-site request forgery and clickjacking
- **Scalable**: Django uses a component-based "shared-nothing" architecture, which makes it highly scalable
- **Versatile**: Django can be used to build almost any type of website — from content management systems and wikis, through to social networks and news sites
- **ORM (Object-Relational Mapping)**: Django provides a powerful ORM that allows you to interact with your database using Python code instead of SQL
- **Admin Interface**: Django comes with a built-in admin interface that makes it easy to manage your application's data

## About FinanceViz

**FinanceViz** is an interactive financial data visualization platform built with Django. This web application allows users to visualize and analyze their financial data in a simple and effective manner.

### Features

- **Data Upload**: Import your financial data directly or upload CSV files
- **Multiple Visualization Types**: Create line charts, bar charts, and pie charts
- **Data Filtering**: Filter your data by specific columns and values
- **Interactive Tables**: View your data in clean, formatted HTML tables
- **PDF Export**: Download your visualizations and data tables as PDF documents
- **User-Friendly Interface**: Simple and intuitive web interface built with Django templates

### Technology Stack

- **Backend**: Django 5.1.4
- **Frontend**: HTML templates with Bootstrap styling
- **Data Processing**: Pandas for data manipulation
- **Visualization**: Matplotlib and Seaborn for chart generation
- **PDF Generation**: ReportLab for creating downloadable reports
- **Database**: SQLite (default)

## Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/zounoogo/Projet_Django.git
cd Projet_Django
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required dependencies:
```bash
pip install django pandas matplotlib seaborn reportlab
```

4. Navigate to the project directory:
```bash
cd FinaceViz
```

5. Apply database migrations:
```bash
python manage.py migrate
```

6. Run the development server:
```bash
python manage.py runserver
```

7. Open your browser and visit: `http://127.0.0.1:8000/`

## Usage

### Home Page
Visit the home page to get started with FinanceViz. You'll see options to:
- Upload data directly
- Import data from a CSV file

### Direct Data Upload
1. Navigate to "Télécharger directement vos données"
2. Enter your data in JSON format
3. Select your chart type (line, bar, or pie)
4. Apply filters if needed
5. View your generated visualization and data table

### CSV File Upload
1. Navigate to "Entrer un fichier csv_file"
2. Upload a CSV file containing your financial data
3. Ensure your CSV has a "Date" column
4. Select your chart type
5. Apply filters if desired
6. View or download your visualization as PDF

### About & Contact
- Visit the **About** page to learn more about the project
- Use the **Contact** page to get in touch

## Project Structure

```
FinaceViz/
├── FinaceViz/           # Main project configuration
│   ├── settings.py      # Django settings
│   ├── urls.py          # Main URL configuration
│   └── wsgi.py          # WSGI configuration
├── visualization/       # Main application
│   ├── views.py         # View logic
│   ├── urls.py          # App URL patterns
│   ├── models.py        # Database models
│   ├── forms.py         # Form definitions
│   └── templates/       # HTML templates
├── manage.py            # Django management script
└── db.sqlite3          # SQLite database
```

## Contributing

This is a personal project developed as part of learning Django web development. Contributions, issues, and feature requests are welcome!

## License

This project is open source and available for educational purposes.

## Author

Developed as a Django learning project to demonstrate financial data visualization capabilities.
