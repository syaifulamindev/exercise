### Assignment: Event Scheduling System

#### Objective:
Create a comprehensive event scheduling system using Swift that handles events, participants, and notifications. This system will utilize protocols, delegates, error handling, and extensions.

#### Requirements:

1. **Classes and Structures (20 points)**
   - Create an `Event` class with the following properties:
     - `title: String`
     - `date: Date`
     - `location: String`
     - `participants: [Participant]`
   - Create a `Participant` struct with the following properties:
     - `name: String`
     - `email: String`
   - Implement a method `eventInfo()` in the `Event` class that returns a string with the event details.

2. **Protocols and Delegates (30 points)**
   - Define a protocol `EventDelegate` with the following methods:
     - `eventDidStart(_ event: Event)`
     - `eventDidEnd(_ event: Event)`
   - Create an `EventManager` class that manages events and implements the `EventDelegate` protocol.
   - Add a property `delegate: EventDelegate?` to the `EventManager` class.
   - Implement the `EventDelegate` methods in the `EventManager` class to handle event start and end notifications.

3. **Error Handling (20 points)**
   - Define an enum `EventError` conforming to the `Error` protocol with cases `eventNotFound` and `participantNotFound`.
   - Create methods in the `EventManager` class to add, remove, and find events by title. Implement appropriate error handling in these methods.

4. **Extensions (20 points)**
   - Create an extension for the `String` type that adds a method `isValidEmail() -> Bool`. The method should return `true` if the string is a valid email address, otherwise `false`.
   - Create an extension for the `Array` type that adds a method `filterEvents(byDate date: Date) -> [Element]` where `Element` is `Event`.

5. **Unit Testing (10 points)**
   - Write unit tests to verify the functionality of your event scheduling system, including testing error cases and delegate methods.

#### Submission:
- Submit the Swift Playground or Xcode project.
- Include comments explaining your code.
- Provide a README file with instructions on how to run your code and any other relevant information.
- Include unit tests to verify the functionality.

#### Grading Criteria:
- **Classes and Structures (20 points):** Proper definition and usage of classes, properties, and methods.
- **Protocols and Delegates (30 points):** Correct implementation of protocols and delegate methods.
- **Error Handling (20 points):** Proper error handling and throwing of custom errors.
- **Extensions (20 points):** Useful extensions for string validation and array filtering.
- **Unit Testing (10 points):** Comprehensive unit tests covering all aspects of the system.
