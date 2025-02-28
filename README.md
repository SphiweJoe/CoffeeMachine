Certainly! Below is the complete content for the `README.md` file, formatted and ready for use:

```markdown
# Coffee Machine Project

## Description
The **Coffee Machine** is a Java-based console application that allows users to select their preferred coffee type (Espresso or Latte), choose the roast level (Light, Medium, Dark), and specify the number of coffees to brew. The application then calculates and returns the total cost of the coffee order.

This project leverages Object-Oriented Programming (OOP) principles, including inheritance, loops, user input handling, and **classes** to organize the code for clarity and reusability.

## Key Features:
- **Coffee Selection**: Choose between Espresso and Latte.
- **Roast Level Selection**: Choose from Light, Medium, or Dark roast.
- **Order Quantity**: Specify the number of coffees to brew.
- **Cost Calculation**: The system calculates the cost based on the selected coffee, roast level, and quantity.
- **Interactive User Interface**: The console-based application guides the user through their coffee order step by step.

## Project Structure
```
CoffeeMachine/
├── CoffeeMachine.java       (Main entry point)
├── Coffee.java             (Abstract base class for coffee types)
├── Espresso.java           (Espresso coffee implementation)
├── Latte.java              (Latte coffee implementation)
├── CoffeeMaker.java        (Handles brewing logic and cost calculations)
└── RoastLevel.java         (Enum for roast levels)
```

### Class Descriptions:

- **CoffeeMachine.java**: The main entry point of the application. This class contains the menu system and orchestrates the coffee selection process using user input.
- **Coffee.java**: An abstract base class that defines common properties and methods for all types of coffee, such as the base cost and brewing logic. This class provides a foundation for Espresso and Latte classes.
- **Espresso.java**: A subclass of `Coffee`, representing the Espresso coffee type, which overrides specific cost and brewing logic.
- **Latte.java**: A subclass of `Coffee`, representing the Latte coffee type, with its own specific cost and brewing logic.
- **CoffeeMaker.java**: A helper class responsible for handling the brewing process and calculating the final cost based on user inputs.
- **RoastLevel.java**: An enum that defines the available roast levels (Light, Medium, Dark).

### Object-Oriented Programming (OOP) & Class Usage:
- The project uses **classes** to encapsulate related data and behaviors, ensuring that each coffee type (Espresso, Latte) has its own class with methods specific to it, such as `brew()` and `calculateCost()`.
- The `Coffee` class is an **abstract class** that defines shared properties and methods for all coffee types, and **inheritance** is used to extend this class into `Espresso` and `Latte` for specific implementations.
- **Polymorphism** is employed in methods like `brew()` to allow different behavior in `Espresso` and `Latte` classes, while still adhering to a common interface.
- **Encapsulation**: Data related to the coffee type, roast level, and price are encapsulated within their respective classes, providing clear boundaries and easy maintenance.
  
## Requirements
- JDK 11 or higher to compile and run the project.

## How to Run

1. Clone or download the repository.
2. Open the project in your preferred IDE (e.g., IntelliJ IDEA, Eclipse) or navigate to the project directory in your terminal.
3. Compile the Java files:
   ```bash
   javac CoffeeMachine/*.java
   ```
4. Run the application:
   ```bash
   java CoffeeMachine.CoffeeMachine
   ```

## Usage

Upon running the application, you will be prompted with the following steps:

1. **Select Coffee Type**:
   - Choose between Espresso or Latte by entering the corresponding number.

2. **Select Roast Level**:
   - After selecting the coffee type, you will be asked to choose the roast level: Light, Medium, or Dark.

3. **Enter Quantity**:
   - Specify the number of coffees you wish to order.

4. **View Total Cost**:
   - The program will display the total cost of your order, taking into account the selected coffee, roast level, and quantity.

## Example Interaction:

```bash
Welcome to the Coffee Machine!
Select your coffee type:
1. Espresso
2. Latte
Enter your choice: 1

Choose the roast level:
1. Light
2. Medium
3. Dark
Enter your choice: 2

How many coffees would you like to order? 3

Your total cost is: $15.00
```

### Coffee Pricing:
- **Espresso**: $5.00 per coffee
- **Latte**: $6.00 per coffee

### Roast Level Pricing:
- **Light**: $0.00 additional
- **Medium**: $1.00 additional
- **Dark**: $1.50 additional

## Design & Implementation:

### Object-Oriented Programming (OOP):
The project makes use of OOP concepts such as:
- **Inheritance**: `Espresso` and `Latte` classes inherit from the `Coffee` base class, sharing common properties and behaviors while customizing specific implementations.
- **Polymorphism**: The `brew()` method is overridden in the subclasses (`Espresso` and `Latte`) to provide different brewing behaviors.
- **Encapsulation**: Coffee-related data (e.g., cost and roast level) is encapsulated in classes, protecting data integrity and providing methods to access or modify it.
- **Classes**: Each coffee type (Espresso, Latte) is represented by a distinct class, making it easy to extend the project with new types in the future.

### Loops:
The program uses loops to repeatedly prompt the user until they provide valid input, ensuring a smooth and user-friendly experience. This also includes prompting for the number of coffees to order and allowing users to retry if they make an invalid selection.

## Future Enhancements
- Add more coffee types (e.g., Cappuccino, Mocha, etc.).
- Implement ingredient tracking (e.g., coffee beans, milk, water).
- Add an option for custom coffee flavors or special instructions.
- Implement a graphical user interface (GUI) for a more interactive experience.

## License
This project is open-source and available under the MIT License.

---

Feel free to modify this as needed for your specific project requirements. If you have any questions or need further assistance, don't hesitate to ask!
```

This is the final `README.md` content. You can copy and paste this directly into your project's `README.md` file. Let me know if you need any more changes or additions!# CoffeeMachine
