#SQL Injection Test Using Selenium WebDriver


##Overview
This Java program demonstrates how to perform a controlled SQL injection test on a sample web application login form using Selenium WebDriver. The test is conducted on the OWASP Juice Shop, a safe environment designed for security testing.

#Prerequisites
Java Development Kit (JDK) installed
Selenium WebDriver (Java bindings)
ChromeDriver (Ensure the path to ChromeDriver is set correctly)
Chrome browser installed

#Approach
Launching the Web Browser: The program uses Selenium WebDriver to open a Chrome browser and navigate to the OWASP Juice Shop login page.
Locating Elements: The username and password fields are located using the By.id locator method.
Crafting the SQL Injection Payload: A simple SQL injection payload (' OR '1'='1) is entered into the username field.
Form Submission: The form is submitted, and the program waits for a response.
Response Analysis: The program checks for any error messages that might indicate the success or failure of the SQL injection attempt.
Exception Handling
The program is designed to handle common exceptions, such as:

NoSuchElementException: Caught when an element is not found on the page.
General Exception Handling: All other exceptions are caught and logged to the console.
Running the Program
Ensure all dependencies are set up (JDK, Selenium, ChromeDriver).
Compile and run the Java program.
Assumptions
The login form is vulnerable to SQL injection.
The OWASP Juice Shop is being used in a controlled environment.
Conclusion
This program demonstrates a basic SQL injection test using Selenium WebDriver. It should be used only in safe, controlled environments, such as OWASP Juice Shop, for learning and educational purposes.
