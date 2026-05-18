# JPetStore - Sign In Page Test Cases

📥 **Excel Version:**  
[JPETSTORE_Signin_page_TestCases.xlsx](./JPETSTORE_Signin_page_TestCases.xlsx)

---

## Module
Signin / User Login

## Application
JPetStore Demo Application

## Objective
To validate UI elements, login validations, authentication behavior, error handling, and successful login functionality of the Sign In page.

---

## Test Cases

| Test Case ID | Test Case Name | Test Scenarios | Pre-condition | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC_S01 | Sign In page Display | To validate the Sign In page is displayed to the user | User opens JPetStore application URL | Manual | 1. Open JPetStore application | Sign In page is displayed successfully |  | Not Executed | High |
| TC_S02 | Logo visibility | To validate JPET Store logo is displayed on the Sign In page | User is on the Sign In page | Manual | 1. Observe top section of Sign In page | JPET Store logo is visible |  | Not Executed | Low |
| TC_S03 | Navigation Links Display | To validate top navigation links (Fish, Dogs, Reptiles, Cats, Birds) are displayed | Sign In page is open | Manual | 1. Observe top navigation bar | Fish, Dogs, Reptiles, Cats, Birds links shown |  | Not Executed | Low |
| TC_S04 | Instructional Text Display | To validate instructional text “Please enter your username and password” is displayed | Sign In page is open | Manual | 1. Observe instructional text section | Text “Please enter your username and password” displayed |  | Not Executed | High |
| TC_S05 | Username & Password Fields Display | To validate Username and Password fields are displayed | Sign In page is open | Manual | 1. Observe Username and Password fields | Username and Password fields visible |  | Not Executed | High |
| TC_S06 | Valid Input in Fields | To validate Username field and Password Field accept valid input | Sign In page is open | Manual | 1. Enter valid username<br>2. Enter valid password | System allows valid entries |  | Not Executed | High |
| TC_S07 | Blank Field Validation | To validate Username field and Password field do not accept blank value | Sign In page is open | Manual | 1. Leave fields blank<br>2. Click login | Fields do not accept blank submission |  | Not Executed | High |
| TC_S08 | Empty Field Error Message | To validate the error message is displayed when Username and Password fields are empty | Sign In page is open | Manual | 1. Submit form without entering credentials | Proper error message displayed |  | Not Executed | High |
| TC_S09 | Password security in page source | To validate that password is not visible in page source | Sign In page is open | Manual | 1. Enter password<br>2. Inspect page source | Password is not visible in page source |  | Not Executed | High |
| TC_S10 | Username Alphanumeric validation | To validate that Username field accepts alphanumeric values | Sign In page is open | Manual | 1. Enter alphanumeric username | Alphanumeric usernames accepted |  | Not Executed | High |
| TC_S11 | Login Button display | To validate Login button is displayed | Sign In page is open | Manual | 1. Observe Login button | Login button visible |  | Not Executed | High |
| TC_S12 | Register Link Display | To validate “Register Now!” link is displayed | Sign In page is open | Manual | 1. Observe Register Now link | “Register Now!” link visible |  | Not Executed | High |
| TC_S13 | Successful login | To validate login with valid username and password | User account exists | Manual | 1. Enter valid credentials<br>2. Click login | User logged in successfully |  | Not Executed | High |
| TC_S14 | Logout functionality | To validate user is logged out successfully when Logout is clicked | User must be logged in | Manual | 1. Click Logout button | User logged out and redirected to Sign In page |  | Not Executed | Medium |
| TC_S15 | Post-Login Redirect | To validate successful login redirects user to Dashboard page | User must enter valid credentials | Manual | 1. Login successfully | User redirected to Dashboard page |  | Not Executed | High |
| TC_S16 | Register Link Navigation | To validate “Register Now!” link navigates to Signup page | Sign In page is open | Manual | 1. Click “Register Now!” link | User is redirected to Signup page |  | Not Executed | Medium |

---

## ✅ Summary

These test cases validate Sign In functionality including UI validation, input validation, authentication checks, security validation, navigation, and successful login workflow.

---

## 👨‍💻 Author
Created as part of QA learning journey by Smrity Thapa.
