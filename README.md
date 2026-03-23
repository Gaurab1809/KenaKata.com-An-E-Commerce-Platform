<!-- Logo on top -->
<p align="center">
  <img src="KenaKata_Logo.png" alt="KenaKata Logo" width="600"/>
</p>

<!-- Title centered and purple -->
<h1 align="center">
  <span style="color:blue; font-size:36px; font-weight:bold;">🛒 KenaKata.com – An E-Commerce Platform</span>
</h1>

<h3 align="center">
  <b style="color:purple;">💻 A Full-Featured Laravel-Based E-Commerce Web Application</b>
</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Web-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Frontend-Blade-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Backend-Laravel-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Database-MySQL-brightgreen?style=for-the-badge">
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- Abstract Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=📌%20Overview&fontSize=32&width=1200&height=130&color=0:9D50BB,100:6E48AA" width="100%">

**KenaKata.com** is a comprehensive **e-commerce web platform** built with Laravel (PHP framework) to allow users to browse products, manage carts, place orders, and process payments.  

The system includes administrative modules for product, category, and user management, as well as order tracking, while following modern software engineering practices like MVC, SOLID, OOP principles, and design patterns.  

**Keywords:** E-commerce, Laravel, MVC, Blade templates, MySQL, OOP, Design Patterns, SOLID Principles.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- Introduction Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=📖%20Introduction&fontSize=32&width=1200&height=130&color=0:9D50BB,100:6E48AA" width="100%">

In today’s online shopping era, users require a secure, scalable, and intuitive platform to browse products, make purchases, and track orders.  

**KenaKata.com addresses these needs by offering:**
- 🌐 A unified e-commerce ecosystem  
- 🛒 Product browsing and cart management  
- 💳 Secure checkout and payment processing  
- 📊 Admin features for product, user, and order management  

The platform ensures smooth user experience and maintainable backend architecture for long-term scalability.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- System Modules Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=🏗️%20System+Modules&fontSize=32&width=1200&height=130&color=0:FF416C,100:FF4B2B" width="100%">

### 👤 User Features
- Browse products by category  
- Add and manage items in cart  
- Place and track orders  
- Secure checkout and payment processing  

### 🛠️ Admin Features
- Product management (Create, Read, Update, Delete)  
- Category management  
- User management  
- Order tracking and status updates  

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- Background Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=🏗️%20System+Architecture&fontSize=32&width=1200&height=130&color=0:00F260,100:0575E6" width="100%">

The platform follows the **Model-View-Controller (MVC)** architecture with additional Service and Repository layers:

- **Model:** Handles data and business logic (Product, Order, User)  
- **View:** Presentation using Blade templates  
- **Controller:** Handles requests, validation, and communication between Model and View  
- **Service Layer:** Encapsulates business logic  
- **Repository Layer:** Abstracts data access logic  

**MVC Lifecycle:**
1. User interacts with the interface (View)  
2. Request routed to Controller  
3. Controller validates input and calls Service layer  
4. Service layer processes logic and communicates with Repository  
5. Repository interacts with Models via Eloquent ORM  
6. Response sent back through Controller to View  

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- Technology Stack Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=⚙️%20Technology+Stack&fontSize=32&width=1200&height=130&color=0:FC5C7D,100:FF416C" width="100%">

- Backend: Laravel (PHP Framework)  
- Frontend: Blade Templates, HTML, CSS, JavaScript, Bootstrap  
- Database: MySQL  
- ORM: Eloquent ORM  

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- Software Architecture & Design Principles Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=Software%20Architecture%20and%20Design%20Principles&fontSize=32&width=1200&height=130&color=0:6A82FB,100:FC5C7D" width="100%">


### Object-Oriented Programming (OOP) Principles
KenaKata.com leverages **OOP principles** to ensure a modular, maintainable, and scalable architecture. Key principles implemented include:

- **Encapsulation:**  
  All critical data in models like `User`, `Product`, `Order`, and `Cart` are **protected** and accessed only via getter and setter methods. This prevents accidental data manipulation and promotes safe interaction with objects.

- **Abstraction:**  
  Interfaces such as `RepositoryInterface` and `ServiceInterface` hide implementation details from the consumer. Controllers interact with abstractions rather than concrete classes, reducing coupling and enhancing flexibility.

- **Inheritance:**  
  Base classes provided by Laravel, such as `Controller`, are extended to create specific controllers (`ProductController`, `OrderController`). This allows code reuse and enforces a consistent structure across the application.

- **Polymorphism:**  
  The system supports multiple **payment strategies** (`PayPalPayment`, `StripePayment`, `CashOnDelivery`) that implement a common `PaymentInterface`. This allows switching or adding payment methods without modifying existing code.

---

### Design Patterns Implemented
KenaKata.com applies widely recognized **software design patterns** to solve recurring problems efficiently:

- **Strategy Pattern:**  
  Used for **pricing and payment strategies**, enabling dynamic switching of behavior at runtime without altering client code.

- **Adapter Pattern:**  
  Integrates legacy or third-party systems with the application via a common interface.

- **Repository Pattern:**  
  Abstracts data access logic from business logic, making the system flexible to change database implementations or perform complex queries via Eloquent ORM.

- **Service Layer Pattern:**  
  Encapsulates business logic separate from controllers and repositories, keeping controllers lightweight.

- **Observer Pattern:**  
  Implements **events and notifications**, e.g., sending emails when an order is placed or status is updated.

- **Factory Pattern:**  
  Generates test data and objects for unit testing and seeding purposes, ensuring consistency and reducing repetitive code.
---

### SOLID Principles

KenaKata.com follows the **SOLID principles** to ensure that the codebase is **maintainable, scalable, and easy to extend**. These principles guide the design of classes, interfaces, and modules in the application.

- **S – Single Responsibility Principle (SRP):**  
  Each class in the system has a **single responsibility**. For example, the `ProductService` handles all business logic related to products, while the `OrderService` focuses only on order processing. This reduces complexity and improves maintainability.

- **O – Open/Closed Principle (OCP):**  
  Classes and modules are **open for extension but closed for modification**. For instance, new payment methods or discount strategies can be added via strategy patterns without modifying existing classes, ensuring minimal risk of breaking existing functionality.

- **L – Liskov Substitution Principle (LSP):**  
  Subclasses can **replace their parent classes** without affecting the correctness of the program. Example: Different types of `PaymentGateway` implementations (like `PayPalGateway` or `StripeGateway`) can be used interchangeably wherever the base `PaymentGateway` interface is expected.

- **I – Interface Segregation Principle (ISP):**  
  Clients are not forced to implement interfaces they don’t use. The system defines **specific interfaces** for services, repositories, and payment strategies, so each module only implements the methods it actually needs.

- **D – Dependency Inversion Principle (DIP):**  
  High-level modules depend on **abstractions, not concrete implementations**. For example, controllers depend on service interfaces rather than directly instantiating service classes, which allows easy swapping of implementations and better testability.
  
By adhering to SOLID principles, KenaKata.com achieves a **robust, flexible, and modular architecture**, making future enhancements and maintenance seamless.

---

### Design by Contract (DbC)
The system also implements **Design by Contract** to ensure reliability and correctness:

- **Preconditions:**  
  Input validation is enforced at the controller level using Laravel’s request validation system, ensuring only valid data reaches the business logic.

- **Postconditions:**  
  Unit tests (PHPUnit) verify that actions such as order creation, payment processing, and cart updates meet expected outcomes.

- **Interface Contracts:**  
  Interfaces define clear **contracts**, ensuring that all implementations behave consistently and reliably.
---
By combining **OOP, design patterns, SOLID, and DbC**, KenaKata.com achieves a **high-quality, maintainable, and professional software architecture**.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- Database Design Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=Database%20Design&fontSize=32&width=1200&height=130&color=0:00F260,100:0575E6" width="100%">

The database of **KenaKata.com** is designed to ensure **data integrity, efficiency, and scalability**, following best practices of relational database design.

- **Normalized Structure:**  
  The database is normalized to reduce redundancy and ensure consistency across tables.

- **Foreign Key Constraints:**  
  Relationships between entities are enforced using foreign keys, maintaining referential integrity.

- **Naming Conventions:**  
  Uses `snake_case` naming for tables and columns to maintain consistency and readability.

- **Primary Keys:**  
  Auto-incremented primary keys are used for unique identification of records.

---

### Core Entities
The system is built around the following key entities:

- **Users:** Stores user credentials, roles, and profile information  
- **Products:** Contains product details such as name, price, stock, and category  
- **Orders:** Manages order transactions, statuses, and user associations  
- **Categories:** Organizes products into logical groups  
- **Cart:** Handles temporary user selections before checkout  

---

### ORM & Querying
The application utilizes Laravel’s **Eloquent ORM** for efficient and expressive database interaction:

- Supports **One-to-Many** (e.g., User → Orders) and **Many-to-Many** (e.g., Products ↔ Categories) relationships  
- Provides **fluent, readable queries** similar to LINQ  
- Simplifies CRUD operations and relationship management  

---

### Advanced Database Features
To enhance performance and enforce business logic at the database level, the system also incorporates:

- **Joins & Complex Queries:**  
  SQL joins (INNER JOIN, LEFT JOIN, etc.) are used to efficiently retrieve related data across multiple tables (e.g., orders with user and product details).

- **Stored Procedures:**  
  Predefined SQL procedures are used for complex operations such as order processing and bulk data manipulation, improving performance and reducing application-level overhead.

- **Database Triggers:**  
  Triggers are implemented to automatically execute actions on events like insert/update/delete (e.g., updating stock after an order is placed).

- **Optimized Query Execution:**  
  Indexing and efficient query design are used to improve database performance for large-scale data handling.

---

Overall, the database design ensures **high performance, consistency, and scalability**, supporting the application’s real-world e-commerce requirements.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<!-- Installation Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&text=📦%20Installation&fontSize=32&width=1200&height=130&color=0:FF416C,100:FF4B2B" width="100%">

### 1. Clone the Repository
```bash
git clone https://github.com/Gaurab1809/KenaKata.com---An-E-Commerce-Platform.git
cd KenaKata.com---An-E-Commerce-Platform
```
### 2. Install Dependencies
```bash
composer install
npm install
```
### 3. Setup Environment
```bash
cp .env.example .env
php artisan key:generate
```
### 4. Configure Database

Edit .env file:
```bash
DB_DATABASE=your_db
DB_USERNAME=root
DB_PASSWORD=
```
### 5. Run Migration
```bash
php artisan migrate
```
### 6. Start Server
```bash
php artisan serve
```
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">


<!-- Future Work Banner --> 
<img src="https://capsule-render.vercel.app/api?type=waving&text=🔮%20Future+Improvements&fontSize=32&width=1200&height=130&color=0:FF416C,100:FF4B2B" width="100%">

- Multiple payment gateway integration  
- AI-based recommendation system  
- Advanced filtering and search  
- Mobile application integration  
- Real-time notifications
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"> 

<!-- Conclusion Banner --> 
<img src="https://capsule-render.vercel.app/api?type=waving&text=✅%20Conclusion&fontSize=32&width=1200&height=130&color=0:6A82FB,100:FC5C7D" width="100%">

KenaKata.com is a scalable, maintainable, and feature-rich e-commerce platform built with Laravel, demonstrating modern architecture, OOP principles, design patterns, and best practices suitable for real-world applications.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"> 


<!-- Author Banner --> 
<img src="https://capsule-render.vercel.app/api?type=waving&text=👨‍💻%20Author&fontSize=32&width=1200&height=130&color=0:00F260,100:0575E6" width="100%">

### A. K. M. Masudur Rahman (Gaurab)
🎓 Department of Computer Science and Engineering (CSE)   
🏫 Bangladesh Army University of Science and Technology (BAUST), Saidpur    
📧 Email: akmmasudurrahmangaurab@gmail.com

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"> 

<!-- Support Banner --> 

<img src="https://capsule-render.vercel.app/api?type=waving&text=⭐%20Support&fontSize=32&width=1200&height=130&color=0:FF416C,100:FF4B2B" width="100%">

If you like this project, consider giving it a ⭐ on GitHub!
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%"> 
