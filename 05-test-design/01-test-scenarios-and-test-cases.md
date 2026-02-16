# 🧪 Test Scenarios and Test Cases
> A beginner-friendly guide explaining test scenarios, test cases, and core manual testing concepts with examples.


---
## 📑 Table of Contents

- [What is Test Scenario?](#-what-is-test-scenario)
- [What is Test Case?](#-what-is-test-case)
- [Test Scenario vs Test Case](#-test-scenario-vs-test-case)
- [Positive and Negative Testing](#-positive-and-negative-testing)
- [Boundary Value / Edge Case Testing](#-boundary-value--edge-case-testing)
- [How to Write a Good Test Case](#-how-to-write-a-good-test-case)
- [Best Practices](#-best-practices)
- [Common Mistakes to Avoid](#-common-mistakes-to-avoid)
- [Summary](#-summary)

## 📌 What is Test Scenario?

A **test scenario** is a high-level description of what needs to be tested in an application.  
It represents a user action or workflow derived from requirements or user stories.

### Characteristics
- High-level description
- Covers user workflows
- Derived from requirements/user stories
- One test scenario can produce multiple test cases

### Example

**Feature:** User Login

**Test Scenarios**
- User logs in with valid credentials
- User logs in with an invalid password
- User resets a forgotten password
- User login session timeout after inactivity

---

## 📌 What is Test Case?

A **test case** is a detailed step-by-step validation used to verify a specific scenario.

### Characteristics
- Contains detailed execution steps
- Includes input data
- Defines expected results
- Result can be measured as **Pass** or **Fail**

---

## 🔄 Test Scenario vs Test Case

| Aspect | Test Scenario | Test Case |
|--------|--------------|-----------|
| Level | High | Detailed |
| Purpose | What to test | How to test |
| Created by | QA Analyst | QA Engineer |
| Count | Few | Many |
| Example | Login functionality | Verify login with valid email |

---

## 🧪 Positive and Negative Testing

### ✅ Positive Testing

**Positive testing** verifies that the application works correctly when valid inputs are provided.

**Goal:** Confirm the system behaves as expected under normal conditions.

#### Examples (Login Feature)
- User logs in with valid email and password
- User enters correct OTP
- User submits a valid registration form

---

### ❌ Negative Testing

**Negative testing** verifies how the application behaves when invalid or unexpected inputs are provided.

**Goal:** Ensure the system handles errors gracefully and prevents invalid operations.

#### Examples (Login Feature)
- User enters incorrect password
- User leaves required fields empty
- User enters invalid email format
- User attempts login without internet connection

---

## 📏 Boundary Value / Edge Case Testing

### What is Boundary Value Testing?

**Boundary Value Testing** focuses on testing values at the limits of allowed input ranges because defects commonly occur at boundaries.

Systems often fail at minimum, maximum, or just outside valid limits.

---

### Example

**Password Length Requirement:** `8–16 characters`

| Test Type | Input Length | Expected Result |
|-----------|-------------|-----------------|
| Below Minimum | 7 | Error message |
| Minimum Boundary | 8 | Accepted |
| Valid Middle | 12 | Accepted |
| Maximum Boundary | 16 | Accepted |
| Above Maximum | 17 | Error message |

---

### Edge Case Testing

**Edge case testing** checks unusual, extreme, or unexpected situations that users might encounter.

#### Examples
- Very long input text
- Special characters or emojis
- Rapid multiple clicks on login button
- Session expiration during form submission
- Network interruption during payment

---

## ✍️ How to Write a Good Test Case

A good test case should be clear, reusable, and easy for anyone to execute without confusion.

---

### 🧩 Standard Test Case Structure

| Field | Description |
|------|-------------|
| Test Case ID | Unique identifier (e.g., TC_LOGIN_001) |
| Test Scenario | Related high-level scenario |
| Test Description | What is being verified |
| Preconditions | Required setup before execution |
| Test Steps | Step-by-step actions |
| Test Data | Input values used |
| Expected Result | Expected system behavior |
| Actual Result | Actual outcome after execution |
| Status | Pass / Fail |
| Priority | Importance of the test |
| Severity | Impact of failure |

---

### 🪜 Example Test Case

| Field | Value |
|------|-------|
| Test Case ID | TC_LOGIN_001 |
| Test Scenario | User Login |
| Description | Verify login with valid credentials |
| Preconditions | User account exists |
| Steps | 1. Open login page <br> 2. Enter valid email <br> 3. Enter password <br> 4. Click Login |
| Test Data | user@test.com / Password123 |
| Expected Result | User successfully logs into dashboard |
| Status | Not Executed |

---

## ✅ Best Practices

- Write clear and simple steps
- Use **one validation per test case**
- Keep steps concise and sequential
- Avoid ambiguity or assumptions
- Make test cases reusable
- Include both positive and negative scenarios
- Ensure expected results are measurable

---

## ❌ Common Mistakes to Avoid

- Writing vague steps (e.g., "Check login")
- Missing expected results
- Combining multiple validations in one test case
- Using unclear test data
- Skipping preconditions

---

## ✅ Summary

- **Test Scenario** → Defines *what* should be tested.
- **Test Case** → Defines *how* testing is performed.
- Multiple test cases are created from one test scenario.

---

## 👨‍💻 Author
Created as part of QA learning journey by Smrity Thapa.

