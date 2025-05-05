# Drone Food Delivery System

## Introduction
This project is a Flask-based web application for managing drone deliveries of food orders. Users can browse restaurants, place orders, and track drone deliveries in real-time via an interactive web interface.

## Problem Statement
Modern food delivery systems face challenges in speed, efficiency, and live tracking. Human-based delivery is often delayed, lacks transparency, and is hard to scale. Our project addresses this by automating the delivery process using drones, enabling faster, traceable, and contactless food delivery.

## Objectives
- Automate food delivery using drones
- Provide real-time tracking of orders
- Improve transparency and reduce delivery delays
- Allow restaurant and order management through a web interface
- Implement an admin dashboard for monitoring users and products

## Technology Stack
- **Frontend**: HTML, CSS, JavaScript, Leaflet.js
- **Backend**: Python, Flask
- **Database**: PostgreSQL
- **Authentication**: Flask-Login
- **Forms**: Flask-WTF
- **ORM**: Flask-SQLAlchemy
- **Maps**: Leaflet.js
- **Others**: python-dotenv, psycopg2

## Installation Instructions

1. Clone the repository
```bash
git clone https://github.com/snzhrm/ASPAN_15P.git
cd ASPAN_15P
```

2. Create and activate a virtual environment
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Unix or MacOS:
source venv/bin/activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Set up environment variables
Create a `.env` file in the root directory with the following content:
```
FLASK_APP=app
FLASK_ENV=development
SECRET_KEY=your-secret-key-here
SQLALCHEMY_DATABASE_URI=postgresql://username:password@localhost:5432/dbname
SQLALCHEMY_TRACK_MODIFICATIONS=False
```

5. Initialize the database
```bash
flask db init
flask db migrate -m "Initial migration"
flask db upgrade
python init_data.py
```

6. Run the application
```bash
python run.py
```

The application will be available at: http://localhost:5000

## Usage Guide

### For Users
1. Register or log in to your account
2. Browse available restaurants and their menus
3. Add items to your cart
4. Place an order with delivery coordinates
5. Track your order in real-time
6. Confirm delivery when the drone arrives

### For Administrators
1. Log in with admin credentials
2. Access the admin dashboard
3. Manage users, restaurants, and menu items
4. Monitor system statistics and order statuses

## Testing
To run the test suite:
```bash
python -m pytest tests/
```

## Known Issues / Limitations
- Mobile PWA version is not yet supported
- Weather API integration for drone safety is pending
- Currently uses simulated drone GPS data
- Limited to specific geographic area for drone operations

## References
- [Flask Documentation](https://flask.palletsprojects.com/)
- [Flask-Login Documentation](https://flask-login.readthedocs.io/)
- [Flask-SQLAlchemy Documentation](https://flask-sqlalchemy.palletsprojects.com/)
- [Leaflet.js Documentation](https://leafletjs.com/)
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)

## Team Members
- Muratkaliev Meyrambek (220103334) - 15P
- Assadbek Doskaliyev (220103079) - 18P
- Absattar Bereke (230103035) - 15P
- Sanzhar Zhaksykeldi (220103059) - 15P
