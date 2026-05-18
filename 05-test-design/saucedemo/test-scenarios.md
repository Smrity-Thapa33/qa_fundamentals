# 📋 Test Scenarios – SauceDemo Web Application

**Version:** 1.0  
**Author:** Smrity Thapa  
**Date:** May 2026  
**Application:** https://www.saucedemo.com/

---

## Module 1: Login

| Scenario ID | Test Scenario | Type |
|---|---|---|
| TS-LGN-001 | Verify that a valid user can log in successfully and is redirected to the inventory page | Positive |
| TS-LGN-002 | Verify that login with invalid credentials shows an appropriate error message | Negative |
| TS-LGN-003 | Verify that submitting empty login fields shows the correct validation messages | Negative |
| TS-LGN-004 | Verify that a locked-out user cannot log in and sees a specific error message | Negative |

---

## Module 2: Inventory / Product Listing

| Scenario ID | Test Scenario | Type |
|---|---|---|
| TS-INV-001 | Verify that all 6 products are displayed correctly with name, price, image, and button | Positive |
| TS-INV-002 | Verify that product sorting works correctly for all four sort options | Positive |
| TS-INV-003 | Verify that clicking a product navigates to the correct product detail page | Positive |
| TS-INV-004 | Verify that clicking "Add to cart" updates the cart badge and changes the button text | Positive |

---

## Module 3: Cart

| Scenario ID | Test Scenario | Type |
|---|---|---|
| TS-CRT-001 | Verify that adding a product updates the cart badge count correctly | Positive |
| TS-CRT-002 | Verify that removing a product from the inventory or cart page updates the badge | Positive |
| TS-CRT-003 | Verify that cart items are retained after navigating away and returning | Positive |
| TS-CRT-004 | Verify that multiple products can be added and all appear correctly in the cart | Positive |

---

## Module 4: Checkout

| Scenario ID | Test Scenario | Type |
|---|---|---|
| TS-CHK-001 | Verify that clicking Checkout from the cart navigates to the checkout information form | Positive |
| TS-CHK-002 | Verify that submitting the checkout form with any missing field shows a specific error | Negative |
| TS-CHK-003 | Verify that completing the checkout form with valid data proceeds to the order summary | Positive |
| TS-CHK-004 | Verify that the order summary displays the correct items, prices, and totals | Positive |
| TS-CHK-005 | Verify that clicking Finish completes the order and shows a confirmation message | Positive |

---

## Module 5: Navigation

| Scenario ID | Test Scenario | Type |
|---|---|---|
| TS-NAV-001 | Verify that the burger menu opens and displays all expected options | Positive |
| TS-NAV-002 | Verify that clicking Logout from the burger menu logs the user out | Positive |
| TS-NAV-003 | Verify that the Back to Products link on the product detail page returns to inventory | Positive |

---

## Module 6: UI Validation

| Scenario ID | Test Scenario | Type |
|---|---|---|
| TS-UI-001 | Verify that all Add to Cart buttons are visible and correctly labeled on the inventory page | Positive |
| TS-UI-002 | Verify that error messages on the login page are clearly displayed with a close icon | Positive |
| TS-UI-003 | Verify that the cart icon with badge count is visible consistently across all pages | Positive |

---

## Summary

| Module | Total Scenarios | Positive | Negative |
|---|---|---|---|
| Login | 4 | 1 | 3 |
| Inventory | 4 | 4 | 0 |
| Cart | 4 | 4 | 0 |
| Checkout | 5 | 4 | 1 |
| Navigation | 3 | 3 | 0 |
| UI Validation | 3 | 3 | 0 |
| **Total** | **23** | **19** | **4** |

---
## 👨‍💻 Author  
*Created as part of QA learning journey by Smrity Thapa*  
*Repository: https://github.com/Smrity-Thapa33/qa_fundamentals*
