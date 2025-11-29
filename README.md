# Campus-Book-Management
Campus Book Exchange System

A full-stack Web Application built using the MERN Stack (MongoDB, Express.js, React.js, Node.js). This platform is designed specifically for university campuses, allowing students to easily buy, sell, and exchange their used books with other students.

🚀 Features

👤 User Features

Secure Authentication: Students can register and login securely.

Browse Books: View a list of available books with images, prices, and condition details.

Search Functionality: Search for specific books by title, author, or category.

My Cart: Add books to the cart and proceed to checkout.

Buy Books: Purchase books directly through the system (Cash on Delivery).

User Dashboard: View "My Uploaded Books" and "My Purchase History".

📚 Book Management Features

Upload Books: Users can list their old books for sale by uploading details and images.

Edit Details: Update book prices, stock status, or descriptions.

Remove Books: Delete a book listing when it is sold or no longer available.

Stock Management: The system automatically updates the availability status of books upon purchase.

Image Handling: Efficient image upload system for book covers.

🛠️ Technology Stack

Component

Technology

Description

Frontend

React.js

Used for building the interactive User Interface.



React-Bootstrap

For responsive design and layout.



Axios

To communicate with the backend server.

Backend

Node.js

The runtime environment for the server.



Express.js

Framework for building the RESTful API.

Database

MongoDB

NoSQL database to store User, Book, and Order data.

Security

JWT

JSON Web Tokens for secure authentication.

Tools

Multer

For handling book image uploads.

⚙️ Installation & Setup Guide

Follow these steps to run the project locally on your machine.

Prerequisites

Node.js (LTS Version)

MongoDB Community Server

1. Clone the Repository

git clone [https://github.com/your-username/campus-book-exchange.git](https://github.com/your-username/campus-book-exchange.git)
cd campus-book-exchange


2. Backend Setup

Navigate to the backend folder and install dependencies.

cd backend
npm install


Configure Environment Variables:
Create a .env file in the backend folder:

MONGO_URI=mongodb://localhost:27017/campus-book-exchange
JWT_SECRET=your_secret_key_12345
PORT=5000


Start the Server:

npm start


3. Frontend Setup

Open a new terminal, go to the frontend folder, and install dependencies.

cd frontend
npm install


Start the React App:

npm start


The app will open at http://localhost:3000.

📂 Project Structure

campus-book-exchange/
├── backend/                # Server Side Logic
│   ├── models/             # Database Schemas (User, Product/Book, Order)
│   ├── routes/             # API Endpoints
│   ├── uploads/            # Book Images
│   └── server.js           # Entry Point
│
└── frontend/               # Client Side Interface
    ├── src/
        ├── components/     # UI Components (Navbar, Dashboard, Products)
        ├── context/        # State Management
        └── App.js          # Main Component


🔗 API Endpoints

Method

Endpoint

Description

Access

POST

/api/auth/register

Register new student

Public

POST

/api/auth/login

Student login

Public

GET

/api/products

Get list of all books

Public

POST

/api/products

Upload a new book

Private

PUT

/api/products/:id

Update book details

Private (Owner)

DELETE

/api/products/:id

Remove a book

Private (Owner)

POST

/api/orders

Buy books (Checkout)

Private

👨‍💻 Author

[Your Name]

Course: CSE 4th Year - ADBMS Project

University: [Your University Name]

📄 License

This project is open-source.
