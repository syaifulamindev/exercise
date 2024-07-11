### Exercise: Inventory Management System

#### Objective:
Create a simple inventory management system using Swift that handles products in a store.

#### Requirements:

1. **Classes and Structures (20 points)**
   - Create a `Product` class with the following properties:
     - `name: String`
     - `category: String`
     - `price: Double`
     - `quantity: Int`
   - Create a method `productInfo()` that returns a string with the product details.

2. **Inheritance and Polymorphism (20 points)**
   - Create a subclass of `Product` called `PerishableProduct`.
   - Add a new property `expirationDate: Date`.
   - Override the `productInfo()` method to include the expiration date in the output.

3. **Protocols and Extensions (20 points)**
   - Define a protocol `Discountable` with a method `applyDiscount(_ percentage: Double)`.
   - Implement this protocol in both `Product` and `PerishableProduct` classes.
   - Create an extension for the `String` type that adds a method `isValidCategory() -> Bool`. The method should return `true` if the string is a valid category (e.g., "Electronics", "Groceries", "Clothing"), otherwise `false`.

4. **Error Handling (20 points)**
   - Define an enum `InventoryError` conforming to `Error` protocol with cases `outOfStock`, `invalidCategory`, and `expiredProduct`.
   - Create a method `sellProduct(_ product: Product, quantity: Int)` in a new class `InventoryManager` that throws appropriate errors based on the product's availability, category, and expiration date.

5. **Generics (20 points)**
   - Create a generic class `Box<T>` that can hold any type of product.
   - Add methods to add and remove items from the box, and a method to list all items currently in the box.

#### Submission:
- Submit the Swift Playground or Xcode project.
- Include comments explaining your code.
- Provide a README file with instructions on how to run your code and any other relevant information.

#### Grading Criteria:
- **Classes and Structures (20 points):** Proper definition and usage of classes, properties, and methods.
- **Inheritance and Polymorphism (20 points):** Correct implementation of subclass and method overriding.
- **Protocols and Extensions (20 points):** Accurate protocol definition and implementation, and useful extension method.
- **Error Handling (20 points):** Proper error handling and throwing of custom errors.
- **Generics (20 points):** Effective use of generics to create a flexible and reusable class.
