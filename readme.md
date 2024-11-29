Django E-Commerce Project
This project demonstrates a simple e-commerce system using Django, featuring Customer and Order models with a relational structure. It is designed as a starting point for creating and managing customer orders in an online store.

Project Structure
    cusmodel/
    manage.py
    myproject/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
    qn1/
        __init__.py
        admin.py
        apps.py
        migrations/
        models.py
        tests.py
        views.py
Features
Models:

Customer: Stores customer information such as name and email.
Order: Manages customer orders with fields for order date and total amount.
Relationships:
Each Customer can have multiple Order records.
Each Order is associated with a single Customer.
Admin Panel: Includes registration of models for management through Django’s admin interface.

Setup Instructions
1. Prerequisites
Python 3.9+ installed.
Virtual environment support.
Basic understanding of Django.
2. Installation and Setup
Step 1: Clone the Repository
git clone <https://github.com/collozz/APICAT2Q1.git>
cd qn1
Step 2: Set Up a Virtual Environment

python -m venv venv
source venv/bin/activate    # On Linux/Mac
venv\Scripts\activate       # On Windows

Step 3: Install Dependencies

pip install django
Step 4: Run Migrations

python manage.py makemigrations
python manage.py migrate
Step 5: Start the Development Server

python manage.py runserver
Step 6: Access the Application
Open your browser and go to http://127.0.0.1:8000.

Using the Application
Admin Panel
Create a superuser to access the admin panel:

python manage.py createsuperuser
Navigate to http://127.0.0.1:8000/admin and log in.
Manage Customer and Order data through the admin interface.
Customization
Adding Views: Define custom views in ecommerce/views.py.
Routing: Add URL patterns in ecommerce/urls.py and include them in the project’s main urls.py.
Version Control
Initialize Git (if not already initialized):


git init
git add .
git commit -m "Initial project setup with Customer and Order models"
Push the code to GitHub:


git remote add origin <https://github.com/collozz/APICAT2Q1.git>
git branch -M main
git push -u origin main
