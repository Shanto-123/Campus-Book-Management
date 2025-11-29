📚 Campus Book Exchange System

A full-stack MERN (MongoDB, Express.js, React.js, Node.js) web application built for university campuses so students can buy, sell, and exchange used books easily.

🚀 Features
👤 User Features

Secure authentication (Register / Login)

Browse books with images, price, and condition

Search & filter by title, author, or category

Add to cart and checkout (Cash on Delivery)

User dashboard: My Uploaded Books & Purchase History

📚 Book Management

Upload books with images and details

Edit book info (price, stock, description)

Remove book listings

Automatic stock update after purchase

Image handling with Multer

🛠️ Technology Stack

Frontend: React.js, React-Bootstrap, Axios

Backend: Node.js, Express.js

Database: MongoDB

Authentication: JWT (JSON Web Tokens)

File Uploads: Multer

⚙️ Installation & Setup
Prerequisites

Node.js (LTS)

MongoDB Community Server

1. Clone the repository
git clone https://github.com/your-username/campus-book-exchange.git
cd campus-book-exchange

2. Backend setup
cd backend
npm install


Create .env in backend/:

MONGO_URI=mongodb://localhost:27017/campus-book-exchange
JWT_SECRET=your_secret_key_12345
PORT=5000


Start backend:

npm start
# or for dev with hot reload
npm run dev

3. Frontend setup

Open a new terminal:

cd frontend
npm install
npm start


The frontend will open at: http://localhost:3000

📂 Project Structure
campus-book-exchange/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── uploads/
│   ├── .env
│   └── server.js
└── frontend/
    ├── public/
    └── src/
        ├── components/
        ├── pages/
        └── api/

🔗 API Endpoints
Method	Endpoint	Description	Access
POST	/api/auth/register	Register new student	Public
POST	/api/auth/login	Student login	Public
GET	/api/products	Get list of all books	Public
POST	/api/products	Upload a new book	Private
PUT	/api/products/:id	Update book details	Private (Owner)
DELETE	/api/products/:id	Remove a book	Private (Owner)
POST	/api/orders	Buy books (Checkout)	Private
📸 Screenshots

Below are visual previews of the frontend. Replace the placeholder paths with your actual screenshot file paths (commit them under /frontend/public/assets/screenshots/ or /assets/screenshots/).

🏠 Home Page

Shows book listings, navbar, and search bar.


🔍 Search & Filter

Search books by title, category, or author.


📘 Book Details

Detail view with description, price, condition, seller info.


🛒 Cart Page

Review items in cart and proceed to checkout.


📤 Upload Book

Page to upload book details and images.


👤 User Dashboard

View uploaded books, purchase history, and account settings.


✅ Notes & Tips

For production: store images in cloud storage (S3, Cloudinary), enable HTTPS, configure CORS properly, and add rate limiting.

Consider adding client-side validation and richer UI/UX for better user experience.

If you want, I can create optimized screenshot images and a repo banner for README.

👨‍💻 Author

Your Name
Course: CSE 4th Year — ADBMS Project
University: [Your University Name]

📄 License

This project is open-source.
