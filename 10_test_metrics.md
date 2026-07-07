# 📊 Test Metrics — SauceDemo

## 📋 Overview

| Field | Details |
|---|---|
| **Tester** | Smrity Thapa |
| **Application** | SauceDemo (https://www.saucedemo.com) |
| **Testing Type** | Manual Testing |
| **Period** | May 2026 |
| **Total Test Cases** | 33 |
| **Total Bugs Found** | 11 |

---

## 📖 What are Test Metrics?

Test metrics are numbers and measurements that help us understand:
- How much testing was done
- How good the quality of the application is
- How effective the testing was

---

## 1️⃣ Test Case Metrics

### Test Case Execution Summary

| Module | Total TCs | Pass | Fail | Not Executed |
|---|---|---|---|---|
| Login | 7 | 5 | 2 | 0 |
| Inventory | 7 | 1 | 6 | 0 |
| Cart | 5 | 5 | 0 | 0 |
| Checkout | 8 | 7 | 1 | 0 |
| Navigation | 3 | 2 | 1 | 0 |
| UI Validation | 3 | 1 | 2 | 0 |
| **Total** | **33** | **21** | **12** | **0** |

### Key Calculations

| Metric | Formula | Result |
|---|---|---|
| **Test Case Pass Rate** | (Pass / Total) × 100 | (21 / 33) × 100 = **63.6%** |
| **Test Case Fail Rate** | (Fail / Total) × 100 | (12 / 33) × 100 = **36.4%** |
| **Test Execution Rate** | (Executed / Total) × 100 | (33 / 33) × 100 = **100%** |

> ⚠️ A 36.4% failure rate is high — this is expected for SauceDemo since it is an intentionally buggy application designed for testing practice.

---

## 2️⃣ Defect Metrics

### Defect Summary by Severity

| Severity | Count | Bug IDs |
|---|---|---|
| 🔴 High | 1 | BR-003 |
| 🟡 Medium | 4 | BR-004, BR-006, BR-007, BR-011 |
| 🟢 Low | 6 | BR-001, BR-002, BR-005, BR-008, BR-009, BR-010 |
| **Total** | **11** | |

### Defect Summary by Type

| Type | Count | Bug IDs |
|---|---|---|
| Functional | 4 | BR-003, BR-004, BR-006, BR-011 |
| UI / Visual | 7 | BR-001, BR-002, BR-005, BR-007, BR-008, BR-009, BR-010 |
| **Total** | **11** | |

### Key Calculations

| Metric | Formula | Result |
|---|---|---|
| **Defect Density** | Total Bugs / Total TCs | 11 / 33 = **0.33 bugs per test case** |
| **High Severity %** | (High / Total Bugs) × 100 | (1 / 11) × 100 = **9.1%** |
| **Defect Detection Rate** | Bugs Found / Total TCs | 11 / 33 = **33.3%** |

---

## 3️⃣ Defect Distribution by Module

| Module | Bugs Found | Most Critical |
|---|---|---|
| Login | 1 | BR-001 (generic error message) |
| Inventory | 3 | BR-006 (sorting broken), BR-007 (image mismatch) |
| Cart | 1 | BR-004 (reset state UI bug) |
| Checkout | 1 | BR-003 (empty cart checkout — HIGH) |
| UI / Layout | 4 | BR-008, BR-009, BR-010, BR-002 |
| Footer | 1 | BR-011 (footer links not clickable) |

---

## 4️⃣ Regression Suite Metrics

| Metric | Value |
|---|---|
| Total TCs in Regression Suite | 15 |
| Total TCs Excluded | 18 |
| Suite Coverage | 45% |
| Modules Covered | 5 out of 6 |
| UI Validation TCs Included | 0 (intentionally excluded) |

---

## 5️⃣ Quality Summary

| Indicator | Status | Notes |
|---|---|---|
| Core Login Flow | Partial | Generic error message (BR-001) |
| Product Display | Issues Found | Sorting broken (BR-006), image mismatch (BR-007) |
| Cart Functionality | Mostly Working | State reset bug found (BR-004) |
| Checkout Flow | Critical Bug | Empty cart checkout allowed (BR-003) |
| Navigation | Partial | Footer links broken (BR-011) |
| UI / Layout | Multiple Issues | 7 visual bugs found |

### Overall Quality Verdict
> **Not ready for production** — 1 critical bug (BR-003) and 10 additional defects make this application unsuitable for release without fixes.

---

## 📈 Key Takeaways

- **Checkout is the riskiest module** — the empty cart checkout bug (BR-003) is a critical functional gap that could directly impact users and revenue in a real application
- **UI bugs are the most common** — 7 out of 11 bugs are visual, suggesting a rendering or CSS issue (likely tied to `problem_user` behavior in SauceDemo)
- **Cart module is the most stable** — 5/5 test cases passed with only one state sync issue found during exploratory testing
- **100% test execution achieved** — all 33 planned test cases were executed with no blockers

---

## 👨‍💻 Author
*Created as part of QA learning journey by Smrity Thapa*  
*Repository: https://github.com/Smrity-Thapa33/qa_fundamentals*
