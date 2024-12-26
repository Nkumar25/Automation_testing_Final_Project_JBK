# Automation_testing_Final_Project_JBK
This Java project demonstrates a basic framework for automated testing of a web application's login functionality. It utilizes Selenium WebDriver for browser interaction, TestNG for test execution and management, and Apache POI for reading test data from an Excel spreadsheet.

Key Components:

    BaseClass: Provides common setup and teardown methods, including browser initialization and closing.
    LoginPage: Represents the login page of the application. It uses Page Object Model (POM) design with @FindBy annotations to locate web elements (email field, password field, sign-in button, etc.).
    LoginTestCase: Contains the main test logic. It uses the @Test annotation with a dataProvider to execute the test multiple times with different sets of login credentials.
    LoginTestData: Reads login credentials (username and password) from an Excel spreadsheet using Apache POI library.
    Data-Driven Testing: The project implements data-driven testing by reading test data from an external source (Excel sheet), making the tests more flexible and maintainable.

Functionality:

    Login Test Cases: The LoginTestCase executes multiple login attempts with different credentials read from the Excel sheet.
    Data-Driven Approach: Reads test data from an Excel sheet, enabling easy modification of test data without changing the code.
    Page Object Model: Uses POM for better code organization, maintainability, and reusability.

Limitations:

    Basic Functionality: The current implementation only covers basic login functionality.
    Limited Error Handling: The error handling is basic and can be improved.
    Missing Assertions: The email() and password() methods in LoginPage are not fully implemented, and their assertions are missing.

Further Improvements:

    Implement robust error handling for invalid login attempts.
    Add more comprehensive assertions to verify expected behavior after successful/failed logins.
    Extend the framework to include other test cases such as registration, password recovery, etc.
    Integrate with a reporting framework for better test results visualization.

This project serves as a foundation for building more complex and comprehensive automated testing suites for web applications.
