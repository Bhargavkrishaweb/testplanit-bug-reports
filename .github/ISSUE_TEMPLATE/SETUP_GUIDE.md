# 📁 GitHub Issue Template — Setup Guide
## For TestPlanIt × GitHub Integration

---

## What's Included

```
.github/
└── ISSUE_TEMPLATE/
    ├── test-failure-bug-report.md   ← Main bug report template
    └── config.yml                   ← Disables blank issues, enforces template use
```

---

## How to Upload to Your GitHub Repository

### Option A — Upload via GitHub Web UI (Easiest)

1. Open your GitHub repository
2. Click **Add file → Create new file**
3. In the filename box, type exactly:
   ```
   .github/ISSUE_TEMPLATE/test-failure-bug-report.md
   ```
4. Paste the contents of `test-failure-bug-report.md` into the editor
5. Click **Commit changes**
6. Repeat for `config.yml` using the path:
   ```
   .github/ISSUE_TEMPLATE/config.yml
   ```

### Option B — Upload via Git (Command Line)

```bash
# In your local repo folder:
mkdir -p .github/ISSUE_TEMPLATE

# Copy the two files into that folder, then:
git add .github/ISSUE_TEMPLATE/
git commit -m "Add TestPlanIt bug report issue template"
git push origin main
```

---

## How to Use the Template

### When Creating a GitHub Issue Directly

1. Go to your GitHub repo → **Issues → New Issue**
2. You will see **"🐛 Test Case Failure - Bug Report"** — click **Get started**
3. The template pre-fills with all sections and step placeholders
4. Fill in the test case details from TestPlanIt and submit

### When Creating via TestPlanIt's "Link GitHub Issue" Button

Since TestPlanIt's Create Issue dialog has a plain Description box:

1. Click **"+ Link GitHub Issue"** on the failed test case
2. Click **"+ Create New Issue"**
3. For the **Title**, use the format:
   ```
   [BUG] <Test Case Name> - <Short Failure Summary>
   ```
4. For the **Description**, paste this quick format:
   ```
   **Test Case:** <name>
   **Run:** <run ID> | **Config:** <browser>

   **Step 1:** <action> → Expected: <result> ✅/❌
   **Step 2:** <action> → Expected: <result> ✅/❌
   **Step 3:** <action> → Expected: <result> ✅/❌
   **Step 4:** <action> → Expected: <result> ✅/❌

   **Failed at Step:** <number>
   **Actual Result:** <what went wrong>
   ```
5. Click **Create** — the issue appears in GitHub with step details

---

## Customisation Tips

- **Add more steps:** Duplicate any Step block in `test-failure-bug-report.md`
- **Remove steps:** Delete unused Step sections before committing
- **Change labels:** Edit the `labels:` line at the top of the template file
- **Auto-assign:** Add a GitHub username to `assignees:` at the top of the template

---

## Quick Copy — TestPlanIt Description Template

Use this when filling in TestPlanIt's Create Issue description box:

```
**Test Case:** [PASTE TEST CASE NAME]
**Run ID:** [PASTE RUN ID] | **Browser:** [PASTE BROWSER]
**Status:** ❌ Failed

---
**Step 1:** [ACTION]
↳ Expected: [EXPECTED RESULT]
↳ Actual: ✅ Passed

**Step 2:** [ACTION]
↳ Expected: [EXPECTED RESULT]
↳ Actual: ✅ Passed

**Step 3:** [ACTION]
↳ Expected: [EXPECTED RESULT]
↳ Actual: ✅ Passed

**Step 4:** [ACTION]
↳ Expected: [EXPECTED RESULT]
↳ Actual: ❌ FAILED — [DESCRIBE WHAT WENT WRONG]

---
**Error Message:** [PASTE ERROR IF ANY]
**TestPlanIt URL:** [PASTE URL]
```
