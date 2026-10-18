
# Learnlog: A Web Platform for Academic Accountability

Learnlog is a full-stack web application developed as a school project to help students manage their academic responsibilities. The platform allows students to view assignments, track their progress, and stay accountable, while giving parents visibility into their children's academic progress and teachers tools to manage classes and assignments.

## Screenshots

<img width="585" height="328" alt="Screenshot 2026-10-18 at 2 17 53 PM" src="https://github.com/user-attachments/assets/6de6c78c-8913-472b-b657-ed4732a4b14b" />
<img width="585" height="328" alt="Screenshot 2026-10-18 at 2 17 45 PM" src="https://github.com/user-attachments/assets/f8894755-7b01-410e-a4bc-ff1409224778" />


## Features

- **Student Dashboard:** View assignments associated with enrolled classes.
- **Assignment Tracking:** Update assignment statuses to track progress.
- **Parent Access:** Allow parents to view their children's assignment statuses.
- **Class Management:** Enable teachers to create classes and allow students to join.
- **Assignment Management:** Allow teachers to create assignments for their classes.
- **Input Validation:** Validate user inputs during signup, class creation, and assignment creation.
- **Automated Testing:** Use PHPUnit to test application functionality and validate expected behavior.

## Tech Stack

- **Backend:** PHP,SQL
- **Dependency Management:** Composer
- **Testing Framework:** PHPUnit
- **Frontend:** HTML/CSS
- **Database:** Railway


## Testing Methodologies

Software testing was a major focus of this project. Multiple testing methodologies were used to evaluate application behavior, validate inputs, and maintain functionality throughout development.

### Test-Driven Development (TDD)

Used a test-driven approach extensively to validate inputs and application behavior, particularly during signup, class creation, and assignment creation.

### Equivalence Partitioning

Tested representative inputs from different equivalence classes to verify that valid inputs were accepted and invalid inputs were handled appropriately.

### Boundary Value Analysis and Edge Case Testing

Evaluated boundary conditions and unusual input scenarios to identify potential errors and ensure the application handled a variety of inputs reliably.

### Black-Box Testing

Tested major application features from the user's perspective to verify that the system behaved as expected without relying on its internal implementation.

### White-Box Testing

Tested internal functions and their interactions to help identify issues in application logic and integration.

### Regression Testing

Repeated previously implemented tests as new features were developed. For example, signup and login functionality was retested while class creation and assignment management were being implemented to help prevent regressions.

## Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

- PHP
- Composer
- Git
- The database software used by the project

Verify your PHP installation:

```bash
php -v
```

Verify Composer is installed:

```bash
composer --version
```

### Installation

**1. Clone the repository**

```bash
git clone <repository-url>
cd <project-directory>
```

Replace the placeholders with your repository URL and project directory.

**2. Install dependencies**

```bash
composer install
```

If PHPUnit is not already listed as a project dependency, install it as a development dependency:

```bash
composer require --dev phpunit/phpunit
```

**3. Configure the database**

Create a `config.php` file using `example.Config.php` as a reference:

```bash
cp example.Config.php config.php
```

Update the configuration values to match your local database credentials and settings. Do not commit credentials or other secrets to version control.

Ensure the database is running and any required database or schema setup has been completed before launching the application.

### Running the Application

Navigate to the `Public` directory and start PHP's built-in development server:

```bash
cd Public
php -S localhost:8000
```

Open the application in your browser:

http://localhost:8000

### Running Tests

From the project root, run the PHPUnit test suite:

```bash
vendor/bin/phpunit tests
```

This executes the tests located in the `tests` directory. If your project includes a PHPUnit configuration file, consult it for the expected test command and environment settings.

## Project Goals

Learnlog was designed to encourage academic accountability by connecting students, parents, and teachers through a shared platform. The project provided practical experience in full-stack web development, input validation, automated testing, and maintaining application reliability throughout iterative development.

## Key Takeaways

- Applied multiple software testing techniques to a full-stack web application.
- Practiced test-driven development and regression testing during feature implementation.
- Evaluated valid and invalid inputs using equivalence classes, boundary values, and edge cases.
- Tested application behavior from both user-facing and internal implementation perspectives.
- Gained experience with PHP, Composer, PHPUnit, and local development server configuration.




