# IS601_M05

---

# Description

📌 Command-Line Calculator (Python)

This project is a modular, professional-grade command-line calculator application built in Python. It emphasizes clean architecture, error handling, testing, and continuous integration with GitHub Actions.

✨ Features

- REPL Interface: Interactive Read-Eval-Print Loop for continuous calculations.

- Arithmetic Operations: Addition, subtraction, multiplication, division, power, and modulo.

- Calculation Management: Uses a CalculationFactory to create calculation objects and maintains a history of operations.

- Special Commands: help, history, and exit for enhanced user experience.

- Robust Error Handling: Handles invalid input and division/modulo by zero gracefully.

🧩 Design Patterns Integration

🧱 Factory Pattern

- Creates operation objects dynamically based on user input via the OperationFactory, allowing easy extensibility for new operations.

🔄 Observer Pattern

- Implements observers to monitor and respond to calculator events such as logging calculation results and auto-saving history changes

🧠 Memento Pattern

- Adds undo and redo functionality by saving and restoring the application’s internal state (calculation history and last result).

🧮 Strategy Pattern

- Allows interchangeable strategies for operation execution — promoting flexible computation logic.

🪄 Facade Pattern

- Provides a simplified interface (Calculator class) that hides complexity from multiple subsystems (operations, observers, mementos, configuration, etc.).

📊 Data Management with pandas

- History Management: Utilizes pandas.DataFrame to store, filter, and manage calculation history in memory.

- Auto-Save & Load: Automatically saves history to CSV files and restores from existing history on startup.

⚙️ Configuration Management

- Uses .env files and the python-dotenv library to load configuration settings.

- Validates configuration and gracefully handles missing or invalid environment variables.

🧪 Testing

- Unit & Parameterized Tests with pytest for all components.

- 100% Test Coverage enforced via pytest-cov and GitHub Actions.

- Coverage Exceptions: Specific unreachable lines (e.g., pass, continue) marked with # pragma: no cover.

⚙️ CI/CD

- GitHub Actions workflow runs tests and checks coverage on every push/PR.

- Test coverage 100%.


# Getting Started

## Prequisites
- Install Python 3.10+
- Install Visual Studio Code

## Setup Instructions
- Clone Repo: `git clone git@github.com:kaw393939/module5_is601.git`
- Enter the directory: `cd module5_is601`
- Create Python Virtual Environment: `python -m venv venv`
- Activate Python Virtual Environment: `source venv/bin/activate`
- Install dependencies: `pip install -r requirements.txt`



## Executing program
- Run the tests: `pytest`
- Run the program:`python3 main.py`

# Authors

Maxiel De Jesus

# Version History

[https://github.com/MaxielDJ7/IS601_M04](https://github.com/MaxielDJ7/IS601_M04)

- Implement special commands help, history, and exit.
- Create calculation instances based on user input using CalculationFactory.
- Implement decorator design pattern.
- Achieve 100% test coverage.

[https://github.com/MaxielDJ7/IS601_M03](https://github.com/MaxielDJ7/IS601_M03)

- Implement REPL interface for continous user interaction.
- Input validation.
- Error handling.
- Apply the DRY principle.
- Implement parameterized tests.
- Push code and configuration to GitHub and ensure that GitHub Actions runs tests successfully.

[https://github.com/MaxielDJ7/IS601_M02](https://github.com/MaxielDJ7/IS601_M02)

- Simple calculator application that includes functions for addition, subtraction, multiplication, and division.
- Tests for each calculator function using `pytest`.
- Push code and configuration to GitHub and ensure that GitHub Actions runs tests successfully.

# Acknowledgements

Professor Keith Williams Github Repository: [https://github.com/kaw393939/module5_is601](https://github.com/kaw393939/module5_is601)