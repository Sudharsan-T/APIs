# 📚 APIs – Bookstore & Cart Management using Flask

This repository demonstrates a simple backend API system built with Python, combining **object-oriented programming** and **Flask web development**. It includes:

- A **Bookstore Management System** using custom Python classes.
- A **Library Manager** class to handle operations.
- A **Flask-based shopping cart API** with a basic HTML UI.

---

## 🚀 Features

### ✅ Bookstore System
- Add books with `id`, `title`, `author`, `year`, and `genre`.
- Retrieve a book by its ID.
- Demonstrates object-oriented principles in Python.

### ✅ Library Manager
- Acts as a bridge between the user and the bookstore.
- Manages book addition using clean modular design.

### ✅ Shopping Cart API (Flask)
- Add and delete items from a cart using APIs.
- Displays cart items on a webpage via Jinja2 templates.
- Simple and interactive HTML UI.

---

## 📁 Project Structure

```
APIs/
├── simple.py                # Bookstore class (OOP)
├── manager.py               # LibraryManager class
├── app.py                   # Flask app for shopping cart
├── templates/
│   └── index.html           # Frontend UI for cart
└── README.md                # Project documentation
```

---

## 🛠️ Requirements

- Python 3.x
- Flask

Install Flask using pip:

```bash
pip install flask
```

---

## 🧪 How to Run

### ▶️ Bookstore System

To run the bookstore logic:

```bash
python simple.py
# or
python manager.py
```

### ▶️ Shopping Cart API

To run the Flask API:

```bash
python app.py
```

Then open your browser and go to:

```
http://127.0.0.1:5000/
```

You can:
- Add products to the cart
- View cart items
- Remove products from the cart

---

## 📡 API Endpoints

| Method | Endpoint                  | Description            |
|--------|---------------------------|------------------------|
| POST   | `/api/add`                | Add product to cart    |
| DELETE | `/api/delete/<name>`      | Delete product by name |

---

## 🧩 Example Bookstore Code

```python
bookstore = Bookstore()
book1 = bookstore.add_book(1, "The Great Gatsby", "F. Scott Fitzgerald", 1925, "Fiction")
print(bookstore.get_book_by_id(1)["title"])
```

## 📌 Future Enhancements

- Add full CRUD support (Update, List all)
- Connect to SQLite or PostgreSQL
- Implement user authentication
- Expand UI with modern frontend frameworks

---

## 👨‍💻 Author

**Sudharsan T**  
Aspiring AI & Data Engineer  
🌐 [Portfolio Website](https://sudharsan-t7.web.app)  
💼 [LinkedIn](https://www.linkedin.com/in/yourprofile)  
📦 [GitHub](https://github.com/yourgithub)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
