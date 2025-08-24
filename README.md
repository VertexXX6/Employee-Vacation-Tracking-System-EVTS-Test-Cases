# Employee Vacation Tracking System (EVTS) Test Cases

## Overview
This repository contains test cases for validating the Employee Vacation Tracking System (EVTS) form, accessible at [JotForm](https://www.jotform.com/form/251503336577559). The test cases cover functional requirements (FR1–FR18), non-functional requirements (NFR1–NFR6), business rules (BR1–BR5), and use cases (US1–US6), ensuring the vacation request form meets user and system expectations.

The test cases validate:
- Core functionality (e.g., employee name, date selection, form submission).
- Input validations (e.g., date ranges, vacation allowance).
- UI/UX (e.g., responsiveness, accessibility).
- Security and compliance (e.g., GDPR, role-based access).

## Test Case Summary
- **Total Test Cases**: 34
- **Status**:
  - **Passed**: 6 (TC02, TC03, TC04, TC06, TC11, TC21)
  - **Failed**: 8 (TC01, TC05, TC07, TC08, TC09, TC10, TC28, TC33)
  - **Not Tested**: 20 (TC12–TC20, TC22–TC27, TC29–TC32, TC34)
- **Key Issues**:
  - Employee name not retrieved from database (TC01).
  - Incorrect vacation type options (TC05).
  - Missing validations for dates and allowance (TC07–TC10, TC28, TC33).
  - Limited access to Manager/HR Admin roles for testing critical features (TC12–TC20).

## Prerequisites
To execute these test cases:
1. **Access**:
   - Employee, Manager, and HR Admin accounts.
   - EVTS form: [https://www.jotform.com/form/251503336577559](https://www.jotform.com/form/251503336577559).
2. **Environment**:
   - Browsers: Chrome, Firefox, Safari.
   - Devices: Desktop, tablet, mobile.
3. **Data**:
   - Pre-configured employee data (e.g., 10 days vacation allowance).
   - Configured blocked periods.

## Test Case Structure
Each test case includes:
- **Test Case ID**: Unique identifier.
- **Requirement ID**: Linked requirements or use cases.
- **Test Case Title**: Test description.
- **Preconditions**: Setup requirements.
- **Test Steps**: Execution steps.
- **Expected Result**: Expected system behavior.
- **Actual Result**: Observed behavior.
- **Status**: Pass, Fail, or Not Tested.

## How to Use
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/[your-username]/evts-test-cases.git
   ```
2. **Review Test Cases**:
   - Check the test case file (`test_cases.xlsx`) for details.
   - Prioritize failed and not tested cases for action.
3. **Execute Tests**:
   - Access the EVTS form at [JotForm](https://www.jotform.com/form/251503336577559).
   - Follow the preconditions and test steps.
4. **Report Issues**:
   - Document failed cases with details (e.g., screenshots, environment).
   - Share findings with the development team for resolution.

## Key Issues and Recommendations
- **Database Issue (TC01)**: Verify database connection for employee name retrieval.
- **Vacation Type Mismatch (TC05)**: Align dropdown options with requirements.
- **Validation Errors (TC07–TC10, TC28, TC33)**: Add client/server-side validations.
- **Access Limitations (TC12–TC20, TC22–TC27, TC29–TC32)**: Request Manager/HR Admin access or simulate responses.
- **GDPR Compliance (TC23)**: Confirm data encryption and deletion processes.

## Contributing
- Fork the repository and submit pull requests for new test cases or updates.
- For bug reports, include:
  - Test Case ID
  - Steps to reproduce
  - Environment details

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
