 Django E-commerce API

A simple RESTful backend API built with Django and Django REST Framework to manage products and categories.

## Features

- CRUD operations for Products and Categories
- Search and ordering on Products
- JWT authentication for secure access
- Admin panel for easy management
- Simple and extensible codebase

## Getting Started

### Prerequisites

- Python 3.9+
- pip (Python package installer)

### Installation
1. Clone the repository:
        ```bash
       git clone (https://github.com/SadatLearning121/Django-e-commerce-API)
      cd django-ecommerce-api
   
2.   Create and activate a virtual environment (optional but recommended):
    ```bash

      python -m venv venv
      source venv/bin/activate

3.Install dependencies:

pip install -r requirements.txt

4.Apply migrations:
    ```bash
    python manage.py runserver

5.Create a superuser to access the admin: 
      ```bash
    python manage.py createsuperuser

6. Run the development server:
       ```bash
    python manage.py runserver

7.Open your browser and visit:
API root: http://127.0.0.1:8000/api/products/
Admin panel: http://127.0.0.1:8000/admin/

API Endpoints:
/api/products/ — List, create, update, delete products

/api/categories/ — List, create, update, delete categories

/api/token/ — Obtain JWT token (POST username & password)

/api/token/refresh/ — Refresh JWT token

Authentication
Uses JWT tokens for secure API access

Read-only access for unauthenticated users

Full access (create/update/delete) for authenticated users

How to use JWT:
1.Obtain token:
POST /api/token/
{
  "username": "<your-username>",
  "password": "<your-password>"
}

2.Use the access token in Authorization header:
Authorization: Bearer <access_token>

3.Refresh token when expired by posting refresh token to /api/token/refresh/.

Made with ❤️ by SadatLearning121

---


    

    
