# Library-Management-System
A simple and beginner-friendly Library Management System built using HTML, CSS, JavaScript, Node.js, Express.js, and SQLite. It allows users to add, view, and delete books with a clean and responsive interface. The backend provides fast and secure CRUD APIs using Express, while the SQLite database stores all book records locally. 

📚 Simple Library Management System

A beginner-friendly full-stack Library Management System built using:

Frontend: HTML, CSS, JavaScript

Backend: Node.js + Express.js

Database: SQLite (using better-sqlite3)

This project provides basic CRUD operations for managing books—add, view, and delete books—through a clean and simple UI.

🚀 Features

✔ Add new books with Title, Author, and Unique ISBN
✔ View all books in a clean table layout
✔ Delete any book instantly
✔ SQLite database stored locally (file-based)
✔ API endpoints using Express.js
✔ Zero external dependencies on large frameworks
✔ Perfect for beginners learning full-stack development

📂 Project Structure
library-system/
├── public/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── database.js
├── server.js
└── package.json

⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/yourusername/library-system.git
cd library-system

2️⃣ Install dependencies
npm install

3️⃣ Run the server
npm start

4️⃣ Open in browser
http://localhost:3000

🗃 Database

The project uses SQLite, initialized through better-sqlite3.
A library.db file is automatically created when running the server.

The database table:

books (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  title TEXT NOT NULL,
  author TEXT NOT NULL,
  isbn TEXT UNIQUE NOT NULL
)

🔌 API Endpoints
GET /api/books

Returns all books.

POST /api/books

Adds a new book.
Body:

{
  "title": "Book Name",
  "author": "Author Name",
  "isbn": "1234567890"
}

DELETE /api/books/:id

Deletes a book by ID.

🎨 Frontend Overview

The frontend is built with:

index.html → Structure

style.css → UI styling

script.js → Fetch API (GET/POST/DELETE) + dynamic rendering

The UI includes:

Form for adding new books

Table showing all available books

Delete buttons for each entry

🧩 Future Enhancements (Optional)

🔹 Edit/update existing books
🔹 Search books by title/author
🔹 Pagination
🔹 User login system
🔹 Export book data to PDF/CSV
🔹 Move to React / Vue frontend

🤝 Contributing

Pull requests are welcome.
For major changes, please open an issue first to discuss what you’d like to improve.

📜 License

This project is open-source and available under the MIT License.
