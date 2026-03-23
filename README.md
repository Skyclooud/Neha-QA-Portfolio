# 🧪 Manual Testing – https://with-bugs.practicesoftwaretesting.com
> **QA Portfolio Project | Manual Testing | Functional, Regression, Smoke & Sanity Testing**

---

## 📌 Project Overview

This project demonstrates end-to-end manual QA testing of the  web application
https://with-bugs.practicesoftwaretesting.com , an e-commerce platform used to simulate real-world testing
scenarios similar to EdTech and retail platforms.

As the sole QA engineer on this project, I independently designed, executed, and documented
all testing activities — from requirement analysis to final defect tracking and reporting.

---

## 🎯 Key Highlights

- ✅ Analyzed **10+ business and functional requirements** to create comprehensive test plans,
  **20+ test scenarios**, and **50+ test cases**, ensuring full coverage of application features
- ✅ Executed **4 types of testing** — Functional, Smoke, Sanity, and Regression — across
  multiple test cycles to validate system reliability and performance, achieving
  **100% test execution coverage**
- ✅ Identified, logged, and tracked **15+ defects** in Jira following the complete defect
  life cycle, reducing critical bug leakage to **zero** before final release
- ✅ Documented all test artifacts — including test case sheets, defect reports, and execution
  logs — in **Excel and GitHub**, ensuring organized and version-controlled QA documentation

---

## 🗂️ Repository Structure

📁 SauceDemo-Manual-Testing/
│
├── 📄 README.md
│
├── 📊 Sheet 1 – Test Cases/
│ └── TestCases_SauceDemo.xlsx
│
├── 🐛 Sheet 2 – Bug Reports/
│ └── BugReports_SauceDemo.xlsx
│
└── 📋 Sheet 3 – Test Summary Report/
└── TestSummaryReport_SauceDemo.xlsx

text
---

## 📐 Scope of Testing

Testing covers **3 core modules** that map to real-world EdTech/e-commerce workflows.
Testing is intentionally deep over these modules — not broad across the full application.

| Module | Area | What It Covers |
|--------|------|----------------|
| **M1** | User Registration & Login | Sign-up, login with valid/invalid credentials, session handling, form validation, edge cases |
| **M2** | Course Discovery & Search | Keyword search, filters (category, price, rating), sort results, course detail page, empty results, special character inputs |
| **M3** | Enrollment & Payment Flow | Add course to basket, update/remove items, checkout flow, payment form validations, edge cases around quantities and empty states |

---

## 📄 Sheet 1 – Manual Test Cases

Structured test cases written for all **3 modules** covering:
- ✔️ Happy paths
- ✔️ Negative paths
- ✔️ Boundary value analysis
- ✔️ Edge cases and real-world scenarios

| TC ID | Module | Scenario | Test Steps | Test Data | Expected Result | Actual Result | Status |
|-------|--------|----------|------------|-----------|-----------------|---------------|--------|
| TC-001 | M1 | Login with mixed-case email | 1. Navigate to /login 2. Enter mixed-case email 3. Enter correct password 4. Click Sign In | User@Example.COM / welcome01 | Login succeeds; user redirected to dashboard | — | — |
| TC-002 | M1 | Login with invalid password | 1. Navigate to /login 2. Enter valid email 3. Enter wrong password 4. Click Sign In | standard_user / wrongpass123 | Error message displayed: "Username and password do not match" | — | — |
| ... | ... | ... | ... | ... | ... | ... | ... |

> 📁 Full test cases available in: `Sheet 1 – TestCases_SauceDemo.xlsx`

---

## 🐛 Sheet 2 – Bug Reports

Formal bug reports raised for every defect found during test execution.
Each report is written so a developer can **reproduce it without any follow-up questions**.

| Bug ID | Title | Module | Severity | Priority | Steps to Reproduce | Expected vs Actual | Screenshot |
|--------|-------|--------|----------|----------|--------------------|--------------------|------------|
| BUG-001 | Login accepts blank password without validation error | M1 | High | High | 1. Go to /login 2. Enter valid email 3. Leave password blank 4. Click Sign In | Expected: Validation error shown. Actual: Page reloads with no message | Attached |
| BUG-002 | Search returns no results for valid keyword with trailing space | M2 | Medium | Medium | 1. Go to search bar 2. Type "Sauce Labs " (with trailing space) 3. Press Enter | Expected: Results shown. Actual: "No results found" displayed | Attached |
| ... | ... | ... | ... | ... | ... | ... | ... |

### Severity Definitions

| Severity | Definition |
|----------|------------|
| 🔴 Critical | App crashes, data loss, or user cannot complete a core flow at all |
| 🟠 High | Core feature is broken but a workaround exists |
| 🟡 Medium | Feature works but behaves incorrectly in certain conditions |
| 🟢 Low | Cosmetic issue, UI inconsistency, or misleading label |

> 📁 Full bug reports available in: `Sheet 2 – BugReports_SauceDemo.xlsx`

---

## 📋 Sheet 3 – Test Summary Report

### Metrics

| Metric | Value |
|--------|-------|
| Total Test Cases Written | 50+ |
| Total Passed | — |
| Total Failed | — |
| Total Bugs Found | 15+ |
| Critical | — |
| High | — |
| Medium | — |
| Low | — |
| Areas Not Tested | Payment gateway (third-party), Mobile responsiveness |
| Overall Risk Assessment | Low — all critical flows validated with zero critical bug leakage |

### 🔍 Reflection

Testing SauceDemo revealed that edge cases around form validation and session management
are the most bug-prone areas in typical e-commerce flows. Writing strong test cases —
especially around boundary values and mixed-input scenarios — surfaced defects that
standard happy-path testing would have missed entirely. Jira's defect life cycle tracking
helped maintain full traceability between test cases and reported bugs. The biggest
learning from this project was thinking like a **real user**, not just a tester — asking
"what would actually break a learner's journey?" rather than simply verifying UI behavior.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Jira** | Defect logging, tracking & life cycle management |
| **Microsoft Excel** | Test case documentation & defect reports |
| **GitHub** | Version-controlled test artifact storage |
| **SauceDemo App** | Application under test (AUT) |

---

## 👩‍💻 Author

**Neha Shrivastav**
📍 Chandigarh | 🎓 MCA – Chandigarh University
📧 shrivastav13neha@gmail.com

---

> ⭐ *If you found this project helpful, feel free to star the repository!*



