# Regression Testing — SauceDemo

## Overview

| Field | Details |
|---|---|
| **Tester** | Smrity Thapa |
| **Application** | SauceDemo (https://www.saucedemo.com) |
| **Base Test Suite** | SauceDemo Test Cases v1.0 (33 test cases) |
| **Total TCs in Regression Suite** | 15 |
| **Selection Strategy** | Risk-based + Core flow coverage |

---

## What is Regression Testing?

Regression testing is the process of re-executing a selected set of test cases after a code change, bug fix, or new feature is added — to ensure that existing functionality still works as expected and nothing has been broken.

> Not all test cases need to be re-run every time. A well-defined regression suite focuses on **high-risk, high-priority, and core flow** test cases.

---

## Regression Suite Selection Criteria

Test cases were selected for the regression suite based on the following criteria:

| Criteria | Description |
|---|---|
| **High Priority** | Test cases marked as High priority in the base suite |
| **Core User Flow** | Tests covering critical paths a user must complete (login → browse → cart → checkout) |
| **Previously Failed** | Test cases that have failed before and are likely to regress |
| **High Risk Area** | Functionality most likely to break after a code change |

---

## Regression Test Suite

### Module 1: Login *(3 TCs)*

| TC ID | Test Case Name | Priority | Selection Reason |
|---|---|---|---|
| TC-LGN-001 | Valid Login – Standard User | High | Core entry point — if this breaks, nothing else works |
| TC-LGN-002 | Invalid Username Login | High | Security critical — must always reject invalid credentials |
| TC-LGN-007 | Locked Out User Login | High | Edge case with specific error — likely to regress after auth changes |

---

### Module 2: Inventory *(2 TCs)*

| TC ID | Test Case Name | Priority | Selection Reason |
|---|---|---|---|
| TC-INV-001 | All Products Displayed | High | Core display — if products don't load, the app is broken |
| TC-INV-007 | Add to Cart from Inventory Page | High | Critical user action — triggers cart badge update |

---

### Module 3: Cart *(3 TCs)*

| TC ID | Test Case Name | Priority | Selection Reason |
|---|---|---|---|
| TC-CRT-001 | Cart Badge Updates on Add | High | Visual feedback — must reflect correct item count |
| TC-CRT-002 | Cart Badge Updates on Remove | High | Visual feedback — badge must disappear on empty cart |
| TC-CRT-003 | Cart Retains Items After Navigation | High | State persistence — cart must not reset on page change |

---

### Module 4: Checkout *(5 TCs)*

| TC ID | Test Case Name | Priority | Selection Reason |
|---|---|---|---|
| TC-CHK-001 | Navigate to Checkout from Cart | High | Entry to checkout flow — must always be accessible |
| TC-CHK-002 | Checkout – Empty First Name | High | Validation — must prevent incomplete form submission |
| TC-CHK-006 | Checkout with Valid Information | High | Core flow — must proceed to overview on valid input |
| TC-CHK-007 | Checkout Overview – Correct Items and Pricing | High | Data accuracy — pricing must be correct at all times |
| TC-CHK-008 | Complete Order Successfully | High | End-to-end flow — order completion must always work |

---

### Module 5: Navigation *(2 TCs)*

| TC ID | Test Case Name | Priority | Selection Reason |
|---|---|---|---|
| TC-NAV-002 | Logout via Burger Menu | High | Security critical — user must always be able to log out |
| TC-NAV-003 | Back to Products from Detail Page | Medium | Navigation integrity — back flow must work consistently |

---

## Test Cases Excluded from Regression Suite

These test cases were intentionally excluded to keep the suite lean and fast:

| TC ID | Test Case Name | Reason for Exclusion |
|---|---|---|
| TC-LGN-003 | Invalid Password Login | Similar coverage to TC-LGN-002, low added value |
| TC-LGN-004 | Empty Username Field | Low priority, UI validation unlikely to regress |
| TC-LGN-005 | Empty Password Field | Low priority, UI validation unlikely to regress |
| TC-LGN-006 | Both Fields Empty | Covered partially by TC-LGN-004 |
| TC-INV-002 | Sort A to Z | Medium priority, sorting is secondary to core flow |
| TC-INV-003 | Sort Z to A | Medium priority, sorting is secondary to core flow |
| TC-INV-004 | Sort Price Low to High | Medium priority, sorting is secondary to core flow |
| TC-INV-005 | Sort Price High to Low | Medium priority, sorting is secondary to core flow |
| TC-INV-006 | Navigate to Product Detail Page | Medium priority, covered indirectly by cart tests |
| TC-CRT-004 | Multiple Items Added to Cart | Covered by TC-CRT-001 |
| TC-CRT-005 | Remove Item from Cart Page | Covered by TC-CRT-002 |
| TC-CHK-003 | Checkout – Empty Last Name | Similar to TC-CHK-002 |
| TC-CHK-004 | Checkout – Empty Zip Code | Similar to TC-CHK-002 |
| TC-CHK-005 | Checkout – All Fields Empty | Covered by TC-CHK-002 |
| TC-NAV-001 | Open Burger Menu | Low risk, prerequisite covered in TC-NAV-002 |
| TC-UI-001 | Add to Cart Buttons Visible | UI check, low regression risk |
| TC-UI-002 | Login Error Message Styling | Low priority, cosmetic |
| TC-UI-003 | Cart Icon Visible Across All Pages | Low priority, cosmetic |

---

## Regression Suite Summary

| Module | Total TCs | In Regression Suite | Excluded |
|---|---|---|---|
| Login | 7 | 3 | 4 |
| Inventory | 7 | 2 | 5 |
| Cart | 5 | 3 | 2 |
| Checkout | 8 | 5 | 3 |
| Navigation | 3 | 2 | 1 |
| UI Validation | 3 | 0 | 3 |
| **Total** | **33** | **15** | **18** |

> **Suite Coverage: 45%** — This is intentional. A lean regression suite focused on high-risk areas executes faster and catches the most critical regressions.

---

## When to Run This Regression Suite

| Trigger | Description |
|---|---|
| After a bug fix | Verify the fix didn't break other functionality |
| After a new feature | Ensure existing features still work |
| Before a release | Final sanity check before deployment |
| After UI/layout changes | Confirm core flows still function correctly |

---

## 👨‍💻 Author
*Created as part of QA learning journey by Smrity Thapa*  
*Repository: https://github.com/Smrity-Thapa33/qa_fundamentals*