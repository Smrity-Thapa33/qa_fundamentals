# JPetStore - Cart Module Page Test Cases

📥 **Excel Version:**  
[JPETSTORE_Cart_module_page_TestCases.xlsx](./JPETSTORE_Cart_module_page_TestCases.xlsx)

---
## Module
Shopping Cart

## Application
JPetStore Demo Application

## Objective
To validate UI elements, cart functionality, calculations, validations, navigation, and access control behavior of the Shopping Cart page.

---

## Test Cases

| Test Case ID | Test Case Name | Test Scenarios | Pre-conditions | Type | Steps | Expected Result | Actual Result | Status | Priority |
|--------------|----------------|----------------|---------------|------|-------|-----------------|---------------|--------|----------|
| TC_C01 | Cart Page Display | To validate that the Shopping Cart page is displayed to the user | User is logged in | Manual | 1. Login to application<br>2. Click cart icon | Shopping Cart page displayed |  | Not Executed | High |
| TC_C02 | Logo on Cart Page | To validate that JPET Store logo is displayed on the Cart page | User is on Cart page | Manual | 1. Observe top section | JPET Store logo visible |  | Not Executed | Low |
| TC_C03 | Navigation Links | To validate top navigation links are displayed | User is on Cart page | Manual | 1. Observe navigation bar | Fish, Dogs, Reptiles, Cats, Birds visible |  | Not Executed | Low |
| TC_C04 | Cart Header | To validate “Shopping Cart” header is displayed | User is on Cart page | Manual | 1. Observe page header | "Shopping Cart" header displayed |  | Not Executed | Low |
| TC_C05 | Cart Table Headers | To validate cart table headers are displayed | Cart contains items | Manual | 1. Add product to cart | All cart headers displayed correctly |  | Not Executed | High |
| TC_C06 | Return to Main Menu Link | To validate Return to Main Menu link is displayed | User is on Cart page | Manual | 1. Observe bottom section | "Return to Main Menu" link visible |  | Not Executed | Medium |
| TC_C07 | Search Bar Display | To validate search textbox and button are displayed | User is on Cart page | Manual | 1. Observe search area | Search textbox and button displayed |  | Not Executed | Low |
| TC_C08 | Update Cart Button | To validate Update Cart button is displayed | User is on Cart page | Manual | 1. Observe cart controls | Update Cart button displayed |  | Not Executed | High |
| TC_C09 | Empty Cart Message | To validate empty cart message when no items added | Cart has no items | Manual | 1. Open cart without products | "Your cart is empty" message displayed |  | Not Executed | High |
| TC_C10 | Empty Cart Subtotal | To validate subtotal shows $0.00 when cart is empty | Cart is empty | Manual | 1. Open cart page | Subtotal shows $0.00 |  | Not Executed | High |
| TC_C11 | Add Product to Cart | To validate product is added from product details page | User is on product details page | Manual | 1. Open product details<br>2. Click Add to Cart | Product added successfully |  | Not Executed | High |
| TC_C12 | Product Appears in Cart | To validate added product appears in cart | Product added to cart | Manual | 1. Open cart page | Product appears in cart table |  | Not Executed | High |
| TC_C13 | Correct IDs Displayed | To validate Item ID and Product ID display correctly | Product in cart | Manual | 1. Observe cart row | Correct Item ID & Product ID displayed |  | Not Executed | Medium |
| TC_C14 | Product Info Accuracy | To validate product description and price accuracy | Product in cart | Manual | 1. Observe product details | Description & price correct |  | Not Executed | High |
| TC_C15 | Stock Status Display | To validate stock status is displayed | Product in cart | Manual | 1. Observe stock column | Correct stock status displayed |  | Not Executed | Medium |
| TC_C16 | Default Quantity | To validate default quantity is set to 1 | Product added to cart | Manual | 1. Add product and open cart | Default quantity is 1 |  | Not Executed | High |
| TC_C17 | Single Item Cost Calculation | To validate total cost calculation for single product | Product in cart | Manual | 1. Verify price and total | Total = Price × 1 |  | Not Executed | High |
| TC_C18 | Quantity Update Calculation | To validate total cost updates after quantity change | Product in cart | Manual | 1. Change quantity<br>2. Click Update Cart | Total recalculated correctly |  | Not Executed | High |
| TC_C19 | Subtotal Update | To validate subtotal updates after cart update | Multiple products in cart | Manual | 1. Update quantities | Subtotal updated correctly |  | Not Executed | High |
| TC_C20 | Negative Quantity Restriction | To validate negative quantity is not accepted | Product in cart | Manual | 1. Enter negative value | Error shown or value reset |  | Not Executed | High |
| TC_C21 | Zero Quantity Restriction | To validate zero quantity is not accepted | Product in cart | Manual | 1. Enter quantity as 0 | Product removed or error shown |  | Not Executed | High |
| TC_C22 | Non-numeric Quantity Restriction | To validate quantity field rejects alphabets/symbols | Product in cart | Manual | 1. Enter letters/symbols | Only numeric values accepted |  | Not Executed | High |
| TC_C23 | Remove Product via Quantity 0 | To validate product removal when quantity set to zero | Product in cart | Manual | 1. Set quantity to 0 and update cart | Product removed from cart |  | Not Executed | High |
| TC_C24 | Cart Empty After Removal | To validate cart empty message after removing all products | All items removed | Manual | 1. Remove all products | Cart shows empty message |  | Not Executed | High |
| TC_C25 | Subtotal After Removal | To validate subtotal updates after removal | Items removed in cart | Manual | 1. Remove product and update cart | Subtotal recalculated correctly |  | Not Executed | High |
| TC_C26 | Return to Main Menu Navigation | To validate navigation to dashboard | User is on Cart page | Manual | 1. Click "Return to Main Menu" | Redirected to Dashboard page |  | Not Executed | Medium |
| TC_C27 | Category Navigation from Cart | To validate navigation to category pages | User is on Cart page | Manual | 1. Click category link | Opens respective category page |  | Not Executed | Medium |
| TC_C28 | Out-of-Stock Behavior | To validate cart behavior when product is out of stock | Product becomes out of stock | Manual | 1. Attempt checkout | Warning shown or checkout restricted |  | Not Executed | Medium |
| TC_C29 | Cart Access Control | To validate cart access only for logged-in users | User logged out | Manual | 1. Access cart URL directly | Redirected to Sign In page |  | Not Executed | High |

---
## ✅ Summary

These test cases validate Shopping Cart functionality including UI verification, cart operations, calculation accuracy, validation rules, navigation, and security access control.

---

## 👨‍💻 Author
Created as part of QA learning journey by Smrity Thapa.
