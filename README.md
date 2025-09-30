# Basic-User-Management-Web-Application-using-ExpressJs
This is a full-stack User Management system built with Node.js, Express, MongoDB, EJS, and Bootstrap 5. It supports user registration, login/logout with sessions, and CRUD operations for user profiles. The UI is fully responsive and styled with Bootstrap.


## 🚀 Features
- **User Registration** with input validation  
- **Secure Login/Logout** using sessions  
- **CRUD Operations** (Create, Read, Update, Delete) for user profiles  
- **Protected Routes** with custom middleware  
- **Responsive UI** using Bootstrap 5  

## 🛠️ Tech Stack
- **Backend:** Node.js, Express.js  
- **Frontend:** EJS, HTML, CSS, Bootstrap 5  
- **Database:** MongoDB, Mongoose  
- **Authentication:** Express-session, Middleware  

## 🧩 Project Structure (MVC)

The project follows the **Model-View-Controller (MVC)** pattern for a clean separation of concerns:

- **Model** – Defines the structure of user data using Mongoose (`userModel.js`).  
- **View** – EJS templates render dynamic HTML pages (`login.ejs`, `register.ejs`, `home.ejs`, `editUser.ejs`).  
- **Controller** – Handles application logic and manages interactions between Model and View (`controller.js`).  

UserManagementApp/
│
├── app.js # Main app entry point
├── package.json # Project metadata and dependencies
├── README.md # Project documentation
│
├── config/
│ └── db.js # MongoDB connection setup
│
├── controller/
│ └── controller.js # Handles user registration, login, CRUD logic
│
├── middleware/
│ └── auth.js # Route protection middleware
│
├── model/
│ └── userModel.js # Mongoose schema for users
│
├── routes/
│ └── routing.js # All Express routes
│
└── views/ # EJS templates (UI)
├── login.ejs # Login form
├── register.ejs # Register form
├── home.ejs # Dashboard with user table
└── editUser.ejs # Edit user form
    
## 📦 Modules Used

1. **Express**  
   - Used to create the backend server and define application routes.  
   - Handles HTTP requests and connects controllers to views.  

2. **Mongoose**  
   - Acts as an Object Data Modeling (ODM) library for MongoDB.  
   - Defines schemas and performs database operations.  

3. **EJS (Embedded JavaScript)**  
   - Templating engine to dynamically render HTML pages.  
   - Renders server-side data like usernames, errors, and profile info.  

4. **express-session**  
   - Manages user sessions securely.  
   - Stores session data on the server and authenticates access to protected pages.  

5. **bcrypt**  
   - Hashes user passwords during registration.  
   - Validates hashed passwords during login for secure authentication.  

6. **Bootstrap 5**  
   - Provides a responsive, mobile-friendly, and visually appealing interface.  
   - Styled forms, tables, and alerts for better UX.  

---

## ▶️ How to Run

1. **Clone the repository:**

   git clone https://github.com/your-username/user-management-app.git
   cd user-management-app

2. **Install dependencies:**
     npm install
3. **Set up MongoDB:**
   Run MongoDB locally OR Use MongoDB Atlas and update the MongoDB URI in config/db.js.
4. **Start the server:**
    node app.js
5. **Open in browser:**
   http://localhost:3000
<img width="1092" height="593" alt="Screenshot 2025-09-30 124310" src="https://github.com/user-attachments/assets/b1acc0fd-b17d-4764-b893-1cb440646a36" />

<img width="1037" height="557" alt="Screenshot 2025-09-30 124419" src="https://github.com/user-attachments/assets/8e45f15e-7071-409f-a74e-4f08d0eaa564" />

<img width="1762" height="527" alt="Screenshot 2025-09-30 124433" src="https://github.com/user-attachments/assets/b189145a-4b23-4386-b3ce-892e0cdf475f" />


