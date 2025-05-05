📚 LectureLounge
LectureLounge is a Flask + MongoDB web app that lets users post and explore category-based content. This guide walks you through setting it up locally.

🚀 Getting Started: Run Locally
✅ Requirements
Python 3.x

Git

MongoDB Atlas URI (or local MongoDB instance)

Node.js (optional, for test.js)

🧰 Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/LectureLounge.git
cd LectureLounge
2. Create a Virtual Environment
bash
Copy
Edit
python -m venv venv
- On Windows (PowerShell):
powershell
Copy
Edit
.\venv\Scripts\Activate
- On macOS/Linux:
bash
Copy
Edit
source venv/bin/activate
3. Install Dependencies
If you have a requirements.txt:

bash
Copy
Edit
pip install -r requirements.txt
Or install manually:

bash
Copy
Edit
pip install flask pymongo flask_sqlalchemy flask-login bcrypt
4. Configure MongoDB
In database.py, replace the placeholder with your actual MongoDB URI:

python
Copy
Edit
self.CONNECTION_STRING = "your_mongo_connection_uri"
