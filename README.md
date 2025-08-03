🗂️ Tracker101
Tracker101 is a full-stack productivity application that combines the flexibility of a to-do list with the personalization of a digital diary. It features a Django-powered API backend and a React frontend, allowing users to create, manage, and track their daily tasks or personal reflections in one place.

🔧 Tech Stack
Layer	Tech
Backend	Django, Django REST Framework
Frontend	React.js, Axios
Database	SQLite (default), PostgreSQL-ready
API Format	REST (JSON)
Auth	Token-based (DRF tokens or JWT)
Styling	CSS/Bootstrap/Material UI (customizable)

🚀 Features
✅ User registration and login

✅ Task creation, update, and deletion

✅ Personal diary entries with timestamps

✅ Task tagging and status tracking (e.g., Done, In Progress)

✅ Calendar integration for visual task organization (optional)

✅ Token-based API authentication

✅ Responsive React frontend

✅ RESTful API for mobile or third-party integration

📂 Folder Structure
bash
Copy
Edit
tracker101/
├── backend/              # Django project root
│   ├── api/              # DRF API app
│   ├── users/            # Auth module
│   └── settings.py       # Django settings
│
├── frontend/             # React project
│   ├── src/
│   │   ├── components/
│   │   └── App.js
│   └── package.json
│
└── README.md
🛠️ Getting Started
🔹 Backend (Django)
bash
Copy
Edit
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
🔹 Frontend (React)
bash
Copy
Edit
cd frontend
npm install
npm start
🔐 API Authentication
By default, the API uses token-based auth.

You can generate a token via the login endpoint:

http
Copy
Edit
POST /api/token/
Include the token in request headers:

makefile
Copy
Edit
Authorization: Token <your_token>
📬 Sample API Endpoints
Method	Endpoint	Description
GET	/api/tasks/	List all tasks
POST	/api/tasks/	Create a new task
GET	/api/diary/	Fetch diary entries
POST	/api/diary/	Add a new diary entry
POST	/api/token/	Get auth token

📈 Planned Features (Next Releases)
🔁 Task reminders with email notifications

🧠 AI-based mood detection from diary text

📊 Task completion analytics dashboard

☁️ Cloud deployment (Render / Vercel / Railway)

🧪 Testing
bash
Copy
Edit
python manage.py test
