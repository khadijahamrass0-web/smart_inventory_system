# Inventory Management System

A comprehensive Django-based web application for managing customer orders, products, and inventory. This project combines data analysis, database management, and a web interface for seamless inventory operations.

## 📋 Table of Contents
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies](#technologies)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Team Members](#team-members)

## ✨ Features

- **Customer Management**: Register and manage customer information
- **Product Management**: Create, update, and delete products with easy deletion confirmation
- **Order Processing**: Place orders and manage order items
- **Order History**: Track customer order history with detailed information
- **Data Analysis**: Jupyter notebook for data exploration and analysis
- **Database Management**: Smart inventory tracking with SQL database
- **Data Import/Export**: CSV file support for bulk data operations

## 📁 Project Structure

```
PythonProject12/
├── webapp/                          # Django web application
│   ├── manage.py                   # Django management script
│   ├── inventory/                  # Main Django app
│   │   ├── models.py              # Database models
│   │   ├── views.py               # View logic
│   │   ├── forms.py               # Form definitions
│   │   ├── urls.py                # URL routing
│   │   ├── admin.py               # Admin configuration
│   │   ├── templates/             # HTML templates
│   │   │   └── inventory/
│   │   │       ├── base.html                      # Base template
│   │   │       ├── customer_register.html         # Customer registration
│   │   │       ├── product_form.html              # Product creation
│   │   │       ├── product_list.html              # Product listing
│   │   │       ├── order_form.html                # Order placement
│   │   │       ├── order_history.html             # Order history
│   │   │       └── product_confirm_delete.html    # Delete confirmation
│   │   ├── migrations/             # Database migrations
│   │   └── tests.py               # Unit tests
│   └── webapp/                      # Django settings
│       ├── settings.py             # Project settings
│       ├── urls.py                 # Main URL configuration
│       ├── asgi.py                 # ASGI configuration
│       └── wsgi.py                 # WSGI configuration
├── core/                            # Core utilities
│   └── part1.py                    # Core functionality
├── databse/                         # Database scripts
│   ├── part2.py                    # Database operations
│   └── smart_inv.sql               # Database schema
├── analysis.ipynb                   # Data analysis notebook
├── export_data (1).py              # Data export utility
├── customers.csv                    # Customer data
├── orders.csv                       # Order data
├── order_items.csv                 # Order items data
├── products.csv                     # Product data
└── README.md                        # Project documentation
```

## 🛠 Technologies

- **Python 3.x** - Backend language
- **Django** - Web framework
- **SQL** - Database management
- **HTML/CSS** - Frontend templates
- **Jupyter Notebook** - Data analysis
- **CSV** - Data storage format

## 🚀 Setup Instructions

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Installation

1. **Clone or navigate to the project directory**
   ```bash
   cd PythonProject12/webapp
   ```

2. **Install dependencies** (if requirements.txt exists)
   ```bash
   pip install -r requirements.txt
   # or manually:
   pip install django
   ```

3. **Apply database migrations**
   ```bash
   python manage.py migrate
   ```

4. **Create a superuser account** (for admin access)
   ```bash
   python manage.py createsuperuser
   ```

5. **Load initial data** (if using CSV files)
   ```bash
   python manage.py shell
   # Then use the import utilities in core/part1.py
   ```

### Running the Application

```bash
# Start the development server
python manage.py runserver

# The application will be available at http://127.0.0.1:8000/
```

### Accessing the Admin Panel

```
URL: http://127.0.0.1:8000/admin/
Username: (superuser username)
Password: (superuser password)
```

## 📊 Usage

### Customer Registration
1. Navigate to the customer registration page
2. Fill in customer details
3. Submit to register a new customer

### Product Management
1. Access the product list to view all products
2. Click "Add Product" to create a new product
3. Edit or delete existing products as needed

### Placing Orders
1. Go to the order form
2. Select customer and products
3. Specify quantities and submit
4. View order history to track past orders

### Data Analysis
- Open `analysis.ipynb` in Jupyter Notebook for data exploration and analytics
- Run queries on order and customer data

## 👥 Team Members

- **AHMED MOFADEL**
- **KHADIJA HAMRAS**

---

**Last Updated**: February 2026
