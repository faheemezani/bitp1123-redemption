# BITP1123 — Lab Test Redemption Self-Check

Use this repository to check your fixed lab test submission before the redemption deadline.
Every time you push, the grader runs automatically and posts your result as a comment on your commit.

---

## Who is this for?

Students who scored **below 6.5 / 7.5** in their original lab test and have been given the opportunity to resubmit. The maximum mark you can receive through redemption is **6.5 / 7.5**, regardless of how well you do.

---

## How to submit your work

### Step 1 — Clone this repository

```bash
git clone https://github.com/YOUR_CLASSROOM_ORG/redemption-YOUR_STUDENT_ID.git
cd redemption-YOUR_STUDENT_ID
```

### Step 2 — Place your file in the `submission/` folder

The `submission/` folder is where the grader looks. Place **only your submission file** there — nothing else.

| Lab Test | What to put in `submission/` |
|---|---|
| **Lab Test 1** (Searching) | Your zip file: `B012345678_Set2.zip` |
| **Lab Test 2** (Sorting + Searching) | Your `.cpp` skeleton file: `B012345678_LT2.cpp` |

> ⚠️ Do not rename or restructure the `submission/` folder.
> Do not put multiple zip files in there — only your latest attempt.

### Step 3 — Commit and push

```bash
git add submission/
git commit -m "Submit redemption attempt"
git push
```

### Step 4 — Check your result

1. Go to your repository on GitHub.
2. Click on the latest commit (the message you just typed).
3. Scroll down — you will see a comment from **BITP1123 Grader Bot** with your marks.

You will also find a detailed feedback file inside the `FEEDBACK/` folder after the bot commits it back.

---

## Understanding your result

The commit comment will show one of these banners:

**You have met the cap:**
```
✅ Redemption Result: 6.50/7.5 — Meets the cap (6.5/7.5)
```

**You are below the cap — keep fixing:**
```
❌ Redemption Result: 5.25/7.5 — Below the cap (6.5/7.5)
```

Below the banner you will see your full breakdown, for example:

**Lab Test 1 (Searching):**
```
*** REDEMPTION SUBMISSION ***
Redemption cap: 6.5/7.5

1. File structure compliance [1.0/1.0]
2. Data setup & search loop [1.0/1.0]
3. First algorithm (Sentinel) implementation [1.5/1.5]
4. Binary Search implementation [2.0/2.0]
5. Integration & CHALLENGE element [1.5/1.5]
6. Code quality [0.5/0.5]
Raw score : 7.5/7.5
Capped at  : 6.5/7.5
TOTAL: 6.5/7.5
```

**Lab Test 2 (Sorting + Searching):**
```
*** REDEMPTION SUBMISSION — Lab Test 2 ***
Redemption cap: 6.5/7.5

Part A  Theory blanks (A1–A10)       [20.0/20.0]
Part B  Selection Sort               [20.0/20.0]
Part C  Bubble Sort                  [20.0/20.0]
Part D  Insertion Sort               [20.0/20.0]
Part E  Searching (Linear + Binary)  [16.0/16.0]
Raw score    : 96.0/96
Scaled score : 7.50/7.5  (96.0 / 96 × 7.5)
Capped at    : 6.5/7.5
TOTAL: 6.50/7.5
```

---

## You can push as many times as you like

Every push re-runs the grader. Use this to:
- Fix a bug and check whether it improved your score
- Confirm your final submission before the deadline

> ⚠️ Only your submission **before the deadline** counts. Pushing after the deadline will still run the grader and show you a result, but your lecturer will use the last push **before** the deadline.

---

## Common issues

**"No feedback file generated"**
Your submission file may be missing or in the wrong folder. Make sure your file is inside `submission/` and that you have committed and pushed it.

**"Target not found" for a value you expect to find**
Check that your array is initialised with the correct data from the lab test question.

**Compilation failed**
The grader will still score your theory answers (Part A for LT2) and any structural code analysis it can do. But you will lose marks on the implementation parts. Fix the compile error and push again.

**The grader detected the wrong lab test**
This should not happen if you placed your file correctly. If it does, let your lecturer know.

---

## Deadline reminder

Your redemption submission must be pushed **before the deadline set by your lecturer**.
Late pushes will be visible in the commit history but will not be accepted for marking.

---

*BITP1123 Data Structure and Algorithm | FTMK, UTeM*
