# SLF4J Logging Exercises

This repository demonstrates logging in Java using **SLF4J** and **Logback**.

## Technologies Used

- Java 21
- Maven
- SLF4J
- Logback
- IntelliJ IDEA

## Project Structure

```
src
├── main
│   ├── java
│   │   └── com/example/logging
│   │       ├── LoggingExample.java
│   │       ├── ParameterizedLogging.java
│   │       └── AppenderLogging.java
│   └── resources
│       └── logback.xml
```

## Exercises

### Exercise 1 – Error and Warning Logging

```java
logger.error("This is an error message");
logger.warn("This is a warning message");
```

Output

```
ERROR This is an error message
WARN This is a warning message
```

---

### Exercise 2 – Parameterized Logging

```java
logger.info("Student Name: {}", name);
logger.info("Age: {}", age);
logger.info("Marks: {}", marks);
```

Output

```
INFO Student Name: Ashwin
INFO Age: 20
INFO Marks: 89.5
```

---

### Exercise 3 – Using Different Appenders

Configured Logback with:

- Console Appender
- File Appender

Example

```java
logger.debug("Debug Message");
logger.info("Information Message");
logger.warn("Warning Message");
logger.error("Error Message");
```

The logs are displayed on the console and written to:

```
app.log
```

## Run the Project

```bash
mvn compile
mvn exec:java
```

or simply run the Java classes from IntelliJ IDEA.

## Learning Outcomes

- Configure SLF4J
- Configure Logback
- Log messages at different levels
- Use parameterized logging
- Configure console and file appenders
