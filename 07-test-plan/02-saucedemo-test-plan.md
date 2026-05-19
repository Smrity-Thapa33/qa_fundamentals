# 🧪 Test Plan – SauceDemo Web Application

## 📑 Table of Contents

1. [Introduction](#introduction)
2. [Objectives](#-objectives)
3. [Application Overview](#-application-overview)
4. [Scope of Testing](#-scope-of-testing)
5. [Test Strategy Overview](#test-strategy-overview)
6. [Testing Types](#-testing-types)
7. [Modules Covered](#modules-covered)
8. [Test Environment](#-test-environment)
9. [Test Deliverables](#-test-deliverables)
10. [Defect Management Process](#-defect-management-process)
11. [Entry Criteria](#entry-criteria)
12. [Exit Criteria](#exit-criteria)
13. [Risks & Limitations](#risks--limitations)
14. [Future Improvements](#-future-improvements)
15. [Conclusion](#conclusion)

---

# Introduction

This Test Plan describes the testing approach, scope, objectives, environment, and deliverables for manual testing of the SauceDemo web application.

The primary purpose of this testing activity is to validate core business functionalities, identify defects, and maintain structured QA documentation through test cases, bug reports, and testing evidence.

Application Under Test:  
https://www.saucedemo.com/

---

# 🎯 Objectives

The main objectives of this testing process are:

- Validate major user workflows
- Verify application functionality
- Identify UI and functional defects
- Detect inconsistent application behavior
- Practice structured bug reporting
- Improve manual testing skills
- Maintain professional QA documentation

---

# 🌐 Application Overview

SauceDemo is a demo e-commerce web application commonly used for software testing and automation practice.

The application contains modules such as:

- Login
- Product Inventory
- Cart
- Checkout
- Navigation
- Product Sorting

The platform also includes special test users such as:

- `standard_user`
- `locked_out_user`
- `problem_user`
- `performance_glitch_user`

These users help testers identify different application behaviors and edge cases.

---

# 📂 Scope of Testing

## ✅ In Scope

The following functionalities are included in testing:

### 🔐 Login Module
- Valid login
- Invalid login
- Empty field validation
- Locked user validation
- Error message validation

### 📦 Inventory Module
- Product display
- Product sorting
- Product detail navigation
- Add to cart functionality

### 🛒 Cart Module
- Add/remove items
- Cart badge validation
- Cart persistence
- Multiple item handling

### 💳 Checkout Module
- Checkout information form
- Required field validation
- Checkout overview
- Order completion

### 🎨 UI Validation
- Button visibility
- Navigation consistency
- Error message display
- Layout consistency

---

## ❌ Out of Scope

The following testing activities are excluded:

- Automation Testing
- API Testing
- Security Testing
- Performance Testing
- Database Testing
- Mobile Device Testing

---

# Test Strategy Overview

Testing is performed using a manual testing approach based on:

- Requirement understanding
- User workflow validation
- Positive and negative test scenarios
- Exploratory testing
- Functional validation
- UI behavior validation

Testing is conducted module-wise to maintain organized documentation and defect tracking.

Special focus is given to:
- validation messages
- inconsistent UI behavior
- cart state management
- checkout validations
- edge-case scenarios

---

# 🧪 Testing Types

The following testing types are performed:

- Functional Testing
- UI Testing
- Smoke Testing
- Exploratory Testing
- Regression Testing (basic)
- Positive Testing
- Negative Testing

---

# Modules Covered

| Module | Description |
|---|---|
| Login | Authentication and validation |
| Inventory | Product listing and interactions |
| Cart | Cart operations and validations |
| Checkout | Checkout workflow and form validation |
| Navigation | Menu and page transitions |
| UI Validation | Layout and visual behavior |

---

# 🌐 Test Environment

| Component | Details |
|---|---|
| Application | SauceDemo |
| URL | https://www.saucedemo.com/ |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Testing Type | Manual Testing |

---

# 📋 Test Deliverables

The following QA artifacts are maintained:

- Test Scenarios
- Test Cases
- Bug Reports
- Screenshots
- Excel Documentation
- Markdown Documentation

---

# 🐞 Defect Management Process

Defects identified during testing are documented using structured bug reports containing:

- Bug ID
- Bug Summary
- Environment
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Screenshots

Example defects identified during testing include:

- Incorrect validation messages
- Cart inconsistencies
- Checkout validation issues
- UI behavior inconsistencies
- State-related functionality problems

Bug reports are maintained in the `06-bug-reports` section of the repository. :contentReference[oaicite:1]{index=1}

---

# Entry Criteria

Testing begins when:

- Application is accessible
- Test environment is ready
- Test data is available
- Test scenarios are prepared

---

# Exit Criteria

Testing is considered complete when:

- Planned test cases are executed
- Critical defects are documented
- Major workflows are validated
- QA documentation is updated

---

# Risks & Limitations

- Limited browser coverage
- Manual testing only
- No automation support currently
- No backend/database validation
- Limited cross-device testing

---

# 📈 Future Improvements

Future enhancements may include:

- API Testing
- Postman Collections
- Automation Testing
- Jira Workflow Practice
- Cross-browser Testing
- Advanced Regression Testing
- Selenium-based Automation Framework

---

# Conclusion

This Test Plan provides a structured framework for manually testing the SauceDemo web application while maintaining professional QA documentation practices.

The project focuses on practical manual testing skills including:
- test design
- defect identification
- bug reporting
- documentation
- exploratory testing
- workflow validation

The repository will continue evolving with additional QA concepts, testing practices, and automation learning.

---
## 👨‍💻 Author
Created as part of QA learning journey by Smrity Thapa.