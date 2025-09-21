# Assignment3gw8525

The prject helps connect Rect (Vite) to a ode and Express backend to connect to MySql database. it will be able to display results from ten select quies each joinin at least 2 tables using at least 2 conditions. 
##Project Structure
reactmysql/
├─ backend/
│  ├─ server.js
│  └─ package.json
├─ frontend/frontend
│  ├─ index.html
│  └─ src/
│     ├─ main.jsx
│     └─ App.jsx
└─ sql.txt             

Prerequistites
-Node,js LTS
-MySQL
-phpMYAdmin
Database Used
-students (id PK, name, birthday, gpa, dept_id)
-departments (id PK, name)
-courses (crscode PK, title, dept_id, credits)
-instructors (id PK, name, dept_id)
-transcript (studentid FK, crscode FK, semester, grade)
-teaches (instructorid FK, crscode FK, semester)

Backend
cd backend
npm install
npm start
OPEN: http://localhost:8081/listall and http://localhost:8081/q1 in the browser to show JSON.

Install and Run
cd ./backend
npm install
npm start

Front end (Vite + React)
cd frontend/frontend
npm install
npm run dev
OPEN: http://localhost:5173
The React app fetches http://localhost:8081 endpoints and displays JSON for /listall and /q1…/q10.

Troubleshooting 

DB connection error in server.js verifying: 
host: "localhost",
port: 3306,
user: "root",
password: "",   // or your password
database: "test"

Foreign key: Heps to ensure that student.id and courses.crscode are defined as Primary Key before creating transcript/teaches


