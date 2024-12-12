# Factorial Calculator Automation

## Project Description
This project demonstrates a basic automation script written in Java using Selenium WebDriver. The script performs the following tasks on the **Factorial Calculator** application available at https://qainterview.pythonanywhere.com/:

1. Launches the application in a browser.
2. Interacts with various elements like text boxes, buttons, and hyperlinks.
3. Validates the basic functionalities of the application, such as factorial calculation and navigation through different pages.
4. Ensures clean and proper closure of browser sessions.

## Key Features
- Automated browser interactions using Selenium WebDriver.
- Dynamic driver setup using **WebDriverManager** by Bonigarcia.
- Compatibility with Google Chrome browser.
- Implementation of best practices for handling browser sessions.

## Prerequisites
### Software Requirements
- **Java Development Kit (JDK)**: Version 8 or above.
- **Maven**: For dependency management.
- **Google Chrome**: Latest stable version.
- **IDE**: IntelliJ IDEA, Eclipse, or any Java-compatible IDE.

### Dependencies
- **Selenium WebDriver**: For browser automation.
- **WebDriverManager**: For automatic driver management.

## Installation and Setup
1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```

2. Open the project in your preferred IDE.

3. Ensure Maven is configured in your IDE. If not, install Maven and add it to your system PATH.

4. Add the following dependencies to the `pom.xml` file if not already present:
   ```xml
   <dependencies>
       <dependency>
           <groupId>org.seleniumhq.selenium</groupId>
           <artifactId>selenium-java</artifactId>
           <version>4.8.0</version>
       </dependency>
       <dependency>
           <groupId>io.github.bonigarcia</groupId>
           <artifactId>webdrivermanager</artifactId>
           <version>5.5.0</version>
       </dependency>
   </dependencies>
   ```

5. Build the project to download all dependencies:
   ```bash
   mvn clean install
   ```

6. Run the `FactorialCalculatorAutomation` class as a Java application.

## Usage
The script performs the following tasks:

1. **Launch the Application:**
   - Opens the URL `https://qainterview.pythonanywhere.com/` in Google Chrome.
   - Maximizes the browser window.

2. **Perform Factorial Calculation:**
   - Inputs the number `5` in the text box.
   - Clicks the **Calculate** button.
   - Verifies the result.

3. **Navigate Pages:**
   - Clicks the "About" link.
   - Navigates back to the home page.
   - Interacts with the "Terms and Conditions" and "Privacy" links.
   - Returns to the home page after each navigation.

4. **Handle Copyright Message:**
   - Interacts with the copyright message on the home page.

5. **Close the Browser:**
   - Ensures clean termination of the browser session.

## Project Structure
```
|-- src/main/java
|   |-- FactorialCalculatorAutomation.java  # Main automation script
|
|-- pom.xml  # Maven configuration file
```

## Best Practices Implemented
- **WebDriverManager:** Simplifies the setup and maintenance of browser drivers.
- **Thread.sleep():** Used to provide visibility during execution, though it can be replaced with explicit waits for production-level code.

## Troubleshooting
### Common Issues
1. **Browser Compatibility Issues:**
   - Ensure Google Chrome and ChromeDriver are updated to compatible versions.

2. **`Connection reset` Exception:**
   - Use the latest Selenium WebDriver and WebDriverManager.
   - Avoid terminating the browser session prematurely.

3. **Maven Dependency Errors:**
   - Verify the `pom.xml` file contains the correct dependencies.
   - Run `mvn clean install` to resolve dependencies.

## Contact
For further queries, reach out to:
- **Email:** [jogigoud95@gmail.com]
- **GitHub:** [ManideepJ-tech]

