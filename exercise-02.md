### Assignment: Employee Management System

#### Objective:
Create a simple employee management system using Swift to manage employees and their details.

#### Requirements:

1. **Classes and Structures (20 points)**
   - Create an `Employee` class with the following properties:
     - `name: String`
     - `id: Int`
     - `position: String`
     - `salary: Double`
   - Create a method `employeeInfo()` that returns a string with the employee details.

2. **Inheritance and Polymorphism (20 points)**
   - Create a subclass of `Employee` called `Manager`.
   - Add a new property `department: String`.
   - Override the `employeeInfo()` method to include the department in the output.

3. **Protocols and Extensions (20 points)**
   - Define a protocol `Payable` with a method `calculateAnnualSalary() -> Double`.
   - Implement this protocol in both `Employee` and `Manager` classes.
   - Create an extension for the `Double` type that adds a method `formattedCurrency() -> String`. The method should return the double value formatted as a currency string.

4. **Generics (20 points)**
   - Create a generic class `Company<T>` that can hold any type of employee (e.g., regular employees, managers).
   - Add methods to add and remove employees from the company, and a method to list all employees currently in the company.

5. **Error Handling (20 points)**
   - Define an enum `EmployeeError` conforming to the `Error` protocol with cases `employeeNotFound`, `invalidID`, and `duplicateEmployee`.
   - Create a method `findEmployee(byID id: Int)` in the `Company` class that throws appropriate errors based on the employee's existence.

#### Submission:
- Submit the Swift Playground or Xcode project.
- Include comments explaining your code.
- Provide a README file with instructions on how to run your code and any other relevant information.

#### Grading Criteria:
- **Classes and Structures (20 points):** Proper definition and usage of classes, properties, and methods.
- **Inheritance and Polymorphism (20 points):** Correct implementation of subclass and method overriding.
- **Protocols and Extensions (20 points):** Accurate protocol definition and implementation, and useful extension method.
- **Generics (20 points):** Effective use of generics to create a flexible and reusable class.
- **Error Handling (20 points):** Proper error handling and throwing of custom errors.
