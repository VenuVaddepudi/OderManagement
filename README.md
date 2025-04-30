# iOS Order Management System

This iOS application is an Order Management System that allows users to manage orders. Users can register, log in, view orders, add new orders, edit existing orders, and delete orders.

## Requirements

The application fulfills the following requirements:

* Develops a registration page with username, password, and confirm password fields.
* Creates a login page with username, password, and a "remember me" option.
* Validates username and password fields to ensure they are not empty.
* Redirects users to an orders screen upon successful login.
* Displays all orders in a table view on the orders screen.
* Provides details for each order, including Order Number, Order Due Date, Customer Buyer Name, Customer Address, Customer Phone, and Order Total.
* Implements edit and delete actions within the order table.
* Includes a "New Order" button to add new orders.
* Opens a popup/form for adding new orders and editing existing orders.
* Allows editing of all fields in the edit order form.
* Prompts users for confirmation before deleting an order.
* Utilizes Core Data for storing user login and order details.
* Supports multiple user logins.
* Maintains a clean and simple user interface (UI).

## Features

### User Authentication:
* User registration with username, password, and confirm password validation.
* User login with username and password.
* Toggling between login and registration views.

### Order Management:
* Displaying orders in a table view.
* Adding new orders with details (Order Number, Order Due Date, Customer Buyer Name, Customer Address, Customer Phone, Order Total).
* Editing existing orders.
* Deleting orders with confirmation.

## Technical Details

* **Language:** Swift  
* **SDK:** Latest iOS SDK  
* **Data Persistence:** Core Data

## Code Structure

* `ViewController.swift`: Handles user authentication (login/registration) and navigation.
* `OrderViewController.swift`: Handles the display and management of orders (table view, add, edit, delete).
* `OrderFormViewController.swift`: Handles the order form popup for creating/editing orders.
* `AppDelegate.swift`: Sets up the Core Data stack.
* Core Data Model (`.xcdatamodeld`): Defines the data model for User and Order entities.

## Approach

1. **Core Data Setup:**
   * Defined the `User` and `Order` entities in the Core Data model.
   * Established a relationship between `User` and `Order` to manage user-order associations.

2. **UI Development:**
   * Created UI elements for login, registration, order display, and order forms.
   * Used `UIStackView` and Auto Layout for flexible and responsive UI.
   * Implemented UI toggling between login and registration modes.

3. **Authentication Logic:**
   * Implemented user registration and login functionality using Core Data to store and retrieve user data.
   * Included input validation for registration (password confirmation).

4. **Order Management Logic:**
   * Developed the order display table view.
   * Implemented functionality to add, edit, and delete orders, interacting with Core Data to persist changes.
   * Used mock data for order details during development.

## Challenges Faced

* **Core Data Relationships:** Initially, setting up the inverse relationship in Core Data was tricky, but it was crucial for data consistency.
* **UI Layout:** Achieving a clean and adaptable UI across different screen sizes required careful use of `UIStackView` and Auto Layout.
* **State Management:** Managing the login/registration mode and updating the UI accordingly required a clear state management approach.

## Areas for Improvement

* **Password Hashing:** In a real-world application, passwords should be hashed (e.g., using `bcrypt`) instead of stored in plain text. *This is a critical security improvement.*
* **Error Handling:** More robust error handling and user feedback could be implemented (e.g., specific error messages for username already exists).
* **UI Polish:** Further UI/UX enhancements could be added for a more polished look and feel.
* **"Remember Me" Functionality:** The "Remember Me" feature is in the UI but not fully implemented. This would require saving user sessions (securely).
* **Navigation:** Using segues or coordinators for navigation between login/registration and order screens would improve code organization.
* **Data Validation:** More comprehensive data validation for order details could be added.

## How to Run the App

1. Clone the GitHub repository.
2. Open the `OrderManagement.xcodeproj` in Xcode.
3. Build and run the app on a simulator or a physical iOS device.

## GitHub Repository

[https://github.com/VenuVaddepudi/OderManagement]

## Commit History

The commit history is maintained to be readable and clear, documenting the development process.

## Contact

venuvaddepudi@gmail.com

Thank you for reviewing my application.

---
