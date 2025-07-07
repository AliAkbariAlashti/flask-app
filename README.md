Simple Flask Web App
This is a simple web application built with Flask and Bootstrap 5. It includes a home page and a contact form, designed to be responsive and accessible on both mobile and desktop devices.
Features

Home page with a welcome message
Contact form with flash messages
Responsive design using Bootstrap 5
Deployable on Render

Setup

Clone the repository:
git clone https://github.com/AliAkbariAlashti/flask-app.git
cd flask-app


Create a virtual environment and install dependencies:
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt


Run the app locally:
python app.py


Access the app at http://localhost:5000.


Deployment
To deploy on Render:

Create a new Web Service on Render and connect your GitHub repository.
Set the following configurations:
Environment: Python
Build Command: pip install -r requirements.txt
Start Command: gunicorn --bind :8080 --workers 2 app:app


Deploy the app and get the public URL.

Notes

Ensure you change the SECRET_KEY in app.py to a secure value before deployment.
The app uses Bootstrap 5 via CDN, which may require a VPN in some regions due to filtering.
