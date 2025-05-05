Installation Guide

1. Clone the Repository
   git clone https://github.com/snzhrm/ASPAN_15P.git
   cd ASPAN_15P
2. Create and Activate Virtual Environment
   python -m venv venv
   # Windows:
   venv\Scripts\activate
   # Mac/Linux:
   source venv/bin/activate
3. Install Dependencies
   pip install -r requirements.txt
4. Setup Environment Variables

Create a .env file in the root folder:
   FLASK_APP=app
   FLASK_ENV=development
   SECRET_KEY=your-secret-key-here
   SQLALCHEMY_DATABASE_URI=postgresql://username:password@localhost:5432/dbname

6. Run the Application
   python run.py
Visit http://localhost:5000
