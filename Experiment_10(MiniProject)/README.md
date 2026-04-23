# 🛒 E-Commerce Inventory & Order System

## 📌 Project Overview
This project is a scalable **E-Commerce Inventory & Order Management System** inspired by platforms like Amazon and Flipkart.  
It allows users to browse products, manage carts, place orders, and track them, while ensuring efficient inventory management and system scalability.

---

## 🎯 Objectives
- Design a production-grade system using System Design principles
- Implement scalable architecture
- Ensure consistency in inventory management
- Apply real-world trade-offs and optimizations

---

## ⚙️ Features

### 👤 User Features
- User Registration & Login
- Browse/Search Products
- Add to Cart
- Place Orders
- Track Orders

### 🏪 Admin/System Features
- Product Management
- Inventory Management
- Order Processing
- Payment Handling
- Notifications

---

## 🧠 System Design Concepts Used
- High-Level Design (HLD)
- Low-Level Design (LLD)
- REST API Design
- Database Design
- Caching Strategy
- Load Balancing
- Distributed Systems
- CAP Theorem
- Scalability & Reliability Engineering

---

## 🏗️ System Architecture (Overview)
The system follows a modular architecture with the following components:

- API Gateway
- User Service
- Product Service
- Cart Service
- Order Service
- Payment Service
- Inventory Service
- Notification Service
- Database (SQL)
- Cache (Redis)
- Message Queue (Kafka)

---

## 🔄 Data Flow (Order Placement)
1. User places an order
2. Order Service creates order
3. Payment Service processes payment
4. Inventory Service updates stock
5. Notification Service sends confirmation

---

## 🛠️ Tech Stack (with Justification)

| Layer | Technology | Reason |
|------|-----------|--------|
| Backend | Node.js / Spring Boot | Scalable & fast |
| Database | MySQL / PostgreSQL | Strong consistency |
| Cache | Redis | Low latency reads |
| Message Queue | Kafka | Asynchronous processing |
| Storage | AWS S3 | Scalable file storage |
| API | REST | Simplicity & compatibility |

---

## ⚖️ Trade-offs
- **SQL vs NoSQL:** Chose SQL for strong consistency in inventory
- **Consistency vs Availability:** Prioritized consistency to avoid overselling
- **Monolith vs Microservices:** Started with modular monolith for simplicity

---

## 🚧 Assumptions
- Single region deployment (initial phase)
- Moderate traffic initially
- Users have stable internet connection
- Payment gateway is reliable

---

## 📈 Scalability Considerations
- Horizontal scaling using load balancers
- Redis caching for frequently accessed data
- Database replication for read scalability
- Sharding for large datasets
- Kafka for asynchronous processing

---

## ⚠️ Bottleneck Identified
**Inventory Service overload during high traffic**

### ✅ Solution:
- Introduced Kafka queue for async inventory updates
- Reduced direct DB writes
- Improved system throughput

---

## 🔒 Reliability & Performance
- Retry mechanisms for failed requests
- Circuit breaker pattern
- Rate limiting to prevent abuse
- CDN for faster content delivery

---

## 🔮 Future Improvements
- Microservices architecture
- AI-based recommendation system
- Multi-region deployment
- Advanced analytics dashboard
- Real-time order tracking

---

## 📂 Project Structure
/MiniProject_E-CommerceSystem
├── HLD.drawio
├── LLD.drawio
├── api.drawio
├── scaling.drawio
└── README.md

---

## 🧪 Optional Enhancements
- Backend implementation (Node.js / Java)
- Swagger API documentation
- Deployment on AWS / Docker

---

## 📅 Submission Details
- Course: System Design Lab
- Project Type: Mini Project
- Deadline: As per submission guidelines

---

## 👨‍💻 Author
- Name: Shivanshu Ranjan
- Course: B.Tech CSE

---

## ⭐ Final Note
This project demonstrates real-world system design thinking including scalability, reliability, and trade-offs, similar to top product-based companies.
