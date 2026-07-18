# Test Cases

This document contains the manual test cases executed for the **SauceDemo** web application. 

Each test case is designed to validate a specific feature, verify the expected functionality, and ensure that the application behaves correctly under different user scenarios.

## Objective
The objective of these test cases is to identify functional issues, validate user workflows, and maintain software quality through systematic testing. 

The execution status of each test case is recorded based on the observed results during testing.


## Test Case Summary
The table below showcases multiple Test-Cases and validates core functionalities of the **SauceDemo.**
| Test Case ID | Module | Test Scenario | Preconditions | Test Steps | Expected Result | Status |
|--------------|--------|---------------|---------------|------------|-----------------|--------|
| TC-001 | Login | Login with valid credentials | User is on login page | Enter valid username and password, then click **Login** | User is redirected to the Products page | Pass |
| TC-002 | Login | Login with invalid password | User is on login page | Enter valid username and incorrect password | Error message is displayed | Pass |
| TC-003 | Login | Login with empty username | User is on login page | Leave username blank and click **Login** | Validation/error message is displayed | Pass |
| TC-004 | Login | Login with empty password | User is on login page | Enter username, leave password blank, then click **Login** | Validation/error message is displayed | Pass |
| TC-005 | Login | Login with both fields empty | User is on login page | Leave username and password blank, then click **Login** | Validation/error message is displayed | Pass |
| TC-006 | Products | Verify product list loads | User is logged in | Navigate to the Products page | All products are displayed correctly | Pass |
| TC-007 | Products | Verify product images | User is logged in | Observe all product images | Images load successfully without distortion | Pass |
| TC-008 | Cart | Add a product to the cart | User is logged in | Click **Add to Cart** on any product | Product is added and cart badge updates | Pass |
| TC-009 | Cart | Remove a product from the cart | Product is already in the cart | Click **Remove** | Product is removed and cart badge updates | Pass |
| TC-010 | Cart | Open shopping cart | User has at least one item in cart | Click the cart icon | Cart page opens with selected products | Pass |
| TC-011 | Checkout | Start checkout | Product exists in cart | Click **Checkout** | Checkout Information page is displayed | Pass |
| TC-012 | Checkout | Submit checkout with missing details | User is on checkout page | Leave mandatory fields blank and click **Continue** | Appropriate validation message is displayed | Pass |
| TC-013 | Checkout | Complete checkout | Valid checkout information entered | Fill all required fields and finish checkout | Order confirmation page is displayed | Pass |
| TC-014 | Navigation | Verify menu functionality | User is logged in | Click the menu icon | Navigation menu opens successfully | Pass |
| TC-015 | Logout | Logout from the application | User is logged in | Open menu and click **Logout** | User is redirected to the login page | Pass |

## Conclusion

Based on the executed test cases, all tested functionalities of the SauceDemo application behaved as expected within the defined testing scope. 

No functional defects were identified during this testing cycle, indicating that the application's core features are stable and perform reliably under the tested conditions. 

Further testing across different environments and scenarios may reveal additional observations beyond the scope of this project.
