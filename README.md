# Drone Delivery System

A Flask-based web application for managing drone deliveries of food orders. This system allows users to browse restaurants, place orders, and track drone deliveries in real-time.

## Features

- User authentication (login/register)
- Restaurant browsing and menu viewing
- Shopping cart functionality
- Order placement and tracking
- Real-time drone position tracking
- Admin panel for managing users and products
- Responsive web interface

## Tech Stack

- **Backend**: Python, Flask
- **Database**: SQLite (can be configured for PostgreSQL)
- **Frontend**: HTML, CSS, JavaScript
- **Authentication**: Flask-Login
- **Forms**: Flask-WTF
- **Database ORM**: Flask-SQLAlchemy
- **Maps**: Folium
- **Environment Management**: python-dotenv

## Installation

1. Clone the repository:
```bash
git clone https://github.com/snzhrm/ASPAN/blob/main/pythonDronProject%20(2).zip
cd drone-delivery
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

4. Create a `.env` file in the project root with the following content:
```
SECRET_KEY=your-secret-key-here
SQLALCHEMY_DATABASE_URI=sqlite:///app.db
```

5. Initialize the database:
```bash
python init_db.py
```

6. Run the application:
```bash
python run.py
```

The application will be available at `http://localhost:5000`

## Project Structure

```
drone-delivery/
├── app/
│   ├── static/          # Static files (CSS, JS, images)
│   ├── templates/       # HTML templates
│   ├── __init__.py     # Application factory
│   ├── models.py       # Database models
│   ├── routes.py       # Application routes
│   └── forms.py        # Form definitions
├── .env                # Environment variables
├── init_db.py         # Database initialization script
├── requirements.txt   # Project dependencies
└── run.py            # Application entry point
```

## Features in Detail

### User Management
- User registration and login
- Password hashing and security
- User profiles and order history

### Restaurant System
- Browse multiple restaurants
- View detailed menus
- Add items to cart
- Place orders with delivery coordinates

### Drone Tracking
- Real-time drone position updates
- ETA calculations
- Weather conditions monitoring
- Battery level tracking

### Admin Features
- User management
- Product management
- Order monitoring
- System statistics

