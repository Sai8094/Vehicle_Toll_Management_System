# 🚗 Vehicle Toll Management System in Java

## 📌 Overview
This project simulates a **Toll Booth System** where different types of vehicles pass through.  
Each vehicle type (Bike, Car, Truck) has its own **toll rate** and **length of stay**.  
The project applies **core OOP principles** like **Abstraction, Inheritance, Polymorphism, and Encapsulation**.

---

## 🛠 Features
- Supports three vehicle types:
  - 🏍 **Bike**
  - 🚙 **Car**
  - 🚛 **Truck**
- Each vehicle has:
  - Unique **plate number**
  - Vehicle-specific **toll amount**
  - **Length of stay** (time at toll plaza)
- Toll Booth operations:
  - ✅ Accept a vehicle
  - 💰 Calculate toll
  - 📊 Track total revenue
  - 📑 Display passing vehicle info

---

## 🏗 Design
- **Vehicle (Abstract Class)**  
  - Fields: `plateNumber`  
  - Abstract Method: `getTollAmount()`  
  - Common Method: `getPlateNumber()`  
- **Bike, Car, Truck (Subclasses)**  
  - Override `getTollAmount()` with vehicle-specific rates  
- **TollBooth (Class)**  
  - Processes different vehicles using **polymorphism**  
  - Tracks **total revenue** and logs vehicle details  
- **Main (Simulation Class)**  
  - Demonstrates toll collection with multiple vehicles  

---

## 🎯 Core Logic
- **Abstraction** → `Vehicle` defines the interface for all vehicles.  
- **Inheritance** → `Bike`, `Car`, and `Truck` extend `Vehicle`.  
- **Polymorphism** → `getTollAmount()` behaves differently for each vehicle type.  
- **Encapsulation** → Details like `plateNumber` and toll rates are kept private.  

---

## 📚 OOP Concepts Used
- **Abstraction** → Base class `Vehicle` provides common structure.  
- **Inheritance** → Subclasses reuse and extend vehicle logic.  
- **Polymorphism** → Same interface (`getTollAmount`) works differently for each vehicle.  
- **Encapsulation** → Vehicle details are private, accessed via getters.  
