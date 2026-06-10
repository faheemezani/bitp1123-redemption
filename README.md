# BITP1123 — Lab Test Redemption Self-Check

Use this repository to check your redemption submission **before** the deadline.  
Within ~2 minutes of pushing your file, a bot will comment on your commit with your result.

---

## Who can use this?

Students who scored **below 6.5 / 7.5** on **Lab Test 1** or **Lab Test 2** and wish to resubmit for redemption.

> The redemption mark is **capped at 6.5 / 7.5** regardless of how well you score on resubmission.

---

## What to submit

| Lab Test | What to submit | Filename |
|----------|---------------|----------|
| **LT1** (Searching) | A **`.zip` file** containing all your `.cpp` source files | e.g. `B012345678.zip` |
| **LT2** (Sorting + Searching) | Your completed **`LT1_skeleton.cpp`** file directly | `LT1_skeleton.cpp` |

> ⚠️ **LT1: Do NOT submit a bare `.cpp` file — it must be a `.zip`.**  
> The grader expects your zip to contain the same set of source files as the original lab test.

---

## Step-by-step instructions

### 1 — Fork this repository

Click the **Fork** button (top-right of this page) and fork it to your personal GitHub account.  
Keep the repo **private** — do **not** share your submission with other students.

> To make your forked repo private after forking:  
> **Settings → General → Danger Zone → Change repository visibility → Private**

### 2 — Enable Actions on your fork

GitHub disables Actions on forks by default.

1. Go to your fork → **Actions** tab  
2. Click **"I understand my workflows, go ahead and enable them"**

### 3 — Prepare your submission file

**LT1:**
- Zip all your `.cpp` source files into a single `.zip` file
- Name the zip file using your student ID, e.g. `B012345678.zip`
- The zip should contain your `.cpp` files at the root level (not inside a subfolder)

**LT2:**
- Use your completed `LT1_skeleton.cpp` file

### 4 — Place your file in the `submission/` folder

- Delete the placeholder file `submission/PLACE_YOUR_FILE_HERE.txt`
- Copy your file (`.zip` for LT1, `.cpp` for LT2) into the `submission/` folder
- Only **one** submission file at a time

### 5 — Commit and push

```bash
git add submission/
git commit -m "Submit redemption"
git push
```

Or use GitHub Desktop / VS Code — just make sure the file lands in `submission/`.

### 6 — Check your commit comment

1. Go to your fork on GitHub
2. Click on your latest commit (the commit hash link near the top of the repo page)
3. Scroll down — the grader bot will have posted a comment, for example:

**LT1 result:**
```
✅ Redemption Result: 6.50 / 7.5 — Meets the cap
   LT1 | Set 3 | Raw: 7.20/7.5 → Capped: 6.50/7.5
```

**LT2 result:**
```
✅ Redemption Result: 6.50 / 7.5 — Meets the cap
   LT2 | Raw: 88/96 → Scaled: 6.88/7.5 → Capped: 6.50/7.5
```

---

## Notes

- You may push as many times as you like before the deadline — each push triggers a fresh check.
- The self-check result is **indicative only**. Your lecturer runs the official grader on your final submission.
- If the Actions tab shows a red ✗, check that you enabled Actions (Step 2) and that your file is inside `submission/`.
- For LT1, if the bot reports an unexpected result, check that your zip contains `.cpp` files at the root level with no extra subfolders.

---

## Deadline

Submit your **final** file to Moodle by the deadline communicated by your lecturer.  
Pushing to this repo does **not** count as an official submission.
