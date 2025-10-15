# 🧾 Inventory Management & Billing System

A simple, console-based **Python application** for managing inventory, processing sales, and generating customer bills — built with pure Python and CSV-based storage (no external databases or frameworks).

This project provides a hands-on example of how to design a modular command-line inventory and billing system suitable for small stores, coursework, or learning exercises.

---

## 🚀 Features

✅ **Inventory Management**
- Add, update, delete, and search products  
- View all products with prices and stock levels  
- Automatically saves data to `shaik_inventory.csv`

✅ **Billing System**
- Add or remove products from the shopping cart  
- Apply fixed or percentage-based discounts  
- Checkout and generate bills (`.txt` or `.csv`)  
- Automatically updates stock quantities after purchase  
- Bills are timestamped as `bill_YYYYMMDD_HHMMSS.txt/csv`

✅ **Reports**
- Daily sales report with total transactions and revenue  
- Low stock report (configurable threshold)

✅ **Data Persistence**
- All data stored locally in simple CSV files — portable and easy to inspect  

✅ **User-Friendly CLI**
- Clear menus and friendly prompts for easy navigation  

---

## 🗂️ File Structure

```
📁 Inventory-Billing-System/
│
├── fp.py                   # Main application (Inventory & Billing logic)
├── shaik_inventory.csv      # Product database (ID, name, price, stock)
├── shaik_sales.csv          # Sales log (datetime, total, discount, final)
├── bill_20251015_130116.csv # Example generated bill
└── README.md                # This file
```

---

## ⚙️ How to Run

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

### 2. Run the application
```bash
python fp.py
```

You’ll see a text-based main menu with options for **Product Management**, **Billing**, and **Reports**.

---

## 🧩 Usage Overview

### ▶ Main Menu
```
INVENTORY MANAGEMENT & BILLING SYSTEM
1. Product Management
2. Billing
3. Reports
4. Exit
```

### 📦 Product Management
- Add a new product with ID, name, price, and quantity  
- Update product details  
- Delete or search products  
- View all inventory items  

### 💳 Billing Menu
- Add or remove products from the cart  
- Apply discounts (percentage or fixed)  
- Checkout and generate bill (`.txt` or `.csv`)  

Example flow:
```
1. Add to Cart → Enter Product ID & Quantity
2. Apply Discount → Choose type (percentage/fixed)
3. Checkout → Save Bill as txt/csv
```

### 📈 Reports Menu
- View daily sales summary  
- Generate low stock report (threshold default = 5)

---

## 🧾 Sample Output (Bill Example)

**Bill (TXT format):**
```
==================================================
BILL
==================================================
Date: 2025-10-15 13:01:16
--------------------------------------------------
Items:
  Apple - 3 x $2.50 = $7.50
  Banana - 2 x $1.00 = $2.00
--------------------------------------------------
Subtotal: $9.50
Discount: -$0.50
Total: $9.00
==================================================
```

---

## 🧰 Requirements

- **Python 3.8+**  
- No external libraries required (uses only built-in `os`, `csv`, `datetime`)

---

## 🧠 Future Improvements

- Add GUI or web interface (Tkinter or Flask)  
- Include authentication for admin/users  
- Export reports to Excel or PDF  
- Add product categories and barcode support  
- Implement automated backups  

---

## 👤 Author

**Shaik Md Jakeer**  
📅 *Created on:* 2025-10-15  
💬 *Learning project while exploring Python CLI apps.*

---

## 🪪 License

This project is open-source and available under the [MIT License](LICENSE) 
