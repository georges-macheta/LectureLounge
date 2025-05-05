# LectureLounge
🚀 Getting Started: Running LectureLounge Locally
Follow these steps to run the Flask + MongoDB app on your local machine.

📦 Requirements
Python 3.x

Git

MongoDB Atlas URI (or local MongoDB instance)

Node.js (if you want to run test.js)

🧰 Step-by-Step Setup
Clone the repository

bash
Copy
Edit
git clone https://github.com/yourusername/LectureLounge.git
cd LectureLounge
Set up a virtual environment

powershell
Copy
Edit
python -m venv venv
.\venv\Scripts\Activate   # (Use 'source venv/bin/activate' on Mac/Linux)
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
If there's no requirements.txt, run:

bash
Copy
Edit
pip install flask pymongo flask_sqlalchemy flask-login bcrypt
Configure MongoDB

In database.py, update:

python
Copy
Edit
self.CONNECTION_STRING = "your_mongo_connection_uri"
Ensure project structure is correct
Your files should be organized like this:

pgsql
Copy
Edit
LectureLounge/
├── app.py
├── database.py
├── test.js
├── README.md
├── venv/
├── website/
│   ├── __init__.py
│   ├── views.py
│   ├── auth.py
│   └── templates/
│       ├── home.html
│       ├── login.html
│       └── signup.html
Run the Flask app

powershell
Copy
Edit
$env:FLASK_APP = "app.py"    # On Windows
flask run
Visit: http://localhost:5000

