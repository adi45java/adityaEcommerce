# Mini E-Commerce Web Application

A **Flask-based mini e-commerce web application**. Users can register/login, place orders, and manage products depending on their role. Uses **SQLite database**.

---
## Features

- **Customer:** Register/Login, View products, Place orders, Order history  
- **Seller:** Login, Add/update products, Manage stock & price  
- **Admin:** Manage users, products, and view all orders  

**Bonus Features:**  
- Password hashing for security  
- Search/filter products  
- Flask-Login authentication  

---
## Project Structure
ECOMMERCE_APP/
│── app.py
│── requirements.txt
│── instance/ecommerce.db
│
├── routes/ (users/, products/, orders/)
├── templates/ (auth/, admin/, cart/, order/, product/)
├── static/ (css/, js/, images/)
├── models/ (user.py, product.py, order.py, cart.py)
├── forms/ (auth.py, product.py, order.py)
└── utils/ (seed.py)

---
## Database (SQLite)

- **Users Table:** `UserID, Username, Password, Email, Role`  
- **Products Table:** `ProductID, Name, Price, Stock, SellerID`  
- **Orders Table:** `OrderID, UserID, ProductID, Quantity, OrderDate`  

---
## How to Run

```bash
# Clone the repository
git clone <repo-url>
cd ECOMMERCE_APP

# Create virtual environment
python -m venv venv

# Activate venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  # Mac/Linux

# Install dependencies
pip install -r requirements.txt

# Run application
flask run
Open in browser: http://127.0.0.1:5000

Author
👨‍💻 Aditya Andhale
