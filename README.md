# LectureLounge

LectureLounge is a Flask + MongoDB web app that lets users post and explore category-based content. This guide walks you through setting it up locally.

## 🚀 Getting Started

### ✅ Requirements

- Python 3.x  
- Git  
- MongoDB Atlas URI (or local MongoDB instance)

---

## 🧰 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/LectureLounge.git
cd LectureLounge
### 2. Create a Virtual Environment
bash
Copy
Edit
python -m venv venv
On Windows (PowerShell):
powershell
Copy
Edit
.\venv\Scripts\Activate
On macOS/Linux:
bash
Copy
Edit
source venv/bin/activate
### 3. Install Dependencies
If you have a requirements.txt file:

bash
Copy
Edit
pip install -r requirements.txt
Or manually install:

bash
Copy
Edit
pip install flask pymongo flask_sqlalchemy flask-login bcrypt
4. Configure MongoDB
In database.py, update the connection string:

python
Copy
Edit
self.CONNECTION_STRING = "your_mongo_connection_uri"
5. Run the App
On Windows (PowerShell):
powershell
Copy
Edit
$env:FLASK_APP = "app.py"
flask run
On macOS/Linux:
bash
Copy
Edit
export FLASK_APP=app.py
flask run
Then open your browser and visit: http://localhost:5000
