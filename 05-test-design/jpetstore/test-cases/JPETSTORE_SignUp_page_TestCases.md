# JPetStore - Signup Page Test Cases

📥 **Excel Version:**  
[JPETSTORE_SignUp_page_TestCases.xlsx](./JPETSTORE_SignUp_page_TestCases.xlsx)

---

## Module
Signup / User Registration

## Application
JPetStore Demo Application

## Objective
To validate UI elements, field validations, input restrictions, error handling, and successful user registration functionality of the Signup page.

---

## Test Cases

| Test Case ID | Test Case Name | Test Scenario | Pre-condition | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC_01 | Signup Page Display | Validate signup page is displayed | User is on Home Page | Manual | 1. Open JPetStore application<br>2. Click "Sign in"<br>3. Click "Register Now" | Signup page displayed successfully |  | Not Executed | High |
| TC_02 | Logo Display | Validate logo is displayed | User on Signup Page | Manual | Observe top section | JPET Store logo visible |  | Not Executed | Low |
| TC_03 | Top Navigation Links | Validate navigation links display | User on Signup Page | Manual | Observe navigation bar | Fish, Dogs, Reptiles, Cats, Birds displayed |  | Not Executed | Low |
| TC_04 | Section Visibility | Validate form sections display | User on Signup Page | Manual | 1. Scroll page<br>2. Observe User, Account & Profile sections | All sections visible and labeled |  | Not Executed | Low |
| TC_05 | Field Alignment | Validate input alignment | User on Signup Page | Manual | Visually inspect fields | Fields aligned properly |  | Not Executed | Low |
| TC_06 | Save Button Display | Validate Save button display | User on Signup Page | Manual | 1. Scroll to bottom<br>2. Check Save Account Information button | Button is shown |  | Not Executed | Low |
| TC_07 | User ID Validation | Validate alphanumeric User ID | User on Signup Page | Manual | Enter letters + numbers | Alphanumeric data accepted |  | Not Executed | High |
| TC_08 | Blank User ID | Validate blank User ID error | User on Signup Page | Manual | 1. Leave User ID blank<br>2. Submit form | Error shown for blank User ID |  | Not Executed | High |
| TC_09 | Existing User ID | Validate duplicate user error | User on Signup Page | Manual | 1. Enter existing User ID<br>2. Submit form | Error message displayed |  | Not Executed | High |
| TC_10 | Password Rules | Validate password rules | User on Signup Page | Manual | 1. Enter valid password<br>2. Submit form | Password accepted |  | Not Executed | High |
| TC_11 | Blank Password | Validate blank password error | User on Signup Page | Manual | 1. Leave password blank<br>2. Submit | Error displayed |  | Not Executed | High |
| TC_12 | Repeat Password Field | Validate repeat password exists | User on Signup Page | Manual | Observe Repeat Password field | Field visible |  | Not Executed | Medium |
| TC_13 | Password Mismatch | Validate mismatch error | User on Signup Page | Manual | 1. Enter different passwords<br>2. Submit | Mismatch error shown |  | Not Executed | High |
| TC_14 | Blank Repeat Password | Validate blank repeat password | User on Signup Page | Manual | 1. Leave repeat password blank<br>2. Submit | Error displayed |  | Not Executed | High |
| TC_15 | Valid Email | Validate email format | User on Signup Page | Manual | Enter valid email | Email accepted |  | Not Executed | High |
| TC_16 | Invalid Email | Validate invalid email error | User on Signup Page | Manual | 1. Enter invalid email<br>2. Submit | Error displayed |  | Not Executed | High |
| TC_17 | Phone Numeric Only | Validate phone numeric input | User on Signup Page | Manual | Enter numbers only | Numbers accepted |  | Not Executed | Medium |
| TC_18 | Invalid Phone | Validate phone validation | User on Signup Page | Manual | 1. Enter letters/symbols<br>2. Submit | Error shown |  | Not Executed | Medium |
| TC_19 | City Alphabetic | Validate city input | User on Signup Page | Manual | Enter letters only | City accepted |  | Not Executed | Medium |
| TC_20 | State Validation | Validate state value | User on Signup Page | Manual | Enter valid state | State accepted |  | Not Executed | Medium |
| TC_21 | ZIP Numeric | Validate ZIP numeric | User on Signup Page | Manual | Enter numeric ZIP | ZIP accepted |  | Not Executed | Medium |
| TC_22 | Country Field | Validate country input | User on Signup Page | Manual | 1. Observe field<br>2. Enter country | Field usable |  | Not Executed | Medium |
| TC_23 | Dropdown Display | Validate dropdown visibility | User on Signup Page | Manual | Observe language & category dropdowns | Both displayed |  | Not Executed | Medium |
| TC_24 | Default Language | Validate default language | User on Signup Page | Manual | Open language dropdown | Default language selected |  | Not Executed | Medium |
| TC_25 | Change Language | Validate language change | User on Signup Page | Manual | Select different language | Language updates |  | Not Executed | Medium |
| TC_26 | Category List | Validate category options | User on Signup Page | Manual | Open category dropdown | All categories listed |  | Not Executed | Medium |
| TC_27 | Select Category | Validate category selection | User on Signup Page | Manual | Choose category | Category saved |  | Not Executed | Medium |
| TC_28 | Checkbox Display | Validate checkbox visibility | User on Signup Page | Manual | Observe MyList & MyBanner | Both visible |  | Not Executed | Medium |
| TC_29 | Checkbox Selection | Validate checkbox toggle | User on Signup Page | Manual | Select/unselect checkboxes | Toggles correctly |  | Not Executed | Medium |
| TC_30 | Save Button Enabled | Validate button enabled | Mandatory fields filled | Manual | 1. Fill required fields<br>2. Observe button | Button enabled |  | Not Executed | High |
| TC_31 | Mandatory Field Errors | Validate required field errors | Fields empty | Manual | 1. Leave fields empty<br>2. Submit | Error messages shown |  | Not Executed | High |
| TC_32 | Successful Signup | Validate successful signup | Valid data entered | Manual | Submit form | Account created & redirected |  | Not Executed | High |
| TC_33 | Success Message | Validate success message | Signup successful | Manual | Observe message | Success message displayed |  | Not Executed | Medium |
| TC_34 | Post Signup Redirect | Validate redirect | Signup successful | Manual | Complete signup | Redirected correctly |  | Not Executed | Medium |
| TC_35 | Password Masking | Validate password masking | Password fields visible | Manual | Type password | Characters masked |  | Not Executed | High |
| TC_36 | Submit via Enter Key | Validate Enter key submission | Mandatory fields filled | Manual | 1. Fill fields<br>2. Press Enter | Form submits successfully |  | Not Executed | High |
---

## ✅ Summary

These test cases validate Signup functionality including UI validation, field validations, input handling, error messaging, and successful account creation workflow.

---

## 👨‍💻 Author
Created as part of QA learning journey by Smrity Thapa.
