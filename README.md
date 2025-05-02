# ASPAN_15P

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
• **Frontend:** HTML, CSS, JavaScript  
• **Backend:** Python, Flask  
• **Database:** SQLite (can be configured for PostgreSQL)  
• **Authentication:** Flask-Login  
• **Forms:** Flask-WTF  
• **ORM:** Flask-SQLAlchemy  
• **Maps:** Folium  
• **Others:** python-dotenv  

## Installation Instructions  
### 1. Clone the repository  
```bash  
git clone https://github.com/snzhrm/ASPAN_15P.git  
```

### 2. Navigate into the project directory  
```bash  
cd ASPAN  
```

### 3. Create and activate a virtual environment  
```bash  
python -m venv venv  
source venv/bin/activate  # On Windows: venv\Scripts\activate  
```

### 4. Install dependencies  
```bash  
pip install -r requirements.txt  
```

### 5. Set environment variables  
Change a `.env` file in the root directory and add:  
```env  
SECRET_KEY=your-secret-key-here  
SQLALCHEMY_DATABASE_URI=sqlite:///app.db  
```

### 6. Initialize the database  
```bash  
python init_db.py  
```

### 7. Run the application  
```bash  
python run.py  
```

The application will be available at: [http://localhost:5000](http://localhost:5000)

## Usage Guide  
- Register or log in as a user  
- Browse available restaurants and their menus  
- Add items to cart and place orders with delivery coordinates  
- View real-time drone location and delivery status  
- Admins can manage users, products, and view system stats  


## Known Issues / Limitations (Optional)  
- No support for mobile PWA version yet  
- Weather API not yet fully integrated for drone safety  
- Currently uses mock drone GPS data  

## References  
- Flask documentation  
- Flask-Login and Flask-WTF tutorials  
- Folium for map rendering  
- SQLite official documentation  

## Team Members  
220103334 Muratkaliev Meyrambek 15P
220103079 Assadbek Doskaliyev 18P
230103035 Absattar Bereke 15P
220103059 Sanzhar Zhaksykeldi 15P
