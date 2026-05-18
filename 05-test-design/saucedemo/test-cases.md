# 🧪 Test Cases – SauceDemo Web Application

**Version:** 1.0  
**Author:** Smrity Thapa  
**Date:** May 2026  
**Application:** https://www.saucedemo.com/

---

## Module 1: Login

| TC ID | Test Case Name | Test Scenario | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC-LGN-001 | Valid Login – Standard User | TS-LGN-001 | Browser open, navigate to https://www.saucedemo.com/ | Positive | 1. Enter `standard_user` in Username<br>2. Enter `secret_sauce` in Password<br>3. Click **Login** | User is redirected to `/inventory.html`. Page title shows "Swag Labs". Products are visible. No error message shown. | | Not Executed | High |
| TC-LGN-002 | Invalid Username Login | TS-LGN-002 | Browser open, navigate to https://www.saucedemo.com/ | Negative | 1. Enter `wrong_user` in Username<br>2. Enter `secret_sauce` in Password<br>3. Click **Login** | Error message displayed: *"Epic sadface: Username and password do not match any user in this service"*. User stays on login page. | | Not Executed | High |
| TC-LGN-003 | Invalid Password Login | TS-LGN-002 | Browser open, navigate to https://www.saucedemo.com/ | Negative | 1. Enter `standard_user` in Username<br>2. Enter `wrongpassword` in Password<br>3. Click **Login** | Error message displayed: *"Epic sadface: Username and password do not match any user in this service"*. User stays on login page. | | Not Executed | High |
| TC-LGN-004 | Empty Username Field | TS-LGN-003 | Browser open, navigate to https://www.saucedemo.com/ | Negative | 1. Leave Username field empty<br>2. Enter `secret_sauce` in Password<br>3. Click **Login** | Error message displayed: *"Epic sadface: Username is required"*. User stays on login page. | | Not Executed | Medium |
| TC-LGN-005 | Empty Password Field | TS-LGN-003 | Browser open, navigate to https://www.saucedemo.com/ | Negative | 1. Enter `standard_user` in Username<br>2. Leave Password field empty<br>3. Click **Login** | Error message displayed: *"Epic sadface: Password is required"*. User stays on login page. | | Not Executed | Medium |
| TC-LGN-006 | Both Fields Empty | TS-LGN-003 | Browser open, navigate to https://www.saucedemo.com/ | Negative | 1. Leave both Username and Password fields empty<br>2. Click **Login** | Error message displayed: *"Epic sadface: Username is required"*. User stays on login page. | | Not Executed | Medium |
| TC-LGN-007 | Locked Out User Login | TS-LGN-004 | Browser open, navigate to https://www.saucedemo.com/ | Negative | 1. Enter `locked_out_user` in Username<br>2. Enter `secret_sauce` in Password<br>3. Click **Login** | Error message displayed: *"Epic sadface: Sorry, this user has been locked out."*. User cannot access the inventory page. | | Not Executed | High |

---

## Module 2: Inventory

| TC ID | Test Case Name | Test Scenario | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC-INV-001 | All Products Displayed | TS-INV-001 | Logged in as `standard_user`, on the inventory page | Positive | 1. Observe the product listing<br>2. Count the number of products<br>3. Check each product has name, description, price, and image | Exactly 6 products displayed. Each product has a visible name, description, price (in $), and image. | | Not Executed | High |
| TC-INV-002 | Sort A to Z | TS-INV-002 | Logged in as `standard_user`, on the inventory page | Positive | 1. Click the sort dropdown<br>2. Select **"Name (A to Z)"** | Products re-order alphabetically A to Z. First product starts with "S" (Sauce Labs Backpack). | | Not Executed | Medium |
| TC-INV-003 | Sort Z to A | TS-INV-002 | Logged in as `standard_user`, on the inventory page | Positive | 1. Click the sort dropdown<br>2. Select **"Name (Z to A)"** | Products re-order alphabetically Z to A. First product starts with "T" (Test.allTheThings() T-Shirt). | | Not Executed | Medium |
| TC-INV-004 | Sort Price Low to High | TS-INV-002 | Logged in as `standard_user`, on the inventory page | Positive | 1. Click the sort dropdown<br>2. Select **"Price (low to high)"** | Products are sorted by price ascending. First product shows the lowest price ($7.99). | | Not Executed | Medium |
| TC-INV-005 | Sort Price High to Low | TS-INV-002 | Logged in as `standard_user`, on the inventory page | Positive | 1. Click the sort dropdown<br>2. Select **"Price (high to low)"** | Products are sorted by price descending. First product shows the highest price ($49.99). | | Not Executed | Medium |
| TC-INV-006 | Navigate to Product Detail Page | TS-INV-003 | Logged in as `standard_user`, on the inventory page | Positive | 1. Click on the product name **"Sauce Labs Backpack"** | User is navigated to the product detail page. Page shows product name, description, price ($29.99), image, and **"Add to cart"** button. | | Not Executed | Medium |
| TC-INV-007 | Add to Cart from Inventory Page | TS-INV-004 | Logged in as `standard_user`, on the inventory page, cart is empty | Positive | 1. Locate **"Sauce Labs Backpack"**<br>2. Click the **"Add to cart"** button | Button text changes to **"Remove"**. Cart icon badge in the header shows **"1"**. | | Not Executed | High |

---

## Module 3: Cart

| TC ID | Test Case Name | Test Scenario | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC-CRT-001 | Cart Badge Updates on Add | TS-CRT-001 | Logged in as `standard_user`, cart is empty | Positive | 1. Click **"Add to cart"** on **"Sauce Labs Backpack"**<br>2. Observe the cart icon in the header | Cart icon displays a badge with number **"1"**. | | Not Executed | High |
| TC-CRT-002 | Cart Badge Updates on Remove | TS-CRT-002 | Logged in as `standard_user`, one item in cart | Positive | 1. Click **"Remove"** on the product that was added<br>2. Observe the cart icon | Cart badge disappears completely. Button text reverts to **"Add to cart"**. | | Not Executed | High |
| TC-CRT-003 | Cart Retains Items After Navigation | TS-CRT-003 | Logged in as `standard_user`, cart is empty | Positive | 1. Add **"Sauce Labs Backpack"** to cart<br>2. Click the product name to go to its detail page<br>3. Click **"Back to products"**<br>4. Click the cart icon | Cart still contains **"Sauce Labs Backpack"**. Badge still shows **"1"**. | | Not Executed | High |
| TC-CRT-004 | Multiple Items Added to Cart | TS-CRT-004 | Logged in as `standard_user`, cart is empty | Positive | 1. Click **"Add to cart"** on **"Sauce Labs Backpack"**<br>2. Click **"Add to cart"** on **"Sauce Labs Bike Light"**<br>3. Click **"Add to cart"** on **"Sauce Labs Bolt T-Shirt"**<br>4. Click the cart icon | Cart badge shows **"3"**. All 3 products listed in the cart with correct names and prices. | | Not Executed | High |
| TC-CRT-005 | Remove Item from Cart Page | TS-CRT-002 | Logged in as `standard_user`, at least one item in cart, on the cart page | Positive | 1. Navigate to cart by clicking the cart icon<br>2. Click **"Remove"** next to **"Sauce Labs Backpack"**<br>3. Observe cart contents and badge | Product is removed from the cart list. If cart is now empty, badge disappears and cart page shows no items. | | Not Executed | Medium |

---

## Module 4: Checkout

| TC ID | Test Case Name | Test Scenario | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC-CHK-001 | Navigate to Checkout from Cart | TS-CHK-001 | Logged in as `standard_user`, one item in cart, on the cart page | Positive | 1. Click the **"Checkout"** button | User is redirected to `/checkout-step-one.html`. Form with First Name, Last Name, and Zip Code fields is displayed. | | Not Executed | High |
| TC-CHK-002 | Checkout – Empty First Name | TS-CHK-002 | Logged in as `standard_user`, on the checkout information page | Negative | 1. Leave First Name empty<br>2. Enter `Thapa` in Last Name<br>3. Enter `44600` in Zip Code<br>4. Click **"Continue"** | Error message displayed: *"Error: First Name is required"*. User stays on the checkout form. | | Not Executed | High |
| TC-CHK-003 | Checkout – Empty Last Name | TS-CHK-002 | Logged in as `standard_user`, on the checkout information page | Negative | 1. Enter `Smrity` in First Name<br>2. Leave Last Name empty<br>3. Enter `44600` in Zip Code<br>4. Click **"Continue"** | Error message displayed: *"Error: Last Name is required"*. User stays on the checkout form. | | Not Executed | High |
| TC-CHK-004 | Checkout – Empty Zip Code | TS-CHK-002 | Logged in as `standard_user`, on the checkout information page | Negative | 1. Enter `Smrity` in First Name<br>2. Enter `Thapa` in Last Name<br>3. Leave Zip Code empty<br>4. Click **"Continue"** | Error message displayed: *"Error: Postal Code is required"*. User stays on the checkout form. | | Not Executed | High |
| TC-CHK-005 | Checkout – All Fields Empty | TS-CHK-002 | Logged in as `standard_user`, on the checkout information page | Negative | 1. Leave all fields (First Name, Last Name, Zip Code) empty<br>2. Click **"Continue"** | Error message displayed: *"Error: First Name is required"*. User stays on the checkout form. | | Not Executed | Medium |
| TC-CHK-006 | Checkout with Valid Information | TS-CHK-003 | Logged in as `standard_user`, on the checkout information page, one item in cart | Positive | 1. Enter `Smrity` in First Name<br>2. Enter `Thapa` in Last Name<br>3. Enter `44600` in Zip Code<br>4. Click **"Continue"** | User is redirected to the checkout overview page (`/checkout-step-two.html`). | | Not Executed | High |
| TC-CHK-007 | Checkout Overview – Correct Items and Pricing | TS-CHK-004 | Logged in as `standard_user`, on the checkout overview page | Positive | 1. Observe product list on the overview page<br>2. Check product names and prices<br>3. Verify Item Total, Tax, and Total amounts are shown | All cart items listed correctly. Item Total, Tax, and Total Price are all visible and calculated correctly. | | Not Executed | High |
| TC-CHK-008 | Complete Order Successfully | TS-CHK-005 | Logged in as `standard_user`, on the checkout overview page | Positive | 1. Review the order summary<br>2. Click the **"Finish"** button | User is redirected to the order confirmation page. Message *"Thank you for your order!"* is displayed. Cart badge disappears. | | Not Executed | High |

---

## Module 5: Navigation

| TC ID | Test Case Name | Test Scenario | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC-NAV-001 | Open Burger Menu | TS-NAV-001 | Logged in as `standard_user`, on the inventory page | Positive | 1. Click the burger menu icon (☰) in the top-left corner | Side navigation menu opens. Four options are visible: **All Items**, **About**, **Logout**, **Reset App State**. | | Not Executed | Medium |
| TC-NAV-002 | Logout via Burger Menu | TS-NAV-002 | Logged in as `standard_user`, burger menu is open | Positive | 1. Click the burger menu icon (☰)<br>2. Click **"Logout"** | User is logged out and redirected to the login page (`/`). Attempting to go back does not allow access to inventory. | | Not Executed | High |
| TC-NAV-003 | Back to Products from Detail Page | TS-NAV-003 | Logged in as `standard_user`, on a product detail page | Positive | 1. Click on any product to go to its detail page<br>2. Click the **"← Back to products"** link | User is returned to the inventory page. All 6 products are displayed. | | Not Executed | Medium |

---

## Module 6: UI Validation

| TC ID | Test Case Name | Test Scenario | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|---|---|---|---|---|---|---|---|---|---|
| TC-UI-001 | Add to Cart Buttons Visible | TS-UI-001 | Logged in as `standard_user`, on the inventory page | UI | 1. Observe each of the 6 products on the inventory page<br>2. Check the button below each product | All 6 products have a clearly visible button labeled **"Add to cart"**. No buttons are missing or hidden. | | Not Executed | Medium |
| TC-UI-002 | Login Error Message Styling | TS-UI-002 | Browser open, on the login page | UI | 1. Leave both fields empty<br>2. Click **Login**<br>3. Observe the error message styling | Error message appears inside a red highlighted container. Text is readable. An **X** (close) icon is present and clicking it dismisses the error. | | Not Executed | Low |
| TC-UI-003 | Cart Icon Visible Across All Pages | TS-UI-003 | Logged in as `standard_user`, one item in cart | UI | 1. Check header on the **Inventory** page<br>2. Navigate to a product detail page and check header<br>3. Navigate to the **Cart** page and check header<br>4. Navigate to **Checkout** page and check header | Cart icon is visible in the header on all 4 pages. Badge showing **"1"** is consistent across all pages. | | Not Executed | Medium |

---

## Execution Summary

| Module | Total TCs | Pass | Fail | Not Executed |
|---|---|---|---|---|
| Login | 7 | 5 | 2 | 0 |
| Inventory | 7 | 1 | 6 | 0 |
| Cart | 5 | 5 | 0 | 0 |
| Checkout | 8 | 7 | 1 | 0 |
| Navigation | 3 | 2 | 1 | 0 |
| UI Validation | 3 | 1 | 2 | 0 |
| **Total** | **33** | **21** | **12** | **0** |


---

## 👨‍💻 Author  
*Created as part of QA learning journey by Smrity Thapa*  
*Repository: https://github.com/Smrity-Thapa33/qa_fundamentals*
