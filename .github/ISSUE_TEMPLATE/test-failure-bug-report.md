---
name: "🐛 Test Case Failure - Bug Report"
about: Report a bug from a failed test case in TestPlanIt
title: "[BUG] <Test Case Name> - <Short Failure Summary>"
labels: bug, test-failure
assignees: ''
---

## 🐛 Bug Report — Test Case Failure

> **Instructions:** Fill in all sections below. Copy the test case name, steps, and results from TestPlanIt. Delete any steps that are not part of your test case.

---

### 📋 Test Case Information

| Field              | Details                          |
|--------------------|----------------------------------|
| **Test Case Name** | <!-- e.g. Registration Failure - Invalid Indian Mobile Number Format --> |
| **Test Run ID**    | <!-- e.g. Run #3/5 -->           |
| **Configuration**  | <!-- e.g. Mozilla Firefox -->    |
| **Overall Status** | ❌ Failed                        |
| **Reported By**    | <!-- Your name / TestPlanIt user --> |
| **Date**           | <!-- YYYY-MM-DD -->              |

---

### 🔁 Steps to Reproduce

> Copy each step from your TestPlanIt test case below. Mark the failing step with ❌.

---

#### Step 1
**Action:**
<!-- e.g. Navigate to the e-commerce website registration page. -->

**Expected Result:**
<!-- e.g. The registration form is displayed. -->

**Actual Result:**
<!-- ✅ Passed / ❌ Failed - describe what actually happened -->

**Status:** <!-- ✅ Passed | ❌ Failed | ⏭️ Skipped -->

---

#### Step 2
**Action:**
<!-- e.g. Fill all required fields with valid data, except for the 'Mobile Number' field. -->

**Expected Result:**
<!-- e.g. All fields except 'Mobile Number' are populated correctly. -->

**Actual Result:**
<!-- ✅ Passed / ❌ Failed - describe what actually happened -->

**Status:** <!-- ✅ Passed | ❌ Failed | ⏭️ Skipped -->

---

#### Step 3
**Action:**
<!-- e.g. Enter an invalid Indian mobile number (e.g., '12345' - too short, 'abcdefghij' - non-numeric, '0123456789' - invalid starting digit). -->

**Expected Result:**
<!-- e.g. The 'Mobile Number' field accepts the input, but no immediate error should prevent typing. -->

**Actual Result:**
<!-- ✅ Passed / ❌ Failed - describe what actually happened -->

**Status:** <!-- ✅ Passed | ❌ Failed | ⏭️ Skipped -->

---

#### Step 4
**Action:**
<!-- e.g. Click the 'Register' or 'Sign Up' button. -->

**Expected Result:**
<!-- e.g. The registration fails. An error message such as 'Please enter a valid Indian mobile number' is displayed. The user remains on the registration page. -->

**Actual Result:**
<!-- ✅ Passed / ❌ Failed - describe what actually happened -->

**Status:** <!-- ✅ Passed | ❌ Failed | ⏭️ Skipped -->

---

#### Step 5 *(if applicable)*
**Action:**
<!-- Add step action here -->

**Expected Result:**
<!-- Add expected result here -->

**Actual Result:**
<!-- Add actual result here -->

**Status:** <!-- ✅ Passed | ❌ Failed | ⏭️ Skipped -->

---

#### Step 6 *(if applicable)*
**Action:**
<!-- Add step action here -->

**Expected Result:**
<!-- Add expected result here -->

**Actual Result:**
<!-- Add actual result here -->

**Status:** <!-- ✅ Passed | ❌ Failed | ⏭️ Skipped -->

---

### ❌ Failure Summary

**Which step failed?**
<!-- e.g. Step 4 -->

**What went wrong?**
<!-- Clear description of what the actual (broken) behaviour was -->

**Error message (if any):**
```
Paste any error messages or console logs here
```

---

### 📸 Attachments

<!-- Drag and drop screenshots or screen recordings here -->
- [ ] Screenshot of failure attached
- [ ] Console log attached *(if applicable)*
- [ ] Video recording attached *(if applicable)*

---

### 🌍 Environment

| Field              | Details              |
|--------------------|----------------------|
| **Browser**        | <!-- e.g. Mozilla Firefox 125 --> |
| **OS**             | <!-- e.g. Windows 11 --> |
| **App Version**    | <!-- e.g. v2.1.0 --> |
| **Test Environment** | <!-- e.g. Staging / Production --> |

---

### 🔗 TestPlanIt Reference

| Field              | Details              |
|--------------------|----------------------|
| **TestPlanIt URL** | <!-- Paste the TestPlanIt test run URL here --> |
| **Test Run Link**  | <!-- e.g. bhargavqa.testplanit.com/en-US/projects/runs/3/5 --> |

---

### 🏷️ Priority Assessment

- [ ] 🔴 **Critical** — System crash / data loss / security issue
- [ ] 🟠 **High** — Core feature broken, no workaround
- [ ] 🟡 **Medium** — Feature broken but workaround exists
- [ ] 🟢 **Low** — Minor UI/UX issue
