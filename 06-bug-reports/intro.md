# 🐞 Bug / Defect Life Cycle (Manual QA Guide)

## 📑 Table of Contents

- [What is a Bug / Defect?](#what-is-a-bug--defect)
- [Severity vs Priority](#severity-vs-priority)
- [Bug / Defect Life Cycle](#-bug--defect-life-cycle)
- [How to Write an Effective Bug Report](#how-to-write-an-effective-bug-report)
- [Severity vs Priority](#severity-vs-priority)
- [Conclusion](#conclusion)

## What is a Bug / Defect?
A **bug (defect)** is a deviation between the **expected result** and the **actual result** of a software application.

- **Expected Result:** What the system is supposed to do 
- **Actual Result:** What the system actually does 

### Example:
If a user enters valid credentials but cannot log in, it is a defect.

---

## Severity vs Priority

### 🔴 Severity (Impact of the bug)
Severity defines how serious the bug is from a **technical perspective**.

| Severity Level | Description | Example |
|----------------|-------------|---------|
| Critical | System crash or data loss | App crashes on launch |
| High | Major functionality broken | Login not working |
| Medium | Feature partially working | Filter not working properly |
| Low | Minor UI issue | Typo in text |

---

### 🔵 Priority (Urgency to fix)
Priority defines how quickly the bug should be fixed from a **business perspective**.

| Priority Level | Description | Example |
|----------------|-------------|---------|
| High | Must be fixed immediately | Payment failure |
| Medium | Should be fixed soon | UI misalignment |
| Low | Can be fixed later | Minor text issue |

---

### Key Difference
- **Severity** → Technical impact 
- **Priority** → Business urgency 

A bug can have different combinations:
- High severity + Low priority 
- Low severity + High priority 

---
## 🔄 Bug / Defect Life Cycle

The Bug Life Cycle describes the journey of a defect from detection to closure.

### Stages:

### 1. New
- Tester identifies and logs the bug

---

### 2. Assigned
- Bug is assigned to a developer

---

### 3. Open
- Developer starts analyzing the bug

---

### 4. Fixed
- Developer fixes the bug and marks it as resolved

---

### 5. Retest / Verification
- QA retests the bug to verify the fix

---

### 6. Closed
- If the bug is resolved successfully, it is closed

---

### Additional States

| State | Description |
|------|-------------|
| Reopened | Bug still exists after fix |
| Rejected | Not a valid bug |
| Duplicate | Same bug already exists |
| Deferred | Fix postponed for future release |

---

# How to Write an Effective Bug Report

A professional bug report should be:
- Clear and concise 
- Easy to reproduce 
- Well-structured 
- Evidence-based 

---

## Standard Bug Report Format
- **Bug Report ID:** BR-001
- **Title:** A short and meaningful summary of the defect.
- **Environment:** Details of the system where the bug occurred:
  - Browser 
  - Operating System 
  - Device 
  - Application version
- **Steps to reproduce:** Clear step-by-step instructions
- **Expected result:** What should happen
- **Actual result:** What is happening
- **Severity:** Low/ Medium/ High/ Critical
- **Priority:** Low/ Medium/ High
- **Attachments:** Include supporting evidence:
  - Screenshots 
  - Screen recordings 
  - Logs (if available)

---
## Sample Bug Report Example
- **Bug Report ID:** BR-0001
- **Title:** Login fails with valid credentials
- **Environment:** 
  - Browser: Chrome 
  - OS: Windows 10

- **Steps to Reproduce:**
  1. Open login page 
  2. Enter valid username and password 
  3. Click Login 

- **Expected Result:**
User should be successfully logged in and redirected to dashboard.

- **Actual Result:**
Error message “Invalid credentials” appears.

- **Severity:** High 
- **Priority:** High

---

# Conclusion
Bug reporting is one of the most critical skills in Manual QA. A well-written bug report improves communication between QA and developers and directly impacts software quality.

Mastering this skill is essential for becoming a job-ready QA engineer.

---

## 👨‍💻 Author
Created as part of QA learning journey by Smrity Thapa.
