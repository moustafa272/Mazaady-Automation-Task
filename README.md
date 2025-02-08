# Mazaady Portal Testing Task

**Objective:**

The objective of this task is to check the coding techniques, quality, and testing methods used in automating the Mazaady portal's login and product addition functionalities.

**Requirements:**

An automation script was developed to perform the following:

1.  Login:  Using the credentials:
    *   Email: `tester@task.com`
    *   Password: `*********`
    *   URL: `https://staging.mazaady.com/login`

2.  Add Product:  The script automates the process of adding a single product, including:
    *   Navigating through the profile menu to access the "add product" section.
    *   Filling in all required elements in the product creation form, which includes:
        *   Main image upload.
        *   Auction details (title, description, etc.).
        *   Policy information.
    *   Selecting the selling type (estimation value).  The following validations are performed:
        *   Buy Now value must be greater than Start Bid.
        *   Estimation value must be less than or equal to Buy Now value.
    *   Choosing one type of auction show type.

**Business Requirements:**

The automation script simulates the user flow of adding a product by selecting it from the profile picture menu.  All required fields for a single product creation are filled.  The script ensures data integrity by validating the Buy Now and Estimation values.

**Acceptance Criteria:**

*   Selenium (or a similar framework) was used for UI automation.
*   Data-driven testing was implemented to manage test data efficiently.
*   The Page Object Model (POM) design pattern was utilized for maintainable code structure.
*   Soft assertions were used to ensure comprehensive test execution and reporting.

**Output:**

1.  A detailed report of the scenario execution, including pass/fail status and any error messages. (The report can be found in the `target/surefire-reports` directory after running tests with Maven.)
2.  This Git repository containing the complete project code.
