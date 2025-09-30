# Basic-User-Management-Web-Application-using-ExpressJs
This is a full-stack User Management system built with Node.js, Express, MongoDB, EJS, and Bootstrap 5. It supports user registration, login/logout with sessions, and CRUD operations for user profiles. The UI is fully responsive and styled with Bootstrap.

Features
User Registration with proper input validation
Secure Login/Logout implemented using sessions
CRUD Operations for managing user profiles (username, email, age)
Protected Routes secured with custom middleware
Responsive UI designed with Bootstrap 5

Project Structure (MVC)
The project follows the Model-View-Controller (MVC) pattern for clean separation of concerns:

Model – Defines the structure of the user data using Mongoose (userModel.js).
View – EJS templates render dynamic HTML pages (login.ejs, home.ejs, etc.).
Controller – Handles logic and interactions between model and view (controller.js).

UserManagementApp/
│
├── app.js                     # Main app entry point
├── package.json               # Project metadata and dependencies
├── README.md                  # Project documentation
│
├── config/
│   └── db.js                  # MongoDB connection setup
│
├── controller/
│   └── controller.js          # Handles user registration, login, CRUD logic
│
├── middleware/
│   └── auth.js                # Route protection middleware
│
├── model/
│   └── userModel.js           # Mongoose schema for users
│
├── routes/
│   └── routing.js             # All Express routes
│
└── views/                     # EJS templates (UI)
    ├── login.ejs              # Login form
    ├── register.ejs           # Register form
    ├── home.ejs               # Dashboard with user table
    └── editUser.ejs           # Edit user form
    
Modules Used

1. Express
Used to create the backend server and define application routes. It handles HTTP requests and connects controllers to views.

2. Mongoose
Acts as an Object Data Modeling (ODM) library for MongoDB. It defines schemas and performs database operations.

3. EJS (Embedded JavaScript)
Templating engine to dynamically render HTML pages using server-side data like usernames, errors, and profile info.

4. express-session
Manages user sessions securely. It stores session data on the server and authenticates access to protected pages.

5. bcrypt
Used to hash user passwords during registration and validate them during login to ensure secure authentication.

6. Bootstrap 5
Provides a responsive, mobile-friendly, and visually appealing front-end interface with styled forms, tables, and alerts.

How to Run

Clone the repository:
git clone https://github.com/your-username/user-management-app.git
cd user-management-app

Install dependencies:
npm install
Set up MongoDB (local or Atlas), and configure your MongoDB URI in config/db.js.

Run the server:
node app.js

Open in browser:
http://localhost:3000

<img width="1762" height="527" alt="Screenshot 2025-09-30 124433" src="https://github.com/user-attachments/assets/cce13237-425e-4a05-a3a8-62917031b969" />
<img width="1037" height="557" alt="Screenshot 2025-09-30 124419" src="https://github.com/user-attachments/assets/37cd1101-9d57-4357-ac2c-515ed5cfc9b4" />
<img width="1092" height="593" alt="Screenshot 2025-09-30 124310" src="https://github.com/user-attachments/assets/8d0dc030-7c0b-458c-83dd-ba3c2c6655a8" />
