# BITP1123 — Lab Test Redemption Self-Check

Use this repository to check your redemption submission **before** the deadline.  
Within ~2 minutes of pushing your file, a bot will comment on your commit with your result.

---

## Who can use this?

Students who scored **below 6.5 / 7.5** on **Lab Test 1** or **Lab Test 2** and wish to resubmit for redemption.

> The redemption mark is **capped at 6.5 / 7.5** regardless of how well you score on resubmission.

---

## Step-by-step instructions

### 1 — Fork this repository

Click the **Fork** button (top-right of this page) and fork it to your personal GitHub account.  
Keep the repo **private** — do **not** share your submission with other students.

> To make your forked repo private:  
> Settings → General → Danger Zone → Change repository visibility → Private

### 2 — Enable Actions on your fork

GitHub disables Actions on forks by default.

1. Go to your fork → **Actions** tab  
2. Click **"I understand my workflows, go ahead and enable them"**

### 3 — Prepare your file

| Lab Test | What to submit |
|----------|---------------|
| LT1 (Searching) | Your `.cpp` source file, named `STUDENTID_SetX.cpp` (e.g. `B012345678_Set3.cpp`) |
| LT2 (Sorting + Searching) | Your completed `LT1_skeleton.cpp` file |

### 4 — Place your file in the `submission/` folder

- Delete the placeholder file `submission/PLACE_YOUR_FILE_HERE.txt`
- Copy your file into the `submission/` folder
- Only **one** file at a time

### 5 — Commit and push

```bash
git add submission/
git commit -m "Submit redemption"
git push
```

Or use GitHub Desktop / VS Code — just make sure the file lands in `submission/`.

### 6 — Check your commit comment

1. Go to your fork on GitHub
2. Click on your latest commit (the commit hash link)
3. Scroll down — the grader bot will have posted a comment like:

```
## 🎓 BITP1123 Redemption Self-Check

✅ Redemption Result: 6.50 / 7.5 — Meets the cap
   LT1 | Set 3 | Raw: 7.20/7.5 → Capped: 6.50/7.5
```

or

```
❌ Redemption Result: 4.80 / 7.5 — Below the cap (minimum 6.5 required)
```

---

## Notes

- You may push as many times as you like before the deadline — each push triggers a fresh check.
- The self-check result is **indicative only**. Your lecturer runs the official grader on your final submission.
- If the Actions tab shows a red ✗, check that you enabled Actions (Step 2) and that your file is inside `submission/`.

---

## Deadline

Submit your **final** file to Moodle by the deadline communicated by your lecturer.  
Pushing to this repo does **not** count as an official submission.
