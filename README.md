# PROG6112-Exam
Mattress Sales Application - Exam Project
This repository contains the completed Java solutions for Questions 1 and 2 of the examination. The project consists of a console-based application for generating sales reports and a Graphical User Interface (GUI) application for processing customer sales, calculating VAT/Commission, and logging data to a file.

🛠️ Prerequisites
Java Development Kit (JDK): Version 8 or higher.

IDE: NetBeans (Recommended, as the project was built using it), Eclipse, or IntelliJ IDEA.

JUnit: The project includes Unit Tests using JUnit 4/5.

📂 Project Structure
The project is organized into a single package (com.mattressapp) containing the following files:

Question 1: Console Application
IProduct.java: The interface defining the required calculation methods.

Product.java: Implements IProduct. It utilizes a 1D array (for product names) and a 2D array (for 3 months of sales data) to calculate total sales, average sales, and the most popular product.

PrintProduct.java: A dedicated class responsible for formatting and printing the output to the console.

MainApp.java: The entry point for the console application. It handles user input via the Scanner class and displays the generated report.

Question 2: GUI Application
IProductCalculations.java: The interface defining the VAT, Commission, and Total calculation methods.

ProductCalculations.java: Implements IProductCalculations. Calculates 15% VAT, 5% Commission, and the final Total.

ProductApp.java: The entry point for the GUI application (built with Java Swing). It includes text fields, a combo box for product selection, a menu bar, event handling for the "PROCESS" button, and file I/O logic to save data to data.txt.

Testing
ProductTest.java: Contains Unit Tests for Question 1 (verifying GetTotalProductsSold and GetAverageProductSold).

ProductCalculationsTest.java: Contains Unit Tests for Question 2 (verifying GetVat and GetTotal).

🚀 How to Run the Applications
Running Question 1 (Console App)
Open the project in your IDE.

In the Project Explorer, navigate to Source Packages -> com.mattressapp.

Right-click on MainApp.java and select Run File (or press Shift + F6 in NetBeans).

Enter the sales data in the console as prompted.

Running Question 2 (GUI App)
In the Project Explorer, navigate to Source Packages -> com.mattressapp.

Right-click on ProductApp.java and select Run File (or press Shift + F6 in NetBeans).

The GUI window will open.

Note: If you press the main "Run Project" button, ensure the project properties are set to run ProductApp as the Main Class (Right-click Project -> Properties -> Run -> Main Class).

🧪 How to Run the Unit Tests
If you are using NetBeans:

Navigate to the Test Packages folder in your project.

Right-click on ProductTest.java and select Run File to test Question 1.

Right-click on ProductCalculationsTest.java and select Run File to test Question 2.

The output window will display the test results (expected: 100% pass rate).

If you encounter errors with @Test annotations, ensure JUnit is added to your project libraries (Right-click Libraries -> Add Library -> JUnit).

📄 File Output (Question 2)
When a sale is processed in the GUI application, the data is automatically appended to a file named data.txt.

This file will be generated in the root directory of the project (e.g., alongside the build, src, and nbproject folders). If the file does not exist, the application will create it automatically.
