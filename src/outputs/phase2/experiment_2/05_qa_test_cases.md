# Test Plan for Sprint 1 - Cropchain Project

## Overview
This test plan outlines the test cases for the user stories committed to Sprint 1 of the Cropchain project. Each test case is designed to validate the acceptance criteria defined in the user stories and ensure the functionality aligns with the requirements.

### User Stories Covered
- US-001: Farmer Account Creation
- US-002: Crop Listing by Farmer
- US-003: Restaurant Buyer Account Creation
- US-004: Grocery Buyer Account Creation
- US-005: Restaurant Buyer Crop Ordering
- US-006: Grocery Buyer Crop Ordering
- US-012: Alert Notifications for Delays and Shortages

---

## Test Cases

### User Story: US-001
**As a Farmer, I want to create an account so that I can list my crops.**

**Mapped Requirement:** REQ-001

| Test Case ID | Test Type   | Test Steps                                                                                     | Expected Result                                                                                     |
|--------------|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| TC-001-01    | Acceptance  | 1. Navigate to the registration page.<br>2. Enter valid email and password.<br>3. Submit form.| Farmer receives a confirmation email and can log in with the registered credentials.               |
| TC-001-02    | System      | 1. Attempt to register with an existing email.<br>2. Submit form.                           | System displays an error message indicating the email is already in use.                           |

### User Story: US-002
**As a Farmer, I want to list my crops so that buyers can see what I offer.**

**Mapped Requirement:** REQ-002

| Test Case ID | Test Type   | Test Steps                                                                                     | Expected Result                                                                                     |
|--------------|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| TC-002-01    | Acceptance  | 1. Log in as a farmer.<br>2. Navigate to the crop listing page.<br>3. Enter crop details (type, quantity, price).<br>4. Submit listing. | Crop is successfully listed and visible to buyers.                                                  |
| TC-002-02    | System      | 1. Log in as a farmer.<br>2. List a crop.<br>3. Edit crop details.<br>4. Save changes.      | Crop details are updated and reflect the changes made.                                            |

### User Story: US-003
**As a Restaurant Buyer, I want to create an account so that I can order crops.**

**Mapped Requirement:** REQ-003

| Test Case ID | Test Type   | Test Steps                                                                                     | Expected Result                                                                                     |
|--------------|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| TC-003-01    | Acceptance  | 1. Navigate to the registration page.<br>2. Enter valid email and password.<br>3. Submit form.| Buyer receives a confirmation email and can log in with the registered credentials.                |
| TC-003-02    | System      | 1. Attempt to register with an existing email.<br>2. Submit form.                           | System displays an error message indicating the email is already in use.                           |

### User Story: US-004
**As a Grocery Buyer, I want to create an account so that I can order crops.**

**Mapped Requirement:** REQ-004

| Test Case ID | Test Type   | Test Steps                                                                                     | Expected Result                                                                                     |
|--------------|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| TC-004-01    | Acceptance  | 1. Navigate to the registration page.<br>2. Enter valid email and password.<br>3. Submit form.| Buyer receives a confirmation email and can log in with the registered credentials.                |
| TC-004-02    | System      | 1. Attempt to register with an existing email.<br>2. Submit form.                           | System displays an error message indicating the email is already in use.                           |

### User Story: US-005
**As a Restaurant Buyer, I want to order crops directly from farmers so that I can manage my inventory.**

**Mapped Requirement:** REQ-005

| Test Case ID | Test Type   | Test Steps                                                                                     | Expected Result                                                                                     |
|--------------|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| TC-005-01    | Integration | 1. Log in as a restaurant buyer.<br>2. Browse available crops.<br>3. Select a crop and specify quantity.<br>4. Place an order. | Order is successfully placed, and buyer receives an order confirmation.                             |
| TC-005-02    | System      | 1. Log in as a restaurant buyer.<br>2. Attempt to order a crop with insufficient quantity.<br>3. Place order. | System displays an error message indicating insufficient stock for the selected crop.              |

### User Story: US-006
**As a Grocery Buyer, I want to order crops directly from farmers so that I can manage my inventory.**

**Mapped Requirement:** REQ-006

| Test Case ID | Test Type   | Test Steps                                                                                     | Expected Result                                                                                     |
|--------------|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| TC-006-01    | Integration | 1. Log in as a grocery buyer.<br>2. Browse available crops.<br>3. Select a crop and specify quantity.<br>4. Place an order. | Order is successfully placed, and buyer receives an order confirmation.                             |
| TC-006-02    | System      | 1. Log in as a grocery buyer.<br>2. Attempt to order a crop with insufficient quantity.<br>3. Place order. | System displays an error message indicating insufficient stock for the selected crop.              |

### User Story: US-012
**As an Actor, I want to receive alerts for delays and shortages so that I can take action.**

**Mapped Requirement:** REQ-012

| Test Case ID | Test Type   | Test Steps                                                                                     | Expected Result                                                                                     |
|--------------|-------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| TC-012-01    | System      | 1. Simulate a shipment delay.<br>2. Check alert notifications for all actors.                | All actors receive an alert via email or app notification regarding the shipment delay.            |
| TC-012-02    | System      | 1. Simulate a shortage of crops.<br>2. Check alert notifications for all actors.             | All actors receive an alert via email or app notification regarding the crop shortage.             |

---

## Summary
- **Total Test Cases Produced:** 15
- **Total Estimated QA Effort:** 8 days (15 test cases / 2 test cases per day)

### Confirmation of Acceptance Criteria
All acceptance criteria for each user story are testable as written, ensuring that the functionality aligns with the expectations set forth in the product backlog.

This structured test plan is ready for presentation to stakeholders and the QA team, ensuring clarity and alignment on the testing strategy for the Cropchain project.