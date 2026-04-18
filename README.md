# NopStore E-Commerce Store

NopStore is a sample e-commerce project built around the **nopCommerce** demo store (commonly used for UI automation / QA practice).  
This repository is structured as a **Java + Maven** project.

## Tech Stack
- Java
- Maven (`pom.xml`)
- (Optional/typical) Selenium WebDriver + TestNG/JUnit (depending on what you add in `pom.xml`)
- Eclipse project files included (`.project`, `.classpath`)

## Project Structure
- `src/` — source code (tests / utilities / page objects, etc.)
- `pom.xml` — Maven dependencies and build configuration
- `.settings/`, `.project`, `.classpath` — IDE configuration (Eclipse)

## Prerequisites
- Java (JDK 8+ recommended)
- Maven 3.6+
- (Optional) Chrome/Firefox + corresponding WebDriver if you run UI tests

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/mohan-1698/NopStore_E-Commerce-Store.git
   cd NopStore_E-Commerce-Store
   ```

2. Install dependencies:
   ```bash
   mvn clean install
   ```

## Running (examples)
Depending on how your tests are set up:

- Run all tests:
  ```bash
  mvn test
  ```

- Run a specific test class (example):
  ```bash
  mvn -Dtest=YourTestClassName test
  ```

## Configuration
If your project uses environment config (base URL, browser, credentials, etc.), document it here. Common options:
- `src/test/resources/config.properties`
- Maven system properties: `-DbaseUrl=... -Dbrowser=chrome`

Example:
```bash
mvn test -DbaseUrl=https://demo.nopcommerce.com -Dbrowser=chrome
```

## Notes
- If this is primarily a UI automation project, consider adding:
  - Page Object Model (POM) folder layout
  - Reporting (Allure / Extent Reports)
  - GitHub Actions CI workflow (`.github/workflows/...`)

## License
Add a license if you plan to share/reuse this project publicly (MIT, Apache-2.0, etc.).
