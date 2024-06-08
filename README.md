# Magical Arena

This is a simple Java implementation of the Magical Arena game using the Strategy Design Pattern.

## Requirements

- Java Development Kit (JDK)
- JUnit 4

## Project Structure

- `SwiggyBackEndAssignment1/src/GameAssignment`: Contains the main source code.
- `SwiggyBackEndAssignment1/src/GameAssignment/UnitTestCase`: Contains Unit Test cases.

## How to Build and Run

To build and run the game using IntelliJ, follow these steps:

1. Open IntelliJ IDEA.
2. Click on "File" -> "Open".
3. Navigate to the directory `SwiggyBackEndAssignment1`.
4. Once the project is imported, locate the `Main.java` file inside `src/GameAssignment`.
5. Right-click on `Main.java` and select "Run Main.main()".

## How to Play

1. Create two players with initial attributes (name, health, strength, attack):
    ```java
    Player playerA = new Player("A", 50, 5, 10);
    Player playerB = new Player("B", 100, 10, 5);
    ```

2. Create an object of `MagicalArena`:
    ```java
    MagicalArena arena = new MagicalArena(playerA, playerB);
    ```

3. If you want to play with your own strategy, create a new class implementing the `CombatStrategy` interface. Then create an object of this class and call the `setCombatStrategy()` method in `MagicalArena`.

4. Call the `startBattle()` method present inside the `MagicalArena`:
    ```java
    arena.startBattle();
    ```

## Unit Tests

Unit tests are provided to ensure the correctness of the code. JUnit 4 and Hamcrest libraries are used for testing.

### Steps to Run Unit Tests

1. Navigate to the `SwiggyBackEndAssignment1/src/GameAssignment/UnitTestCase` directory in the project.
2. Right-click on the test class name `MagicalArenaTest.java`.
3. Select "Run 'MagicalArenaTest'" from the context menu.
4. View the test results in the "Run" tool window.
