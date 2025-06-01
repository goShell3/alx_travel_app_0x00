# ALX Travel App

A Django-based travel application that helps users discover and book travel experiences. This project is part of the ALX Software Engineering Program.

## 🚀 Features

- **User Management**
  - Secure authentication and authorization
  - User profiles with customizable settings
  - Role-based access control (Hosts and Guests)

- **Property Listings**
  - Detailed property information
  - High-quality image galleries
  - Amenities and facilities listing
  - Location-based search
  - Price filtering and sorting

- **Booking System**
  - Real-time availability checking
  - Secure payment processing
  - Booking management dashboard
  - Email notifications
  - Booking history

- **Review System**
  - User ratings and reviews
  - Host responses
  - Review moderation
  - Rating analytics

- **Search & Discovery**
  - Advanced search filters
  - Location-based recommendations
  - Popular destinations
  - Recently viewed properties

## 🛠️ Tech Stack

- **Backend**
  - Python 3.8+
  - Django 4.2+
  - Django REST Framework
  - PostgreSQL
  - Celery (for async tasks)

- **Frontend**
  - Bootstrap 5
  - Font Awesome
  - JavaScript/jQuery
  - AJAX for dynamic content

- **Development Tools**
  - Git for version control
  - Docker for containerization
  - pytest for testing
  - Black for code formatting

## 📋 Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- PostgreSQL database
- Virtual environment (recommended)
- Git

## 🚀 Installation

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/alx_travel_app.git
cd alx_travel_app
```

2. **Create and activate a virtual environment:**
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Set up environment variables:**
Create a `.env` file in the project root:
```env
DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=postgresql://user:password@localhost:5432/alx_travel_app
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_HOST_USER=your-email@gmail.com
EMAIL_HOST_PASSWORD=your-app-password
```

5. **Database setup:**
```bash
python manage.py migrate
python manage.py createsuperuser
python manage.py seed  # Optional: Seed the database with sample data
```

6. **Run the development server:**
```bash
python manage.py runserver
```

The application will be available at `http://localhost:8000`

## 📁 Project Structure

```
alx_travel_app/
├── alx_travel_app/          # Project settings
│   ├── settings.py         # Project configuration
│   ├── urls.py            # Main URL routing
│   └── wsgi.py            # WSGI configuration
├── listings/               # Property listings app
│   ├── models.py          # Database models
│   ├── serializers.py     # API serializers
│   ├── views.py           # View logic
│   ├── urls.py            # URL routing
│   └── tests/             # Test cases
├── bookings/              # Booking management
├── reviews/               # Review system
├── users/                 # User management
├── templates/             # HTML templates
├── static/               # Static files
└── media/                # User-uploaded files
```

## 🔌 API Endpoints

### Authentication
- `POST /api/auth/register/` - User registration
- `POST /api/auth/login/` - User login
- `POST /api/auth/logout/` - User logout

### Listings
- `GET /api/listings/` - List all properties
- `POST /api/listings/` - Create new listing
- `GET /api/listings/{id}/` - Get listing details
- `PUT /api/listings/{id}/` - Update listing
- `DELETE /api/listings/{id}/` - Delete listing

### Bookings
- `GET /api/bookings/` - List all bookings
- `POST /api/bookings/` - Create new booking
- `GET /api/bookings/{id}/` - Get booking details
- `PUT /api/bookings/{id}/` - Update booking status

### Reviews
- `GET /api/reviews/` - List all reviews
- `POST /api/reviews/` - Create new review
- `GET /api/reviews/{id}/` - Get review details

## 🧪 Testing

Run the test suite:
```bash
python manage.py test
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Code Style

- Follow PEP 8 guidelines
- Use meaningful variable and function names
- Write docstrings for all functions and classes
- Keep functions small and focused
- Write unit tests for new features

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- ALX Software Engineering Program
- Django Documentation
- Django REST Framework Documentation
- Bootstrap Documentation
- Font Awesome

## 📞 Support

For support, email support@alxtravelapp.com or create an issue in the repository. 