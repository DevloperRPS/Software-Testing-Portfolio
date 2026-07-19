# Test Cases

This document contains the manual test cases executed for the [OrangeHRM demo application.](https://opensource-demo.orangehrmlive.com/web/index.php/admin/viewSystemUsers) 

The testing focused on validating the application's core functionality, user interface, navigation, and user workflows through systematic manual testing.

## Objective

The objective of this testing activity was to verify that the major modules of the [OrangeHRM application](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login) function according to the expected requirements. 

The testing also aimed to identify functional issues, validate user interactions, and document the overall application behavior.


## Testing Scope

<img width="1920" height="1003" alt="orangehrm-website-dashboard-screenshot-showing-all-modules-for-qa-testing" src="https://github.com/user-attachments/assets/2f78ed7b-6cb7-4416-9186-368ec9c19e85" />

The following modules were included in this testing cycle:

- Login & Authentication
- Dashboard
- Admin Module
- Upgrade Options
- Dashboard
- Leave Management
- Navigation
- User Interface
- Logout


## Testing Approach

Manual functional testing was performed by executing each test scenario independently and comparing the observed behavior with the expected outcome. 

During exploratory testing, one temporary loading issue was observed in the Leave module. After refreshing the page, the module loaded successfully and the issue could not be reproduced consistently. Therefore, it has been recorded as an observation rather than a confirmed defect.


## Manual Test Cases

<img width="1920" height="1003" alt="orangehrm-upgrade-options-module-with-no-price-options-shown-in-qa-testing" src="https://github.com/user-attachments/assets/bfb47dfa-dddc-4434-a997-8e343abe695f" />


| TC ID | Module | Test Scenario | Expected Result | Actual Result | Status |
|------|---------|---------------|-----------------|---------------|--------|
| TC-001 | Login | Login with valid credentials | Dashboard should load successfully | Dashboard loaded successfully | Pass |
| TC-002 | Login | Login with invalid username | Error message displayed | Error displayed | Pass |
| TC-003 | Login | Login with invalid password | Error message displayed | Error displayed | Pass |
| TC-004 | Login | Login with empty username | Validation message displayed | Validation displayed | Pass |
| TC-005 | Login | Login with empty password | Validation message displayed | Validation displayed | Pass |
| TC-006 | Dashboard | Verify dashboard loading | Dashboard loads correctly | Loaded successfully | Pass |
| TC-007 | Navigation | Verify sidebar navigation | Selected module opens | Working correctly | Pass |
| TC-008 | Admin | Open Admin module | Admin page loads | Loaded successfully | Pass |
| TC-009 | Admin | Search existing user | User displayed | Search successful | Pass |
| TC-010 | Admin | Reset search filters | Filters cleared | Working correctly | Pass |
| TC-011 | Leave | Open Leave module | Leave page loads | Initial loading issue observed; loaded after refresh | Observation |
| TC-012 | Leave | Navigate Leave options | Options accessible | Working correctly | Pass |
| TC-013 | PIM | Open Employee List | Employee list displayed | Displayed successfully | Pass |
| TC-014 | PIM | Search employee | Matching employee shown | Working correctly | Pass |
| TC-015 | PIM | Attempt employee deletion | Employee deleted (if permitted) | Delete action unavailable/unsuccessful | Observation |
| TC-016 | UI | Verify page responsiveness | Layout remains consistent | Layout consistent | Pass |
| TC-017 | UI | Verify buttons and links | All controls respond | Functional with slight delay in some CTA actions | Observation |
| TC-018 | Forms | Enter employee details | Input accepted correctly | Characters occasionally disappeared while typing | Observation |
| TC-019 | Dashboard | Verify widgets | Widgets displayed correctly | Working correctly | Pass |
| TC-020 | Upgrade | Select Upgrade option | Pricing details displayed | Price information not displayed | Observation |
| TC-021 | Navigation | Verify breadcrumbs | Breadcrumb navigation works | Working correctly | Pass |
| TC-022 | Session | Refresh page after login | Session remains active | Working correctly | Pass |
| TC-023 | Session | Logout | User redirected to login page | Logout successful | Pass |
| TC-024 | UX | Evaluate overall user experience | Smooth and responsive interaction | Minor lag observed during navigation and interactions | Observation |
| TC-025 | General | Verify overall application stability | Stable application behavior | Stable with minor non-reproducible observations | Pass |
## Observation

During exploratory testing, the Leave module remained in a loading state on one occasion. 

Refreshing the page resolved the issue, and it could not be reproduced consistently during subsequent testing. 

Based on this behavior, the observation has not been classified as a confirmed software defect.

## Conclusion

The manual testing process covered the core functionalities of the OrangeHRM web application, including authentication, navigation, administrative features, employee management, and leave management. 

Most test cases produced the expected results, indicating that the application's primary functionality is stable.

During exploratory testing, a few observations related to user experience and application behavior were identified, including an intermittent loading issue in the Leave module, the absence of pricing information in the Upgrade section, minor interface lag, and occasional inconsistencies while entering text. 

These observations require further verification to determine whether they represent reproducible software defects or environment-specific behavior.

Overall, the testing cycle provided a comprehensive assessment of the application's functionality and served as a foundation for preparing the test summary and tool-based quality assessment reports.
