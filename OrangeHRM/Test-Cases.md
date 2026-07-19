# Test Cases

This document contains the manual test cases executed for the OrangeHRM demo application. 

The testing focused on validating the application's core functionality, user interface, navigation, and user workflows through systematic manual testing.

## Objective

The objective of this testing activity was to verify that the major modules of the OrangeHRM application function according to the expected requirements. 

The testing also aimed to identify functional issues, validate user interactions, and document the overall application behavior.


## Testing Scope

The following modules were included in this testing cycle:

- Login & Authentication
- Dashboard
- Admin Module
- Leave Management
- Navigation
- User Interface
- Logout


## Testing Approach

Manual functional testing was performed by executing each test scenario independently and comparing the observed behavior with the expected outcome. 

During exploratory testing, one temporary loading issue was observed in the Leave module. After refreshing the page, the module loaded successfully and the issue could not be reproduced consistently. Therefore, it has been recorded as an observation rather than a confirmed defect.


## Manual Test Cases

| TC ID | Module | Test Scenario | Expected Result | Actual Result | Status |
|------|---------|---------------|-----------------|---------------|--------|
| TC-001 | Login | Login with valid credentials | Dashboard should open successfully | Dashboard opened successfully | Pass |
| TC-002 | Login | Login with invalid username | Error message should appear | Error message displayed | Pass |
| TC-003 | Login | Login with invalid password | Error message should appear | Error message displayed | Pass |
| TC-004 | Login | Login with empty credentials | Validation message displayed | Validation worked correctly | Pass |
| TC-005 | Dashboard | Dashboard loads after login | Dashboard displayed | Displayed successfully | Pass |
| TC-006 | Navigation | Sidebar navigation | Selected module opens | Working correctly | Pass |
| TC-007 | Admin | Open Admin module | Admin page loads | Loaded successfully | Pass |
| TC-008 | Admin | Search existing user | Matching user displayed | Search worked correctly | Pass |
| TC-009 | Admin | Reset search filters | Filters reset | Working correctly | Pass |
| TC-010 | Leave | Open Leave module | Leave page opens | Initial loading delay observed; loaded successfully after refresh | Pass* |
| TC-011 | Leave | Navigate inside Leave module | All sections accessible | Working correctly | Pass |
| TC-012 | UI | Verify page layout | Proper layout displayed | Layout displayed correctly | Pass |
| TC-013 | UI | Verify buttons | Buttons respond correctly | Working correctly | Pass |
| TC-014 | Forms | Required field validation | Validation messages displayed | Validation worked correctly | Pass |
| TC-015 | Session | Logout | User redirected to Login page | Logout successful | Pass |


## Observation

During exploratory testing, the Leave module remained in a loading state on one occasion. 

Refreshing the page resolved the issue, and it could not be reproduced consistently during subsequent testing. 

Based on this behavior, the observation has not been classified as a confirmed software defect.

## Conclusion

The manual testing process covered the primary functionalities of the OrangeHRM application. 

All planned test cases were executed successfully, and the application behaved as expected within the defined testing scope. 

Apart from a single non-reproducible loading observation in the Leave module, no confirmed functional defects were identified during this testing cycle.
