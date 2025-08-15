# Heladeepa Bookshop – Full-Stack E-Commerce Web Application

## 📖 Overview

**Heladeepa Bookshop** is a full-featured **e-commerce platform** built for a local SME bookstore in Sri Lanka, designed to handle over **100 SKUs** with **real-time order management**.
The system empowers customers to easily browse, search, and purchase books/stationery, while providing administrators with robust catalog, inventory, bulk upload, and notification tools.

This project was delivered through **five agile sprints**, resulting in \~**60% improvement** in admin and customer efficiency.

---

## 🚀 Key Features

### 🛒 Customer-Facing Features

* **Catalog Browsing & Search** – Keyword-based search with real-time suggestions, category navigation.
* **Advanced Filtering** – Filter by price, category, author, publisher, availability.
* **Wishlist & Favorites** – Add/remove items, sync across devices.
* **Shopping Cart** – Add/update/remove items with real-time stock visibility.
* **Promotions & Discounts** – Apply discount codes, view ongoing offers.
* **Checkout & Payments** – Secure checkout via **Stripe** payment gateway.
* **Pre-orders** – Reserve upcoming book releases.
* **Notifications** – Email/SMS alerts for orders, wishlist restocks, and pre-order availability.
* **OCR-Based Booklist Upload** – Upload handwritten booklists via images for automatic extraction.
* **Manual Booklist Entry** – For customers preferring manual input.

### 🛠 Admin & Backend Features

* **Role-Based Access Control** – Manage permissions for admins.
* **Catalog Management** – Add, edit, update, delete items.
* **Inventory Management** – Automated stock updates from sales and restocks.
* **Order Management Dashboard** – Centralized tracking of all orders.
* **Bulk Upload of Booklists** – CSV/Excel upload with error validation and rollback.
* **Promotion Management** – Dedicated admin panel for offers and campaigns.
* **Low-Stock Alerts** – Automated alerts for restocking needs.

---

## 🏗 Architecture & Tech Stack

### Frontend

* **JavaScript (React + Vite)** – High-performance SPA with modular UI components.
* **UI Libraries** – Responsive design with reusable elements.

### Backend

* **Java (Spring Boot)** – REST API services for authentication, catalog, orders, inventory, and notifications.
* **Security** – Password encryption, email verification, session management.

### Database

* **MySQL** – Relational database for structured product, user, and order data.

### Development & Tools

* **IDE:** IntelliJ IDEA
* **API Testing:** Postman
* **Version Control:** GitHub
* **Project Management:** Jira
* **OCR & Image Processing:** Integrated library for handwritten text recognition.

---

## 📅 Agile Development Summary

The project followed **five agile sprints**, each targeting specific epics:

| Sprint | Duration | Goal                                                 |
| ------ | -------- | ---------------------------------------------------- |
| **1**  | 1 week   | Core browsing, search, authentication                |
| **2**  | 2 weeks  | Filtering, cart, wishlist, promotions                |
| **3**  | 3 weeks  | Checkout, payments, admin tools, bulk uploads        |
| **4**  | 2 weeks  | Inventory automation, order dashboard, pre-orders    |
| **5**  | 2 weeks  | OCR-based booklist entry, notifications, refinements |

---

## 🔒 Security Considerations

* Password encryption using industry-standard hashing algorithms.
* Email verification for new users.
* Session security and automatic logout for inactive sessions.
* Role-based access control for admins.

---

## 📂 Project Structure

```
heladeepa-bookshop/
│── backend/         # Spring Boot services
│── frontend/        # React + Vite client app
│── database/        # MySQL schema & migrations
│── docs/            # API docs, Sprint reports
│── tests/           # Unit & integration tests
```

---

## ⚠ Risk Mitigation Strategies

* **Real-time Search Performance:** Optimized DB queries and caching.
* **Payment Reliability:** Early sandbox testing with Stripe.
* **Bulk Upload Data Safety:** File validation, rollback mechanisms.
* **OCR Accuracy:** Pre-trained models with diverse handwriting samples.
* **Notification Reliability:** Event trigger testing with batch job fallback.

---

## 📸 Screenshots & Demos

*(Add screenshots here of catalog, cart, checkout, admin dashboard)*

---

## 🛠 Setup Instructions

### Prerequisites

* **Java 17+**
* **Node.js 18+**
* **MySQL 8+**

### Installation

```bash
# Clone repo
git clone https://github.com/<your-repo>.git
cd heladeepa-bookshop

# Backend
cd backend
./mvnw spring-boot:run

# Frontend
cd ../frontend
npm install
npm run dev
```

### Database Setup

* Import `database/schema.sql` into MySQL.
* Update `application.properties` in backend with DB credentials.

---

## 📬 Contact

* **Developers:** Pavan Kumarage, Sithija Oshan, Madara Chamudini, Nikini Bandara
* **Email:** pavanvilhan@gmail.com
