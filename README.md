# ALX Travel App

A Django-based travel application that helps users discover and book travel experiences.

## Features

- User authentication and authorization
- Property listings with detailed information
- Booking management system
- Review and rating system
- Search and filtering capabilities
- Admin dashboard for property management

## Tech Stack

- Python 3.8+
- Django 4.2+
- Django REST Framework
- PostgreSQL
- Bootstrap 5
- Font Awesome

## Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- PostgreSQL database
- Virtual environment (recommended)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/alx_travel_app.git
cd alx_travel_app
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
Create a `.env` file in the project root with the following variables:
```
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=postgresql://user:password@localhost:5432/alx_travel_app
```

5. Run migrations:
```bash
python manage.py migrate
```

6. Create a superuser:
```bash
python manage.py createsuperuser
```

7. Seed the database (optional):
```bash
python manage.py seed
```

8. Run the development server:
```bash
python manage.py runserver
```

The application will be available at `http://localhost:8000`

## Project Structure

```
alx_travel_app/
├── alx_travel_app/          # Project settings
├── listings/               # Main app for property listings
│   ├── models.py          # Database models
│   ├── serializers.py     # API serializers
│   ├── views.py           # View logic
│   └── urls.py            # URL routing
├── bookings/              # Booking management
├── reviews/               # Review system
├── users/                 # User management
└── templates/             # HTML templates
```

## API Endpoints

- `/api/auth/` - Authentication endpoints
- `/api/listings/` - Property listing endpoints
- `/api/bookings/` - Booking management endpoints
- `/api/reviews/` - Review system endpoints

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- ALX Software Engineering Program
- Django Documentation
- Django REST Framework Documentation 