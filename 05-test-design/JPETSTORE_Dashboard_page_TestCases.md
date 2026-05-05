# JPetStore - Dashboard Page Test Cases

📥 **Excel Version:**  
[JPETSTORE_Dashboard_page_TestCases.xlsx](./JPETSTORE_Dashboard_page_TestCases.xlsx)

---

## Module  
Dashboard / Home Page (Post Login)

## Application  
JPetStore Demo Application

## Objective  
To validate UI elements, navigation, user session behavior, search functionality, and overall usability of the Dashboard page after successful login.

---

## Test Cases  

| Test Case ID | Test Case Name | Test Scenarios | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|--------------|----------------|----------------|---------------|------|-------|-----------------|---------------|--------|----------|
| TC_D01 | Dashboard Page Display | To validate that dashboard is displayed after login | User has valid account | Manual | 1. Open application<br>2. Enter valid credentials<br>3. Click Login | Dashboard page displayed successfully |  | Not Executed | High |
| TC_D02 | Logo Display | To validate JPET Store logo visibility | User is on Dashboard | Manual | 1. Observe top-left section | Logo is visible |  | Not Executed | Low |
| TC_D03 | Welcome Message | To validate welcome message for user | User is logged in | Manual | 1. Observe header section | Welcome message with username displayed |  | Not Executed | Medium |
| TC_D04 | Navigation Links | To validate category navigation links | User is on Dashboard | Manual | 1. Observe top navigation bar | Fish, Dogs, Reptiles, Cats, Birds links visible |  | Not Executed | High |
| TC_D05 | Category Navigation | To validate navigation to category pages | User is on Dashboard | Manual | 1. Click any category link (e.g., Fish) | User redirected to selected category page |  | Not Executed | High |
| TC_D06 | Sidebar Category List | To validate sidebar category list display | User is on Dashboard | Manual | 1. Observe left sidebar | All categories listed correctly |  | Not Executed | Medium |
| TC_D07 | Sidebar Navigation | To validate sidebar links functionality | User is on Dashboard | Manual | 1. Click any sidebar category | Correct category page opens |  | Not Executed | High |
| TC_D08 | Banner Display | To validate promotional banner display | User is on Dashboard | Manual | 1. Observe main section | Banner image displayed properly |  | Not Executed | Low |
| TC_D09 | Search Bar Display | To validate search textbox and button | User is on Dashboard | Manual | 1. Observe top section | Search textbox and button visible |  | Not Executed | High |
| TC_D10 | Search Functionality | To validate product search | User is on Dashboard | Manual | 1. Enter product keyword<br>2. Click Search | Relevant products displayed |  | Not Executed | High |
| TC_D11 | Empty Search Validation | To validate behavior on empty search | User is on Dashboard | Manual | 1. Leave search blank<br>2. Click Search | Error shown or no results handled properly |  | Not Executed | Medium |
| TC_D12 | Invalid Search | To validate search with invalid keyword | User is on Dashboard | Manual | 1. Enter random text<br>2. Click Search | No results message displayed |  | Not Executed | Medium |
| TC_D13 | Cart Icon Display | To validate cart icon visibility | User is logged in | Manual | 1. Observe header section | Cart icon visible |  | Not Executed | High |
| TC_D14 | Cart Navigation | To validate cart access from dashboard | User is on Dashboard | Manual | 1. Click cart icon | User redirected to Cart page |  | Not Executed | High |
| TC_D15 | Sign Out Option Display | To validate logout option visibility | User is logged in | Manual | 1. Observe header section | Sign Out option visible |  | Not Executed | High |
| TC_D16 | Logout Functionality | To validate logout functionality | User is logged in | Manual | 1. Click Sign Out | User logged out and redirected to Sign In page |  | Not Executed | High |
| TC_D17 | Session Persistence | To validate session remains active | User is logged in | Manual | 1. Refresh page | User remains logged in |  | Not Executed | Medium |
| TC_D18 | Direct URL Access Control | To validate dashboard access control | User is logged out | Manual | 1. Enter dashboard URL directly | Redirected to Sign In page |  | Not Executed | High |
| TC_D19 | Page Responsiveness | To validate UI responsiveness | User is on Dashboard | Manual | 1. Resize browser window | Layout adjusts properly |  | Not Executed | Low |
| TC_D20 | Broken Links Check | To validate all links are working | User is on Dashboard | Manual | 1. Click all major links | No broken links found |  | Not Executed | Medium |

---

## ✅ Summary  

These test cases validate Dashboard functionality including UI verification, navigation, search behavior, session handling, and access control after login.

---

## 👨‍💻 Author  
Created as part of QA learning journey by Smrity Thapa.
