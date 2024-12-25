# DemoBlaze-Project
This project is an automated testing framework for the DemoBlaze web application, implemented using Selenium WebDriver and Cucumber in a Page Object Model (POM) structure.
It automates critical workflows such as user sign-up, product addition, cart validation, amount calculations, and checkout processes.



# Table of Contents
1- Overview

2- Project Structure

3- Test Scenarios

4- Setup Instructions

5- Technologies Used

6- Execution

7- Reporting

8- Contributing

9- Author


# Overview
This automation project is designed to validate the functionality of the DemoBlaze website.
The framework leverages Cucumber for behavior-driven testing and Selenium for browser automation.
The code is structured following the Page Object Model (POM) for improved readability, maintainability, and reusability.


# Project Structure
The following is the directory structure of the project:

```

_**DemoBlaze/
│
├── resources/
│   └── Features/
│       ├── TC01_SignUp.feature
│       ├── TC02_Login.feature
│       ├── TC03_addProductToCart.feature
│       ├── TC04_CartValidation.feature
│       └── TC05_CheckOut.feature
│
└── test/
└── java/
├── Pages/
│   ├── L01_SignupLocators.java
│   ├── L02_LoginLocators.java
│   ├── L03_productLocators.java
│   ├── L04_cartValidation.java
│   ├── L05_CheckOutLocators.java
│   └── storeDetails.java
│
├── resources/
│   ├── extent.properties
│   ├── pdf-config.yaml
│   └── spark-config.xml
│
├── stepDefs/
│   ├── Hooks.java
│   ├── TC01_signUpSteps.java
│   ├── TC02_loginSteps.java
│   ├── TC03_productSteps.java
│   ├── TC04_cartValidation.java
│   └── TC05_CheckOutSteps.java
│
└── TestRunners/
└── runners.java

```



# Key Components
* Features: Contains Cucumber .feature files describing test scenarios in Gherkin syntax.
* Locators: Contains classes for element locators implementing the Page Object Model.
* StepDefinitions: Houses step definitions linked to feature files.
* Resources: Includes configuration files for reporting (ExtentReports, YAML, XML).
* TestRunners: Contains the runnerClass.java file to execute tests.


# Test Scenarios
The following scenarios are covered in this project:

* SingUp Functionality
  Verify that a user can successfully sign up on the DemoBlaze website.

* Login
  users could login with valid data.

* Add product to cart Functionality
  add the two products to cart.

* Cart Validation
  Validate that the product added on the cart with accurate details.

* Checkout Process
  Ensure that the user can successfully complete the purchase.



# Setup Instructions
*Prerequisites*

Ensure you have the following tools installed on your machine:

* *Java Development Kit (JDK):* Version 8 or higher.
* *Maven:* For dependency management.
* *IDE:* IntelliJ IDEA (recommended) or Eclipse.
* *Browser Drivers:* ChromeDriver (configured in system PATH).




# Technologies Used
* *Programming Language:* Java
* *Automation Framework:* Selenium WebDriver
* *Test Framework:* Cucumber
* *Build Tool:* Maven
* *Reporting:* ExtentReports (HTML & PDF)
* *IDE:* IntelliJ IDEA



# Execution

## *Run Tests Using Maven*

Execute the tests using the following Maven command:

`mvn test

*Run Tests from IDE*

1. Navigate to the runnerClass.java file in the TestRunners package.
2. Right-click and select Run.



# Reporting
Test execution reports are generated using *ExtentReports*.
The following report formats are supported:

1. *HTML Reports:* Detailed visual reports.
2. *PDF Reports:* Configurable via pdf-config.yaml.
   Reports will be saved in the target directory after test execution.



# Contributing
Contributions are welcome! If you would like to improve this project:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of the changes.



# Author
Developed by *Eng.Zeyad Kareem*.

For inquiries or collaboration, feel free to reach out:

*Email:* zeyadworkspace@gmail.com

*LinkedIn:* www.linkedin.com/in/zeyad-kareem-613675328







# Future Enhancements
* *Parallel Execution:* Implement parallel test execution using TestNG or Cucumber.
* *CI/CD Integration:* Integrate with Jenkins or GitHub Actions for automated test runs.
* *Data-Driven Testing:* Use external data sources (Excel, JSON).
* *Cross-Browser Testing:* Add support for Firefox and Edge browsers.


