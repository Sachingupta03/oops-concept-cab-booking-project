# 🚖 Cab Online Booking System (Uber, Ola, Rapido Clone)

## 📌 Overview
This is a **Cab Booking System** built using **Java** that implements **OOP concepts** such as **Encapsulation, Inheritance, Polymorphism, and Abstraction**. The project follows a **POJO-based architecture** with a layered structure including **Models, Services, Controllers, Exception Handling, and Payment Processing**.

---

## 📂 Project Structure
cab-booking-system/ │── src/ │ ├── model/ # POJO (Plain Old Java Objects) - Entities │ │ ├──
Driver.java │ │ ├── User.java │ │ ├── Rider.java │ │ ├── Rating.java │ │ │ ├── service/ # Business
Logic (Service Layer) │ │ ├── DriverService.java │ │ ├── UserService.java │ │ ├── RiderService.java │ │ ├──
RatingService.java │ │ │ ├── controller/ # API Layer (Controller) │ │ ├── DriverController.java │ │ ├──
UserController.java │ │ ├── RiderController.java │ │ ├── RatingController.java │ │ │ ├── exception/ # Exception Handling │ │ ├── 
CabBookingException.java │ │ │ ├── payment/ # Abstraction (Payment Methods) │ │ ├── Payment.java # Abstract Class 
│ │ ├── UPI.java │ │ ├── Cash.java │ │ ├── CreditCard.java │ │ │ ├── main/ # Entry Point │ │ ├── CabBookingSystem.java │ │──
README.md # Project Documentation │── pom.xml (If using Maven) │── build.gradle (If using Gradle)
## 🎯 Key Features
✅ **User Management:** Register & manage users.  
✅ **Driver Management:** Add, view available drivers.  
✅ **Ride Booking:** Users can book a ride with available drivers.  
✅ **Rating System:** Users can rate drivers after rides.  
✅ **Payment System:** Supports UPI, Cash, Credit Card payments.  
✅ **Exception Handling:** Handles errors like unavailable drivers, invalid payments.  

---

## 🏗️ OOP Concepts Used

### 1️⃣ **Encapsulation (Data Hiding)**
- **POJO classes** (`Driver`, `User`, `Rider`, `Rating`) have **private fields** with public getter/setter methods.
- Prevents direct access to sensitive data.

### 2️⃣ **Inheritance (Code Reusability)**
- **Payment** is an **abstract class** that is inherited by `UPI`, `Cash`, `CreditCard`.
- Helps in **code reuse** by implementing different payment methods.

### 3️⃣ **Polymorphism (Method Overriding & Overloading)**
- **Overriding:** `makePayment()` is overridden in `UPI`, `Cash`, `CreditCard` classes.
- **Overloading:** Different constructors in POJO classes.

### 4️⃣ **Abstraction (Hiding Implementation Details)**
- **Payment** is an **abstract class**, so users only interact with `makePayment()`, hiding internal logic.

---

## 🔧 Setup & Installation

### Prerequisites
- **Java 17+**
- **Maven or Gradle** (optional)
- **IDE** (IntelliJ IDEA, Eclipse, VS Code)

### Steps to Run
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-repo/cab-booking-system.git
   cd cab-booking-system
