# 🥒 OpenCart Cucumber BDD Framework

A **Behavior-Driven Development (BDD)** test automation framework for the **OpenCart e-commerce platform** using **Cucumber** with Java, Selenium, and Page Object Model.

---

## 📖 Overview

This project implements BDD testing for OpenCart using Gherkin feature files, Cucumber step definitions, and the Page Object Model pattern. It supports data-driven testing via Excel, automated reporting with Extent Reports, and cross-browser testing.

---

## ✅ Test Scenarios (Feature Files)

| Feature | Description |
|---------|-------------|
| **Registration.feature** | Account registration flow |
| **Login.feature** | Login with valid credentials |
| **LoginDDTExcel.feature** | Data-driven login testing via Excel |

---

## 📂 Project Structure

```
opencart_Cucumber/
├── pom.xml
├── Features/                           # Gherkin feature files
│   ├── Registration.feature
│   ├── Login.feature
│   └── LoginDDTExcel.feature
├── src/test/java/
│   ├── factory/
│   │   └── BaseClass.java             # WebDriver factory & setup
│   ├── pageObjects/                    # Page Object Model classes
│   │   ├── BasePage.java
│   │   ├── HomePage.java
│   │   ├── LoginPage.java
│   │   ├── AccountRegistrationPage.java
│   │   ├── MyAccountPage.java
│   │   ├── SearchPage.java
│   │   ├── ShoppingCartPage.java
│   │   └── CheckoutPage.java
│   ├── stepDefinitions/                # Cucumber step implementations
│   │   ├── Hooks.java                 # Before/After hooks
│   │   ├── LoginSteps.java
│   │   └── RegistrationSteps.java
│   ├── testRunner/
│   │   └── TestRunner.java            # Cucumber test runner
│   └── utilities/
│       └── DataReader.java            # Excel data reader
└── src/test/resources/
    ├── config.properties               # Environment config
    ├── extent.properties               # Extent Reports config
    └── log4j2.xml                      # Logging config
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| **Java** | Programming language |
| **Cucumber** | BDD framework with Gherkin |
| **Selenium WebDriver** | Browser automation |
| **Page Object Model** | Design pattern |
| **TestNG** | Test runner |
| **Extent Reports** | HTML reporting |
| **Apache POI** | Excel data-driven testing |
| **Log4j2** | Logging |
| **Maven** | Build management |

---

## 🚀 Getting Started

### Prerequisites
- Java JDK 11+
- Maven 3.x
- Chrome / Firefox browser

### Installation
```bash
git clone https://github.com/Shubham00117/opencart_Cucumber.git
cd opencart_Cucumber
mvn clean install
```

### Running Tests
```bash
# Run via TestRunner
mvn test

# Run specific feature
mvn test -Dcucumber.features=Features/Login.feature
```

---

## 📜 License

This project is open source and available for educational purposes.
