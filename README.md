# Bluestock IPO WebApp

A Django-based web application for managing and displaying IPO (Initial Public Offering) information, company details, and related documents via REST APIs and a basic frontend.

## 🔍 Project Overview

This web application allows users to:
- View IPO listings and associated company details
- Upload and view IPO documents
- Interact with a RESTful API
- Navigate a basic homepage rendered via Django templates

## 🛠️ Built With

- [Python 3.11](https://www.python.org/)
- [Django 5.2.3](https://www.djangoproject.com/)
- [Django REST Framework](https://www.django-rest-framework.org/)
- HTML (for templates)
- PostgreSQL (can also be configured for SQLite for development)

---

## 📁 Project Structure

bluestock-ipo-webapp/
│
├── ipo/ # Django app with models, views, serializers
│ ├── migrations/
│ ├── templates/ipo/ # Contains index.html
│ ├── admin.py
│ ├── apps.py
│ ├── models.py
│ ├── serializers.py
│ ├── urls.py
│ └── views.py
│
├── ipoproject/ # Django project settings
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
│
├── manage.py
├── requirements.txt
└── README.md

yaml
Copy
Edit

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/bluestock-ipo-webapp.git
cd bluestock-ipo-webapp
2. Set Up a Virtual Environment
bash
Copy
Edit
python -m venv venv
venv\Scripts\activate  # Windows
# source venv/bin/activate  # Linux/macOS
3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Run Migrations
bash
Copy
Edit
python manage.py makemigrations
python manage.py migrate
5. Start the Development Server
bash
Copy
Edit
python manage.py runserver
Then visit: http://127.0.0.1:8000/

📦 API Endpoints
Endpoint	Method	Description
/api/ipo/	GET	List all IPOs
/api/company/	GET	List all Companies
/api/document/	GET	List all Documents

