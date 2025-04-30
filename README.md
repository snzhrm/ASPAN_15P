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
