# complaint-registry
✅ Purpose
The goal is to streamline the process of registering and tracking complaints using a web portal accessible by both users and administrators.

✨ Features
User registration and login

Complaint submission with form fields

View submitted complaints

Admin panel (if included in your setup)

MongoDB integration

Responsive frontend (React)

🏗️ Architecture
Frontend:
Built with React.js

Components for login, signup, complaint form

Uses Axios for API communication

Backend:
Built with Node.js + Express.js

RESTful APIs

Connected to MongoDB Atlas/local MongoDB

Database:
MongoDB schema includes:

User model

Complaint model

Timestamps, user-complaint linking

⚙️ Setup Instructions
🔧 Prerequisites
Node.js (v14+)

MongoDB (local or Atlas)

Git

📥 Installation
Clone the repo:

bash
Copy code
git clone https://github.com/Niharika-code11/Online-complaint-register.git
cd Online-complaint-register
Install backend dependencies:

bash
Copy code
cd backend
npm install
Start MongoDB server (if local), then run backend:

bash
Copy code
npm start
Open a new terminal tab → Install frontend dependencies:

bash
Copy code
cd ../frontend
npm install
npm start
📁 Folder Structure
css
Copy code
Online-complaint-register/
│
├── backend/           → Express backend (API routes, DB config)
│   ├── models/        → Mongoose schemas
│   ├── routes/        → API endpoints
│   └── index.js       → Main server file
│
├── frontend/          → React app
│   ├── src/
│   │   ├── components/ → React components (Login, Signup, Form)
│   │   ├── pages/      → Routing pages
│   │   └── App.js      → Main app component
🚀 Running the Application
Frontend:
bash
Copy code
cd frontend
npm start
Backend:
bash
Copy code
cd backend
npm start
App will run at:

Frontend: http://localhost:3000

Backend: http://localhost:8000

🔗 API Documentation
You can list endpoints like this if needed:

POST /api/auth/signup
Registers a new user

Request body: { name, email, password }

POST /api/auth/login
Logs in a user

Returns: JWT token

POST /api/complaints
Submits a complaint

Requires: Auth token

🔐 Authentication
Uses JWT (JSON Web Token)

Token stored in localStorage

Protected routes require token in Authorization header

💻 User Interface
Login and Signup screens

Complaint submission form

Dashboard after login

✅ Testing
Manual testing through UI

API tested with Postman (optional)

📸 Screenshots / Demo
You can add screenshots like this:

🐛 Known Issues
No email verification on signup

Admin panel access not restricted yet (if applicable)

🔮 Future Enhancements
Add complaint categories and priorities

Email notifications

Role-based access (User vs Admin)

Pagination for complaint lists
