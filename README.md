# 🚀 Software Engineering Systems

## 👩‍💻 Created by:

**Riya Korani**

---

## 📌 Project Overview

This repository contains system designs and documentation for real-world scalable applications.
It focuses on **software engineering principles, requirement validation, traceability, system design, and real-world problem-solving**.

---

## 🎯 Objective

To design production-level systems with:

* Clear requirements
* Scalable architecture thinking
* Edge case handling
* Testability and validation

---

## 📌 Assumptions

* Users have stable internet connectivity
* Payment gateway is external and reliable
* Restaurants regularly update menu availability
* System operates under normal load unless specified

---

## ⚙️ Constraints

* System must respond within 2 seconds
* Limited database performance under peak load
* Dependency on third-party payment services
* Limited delivery availability during high demand

---

## 📊 Systems Included

### 🚆 IRCTC Train Booking System

* User authentication
* Train search and filtering
* Seat selection & booking
* Payment processing
* Ticket generation

---

### 🛒 Online Shopping System

* User login/signup
* Product browsing & filtering
* Cart management
* Checkout & payment
* Order tracking

---

### 🍔 Food Delivery System

* Restaurant browsing
* Menu selection
* Cart & checkout
* Payment system
* Order tracking & delivery

---

## 🏗️ High-Level Architecture

* User interacts with the system via frontend
* Requests are handled through backend APIs
* Backend manages authentication, orders, and payments
* Database stores users, products, orders, and transactions

---

## 🔗 API Design (Sample)

POST /login
POST /signup
GET /restaurants
GET /products
POST /order
POST /payment
GET /track-order
DELETE /order

---

## ⚡ Non-Functional Requirements

* Scalability: Supports up to 100K concurrent users
* Performance: API response time < 2 seconds
* Availability: 99.9% uptime
* Security: Authentication and authorization enforced
* Reliability: Retry mechanism for failed operations

---

## 🔐 Security Considerations

* Passwords must be encrypted
* Secure authentication mechanism (JWT planned)
* Protection against unauthorized access
* Secure payment processing via trusted gateway

---

## ⚠️ Edge Cases Considered

* Payment failure during checkout
* Duplicate order submission
* Item out of stock
* Service unavailable (restaurant/train/product)
* Network failure during transaction
* Order cancellation after payment

---

## 📊 Requirement Traceability Matrix (RTM)

| ID | Requirement        | Module           | API              | Test Case |
| -- | ------------------ | ---------------- | ---------------- | --------- |
| R1 | User Login         | Auth Service     | POST /login      | TC1       |
| R2 | Browse Restaurants | Catalog          | GET /restaurants | TC2       |
| R3 | Place Order        | Order Service    | POST /order      | TC3       |
| R4 | Payment Processing | Payment Service  | POST /payment    | TC4       |
| R5 | Order Tracking     | Delivery Service | GET /track-order | TC5       |
| R6 | Cancel Order       | Order Service    | DELETE /order    | TC6       |
| R7 | User Signup        | Auth Service     | POST /signup     | TC7       |

---

## 🧪 Sample Test Cases

* TC1: Valid login → User authenticated successfully
* TC2: Invalid login → Error message displayed
* TC3: Payment failure → Retry option available
* TC4: Successful order → Order ID generated
* TC5: Track order → Correct status displayed
* TC6: Cancel order → Order status updated

---

## 📁 Contents

* Flowcharts (PNG format)
* SRS Document
* ER Diagram
* DFD Levels (0, 1, 2)

---

## 📷 Diagrams Preview

### 🚆 IRCTC Train Booking System

![IRCTC System](train-booking-flowchart.drawio.png)

### 🛒 Online Shopping System

![Online Shopping System](Shopping.drawio.png)

### 🍔 Food Delivery System

![Food Delivery System](food%20delivery.drawio.png)

---

## 📊 ER Diagram

### 🍔 Food Delivery System

![Food Delivery System](food-delivery-system-er-diagram.png)

---

## 📊 Food Delivery System - DFD

### 🔹 Level 0 DFD

![Level 0](food_delivery_dfd_level_0.png)

### 🔹 Level 1 DFD

![Level 1](food_delivery_dfd_level_1.png)

### 🔹 Level 2 DFD

![Level 2](food_delivery_dfd_level_2.png)

---

## 🛠 Tools Used

* Creately
* draw.io (diagrams.net)
* Mermaid

---

## 💡 Engineering Highlights

* Requirement Validation applied
* Requirement Traceability ensured
* Edge case handling included
* System design thinking demonstrated
* API-first design approach
* Designed with scalability and failure handling in mind

---

## 🚀 Future Enhancements

* Real-time order tracking
* Recommendation system
* Microservices architecture
* Cloud deployment (AWS/Azure)
* Load balancing and caching

---

## ⭐ Note

This project is designed with a focus on **real-world engineering practices used in scalable systems** and serves as a foundation for backend implementation and system design interviews.

---
