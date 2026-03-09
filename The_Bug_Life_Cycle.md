# 🐞 Technical Concept: The Bug Life Cycle
### The journey of a bug—from the moment you find it until it’s dead. 💀✅

---

## 🧠 The Big Picture
The Bug Life Cycle (or Defect Life Cycle) is the specific set of states a bug moves through. As a QA Tester, you are the **"Guardian"** of this cycle. You are the one who opens the door, and in most professional environments, you are the only one who can officially close it.



---

## 🔄 The Standard Flow (The Happy Path)
When a fix goes perfectly, the bug follows this 7-step journey:

1.  **NEW 🆕:** You find a bug (e.g., the Watch won't sync sleep data) and log it in Jira.
2.  **ASSIGNED 👤:** The Lead reviews it and assigns it to a specific Developer.
3.  **OPEN 🛠️:** The Developer starts analyzing the code and working on a solution.
4.  **FIXED ✅:** The Developer finishes the code change and marks it as "Fixed."
5.  **RETEST 🔍:** **(Crucial Step)** The bug comes back to you. You test the exact same scenario again.
6.  **VERIFIED ⭐:** You confirm the fix works. The "Actual Result" now matches the "Expected Result."
7.  **CLOSED 🏁:** The bug is officially dead. End of story.

---

## 🔁 The "Reality" Paths (Detours & Delays)
In the real world at places like **Google** or **HCLTech**, bugs often take messy detours:

* **REOPEN 😤:** You retest a "Fixed" bug and find it’s still broken. You kick it back to the developer.
* **REJECTED / INVALID 🤷:** The developer claims, *"This is working as intended"* or *"I can't reproduce this on my machine."*
* **DUPLICATE 🔁:** Another tester already reported this. (Always search Jira before logging!)
* **DEFERRED ⏸️:** The bug is real, but it’s not a priority for this release. It’s moved to the "Backlog."



---

## ⚔️ Summary: The Power Dynamics

| Action | Who Does It? | The Goal |
| :--- | :--- | :--- |
| **Log/Open** | Tester | To document the flaw. |
| **Fix/Repair** | Developer | To correct the code. |
| **Retest/Verify**| Tester | To ensure the fix actually worked. |
| **Close** | Tester | To finalize and archive the issue. |

---

## 🧪 The QA Brain Moment (Interview Gold) 🧠
If an interviewer asks: *"What do you do if a developer marks a bug as Fixed, but it still fails during your retest?"*
**The Answer:** "I change the status to **REOPEN**, attach a fresh screenshot or log of the failure, and leave a comment explaining exactly why the fix failed. I never move a failing bug to Closed."

---

### 💡 One-Line Lock-in:
**The Tester opens the bug; the Developer fixes the bug; but ONLY the Tester can close the bug.**

markdown
# 🐞 The Bug Life Cycle
### N-A-O-F-R-V-C: The Professional Sequence

---

## 🚀 The Main Stages
* **NEW:** Bug is reported.
* **ASSIGNED:** Developer is chosen.
* **OPEN:** Developer is working on it.
* **FIXED:** Developer thinks it's done.
* **RETEST:** Tester checks the fix.
* **VERIFIED:** Fix is confirmed working.
* **CLOSED:** Bug is finalized.

---

## ⚠️ The Deviations
* **REOPEN:** Fix failed; send it back.
* **REJECTED:** Not a bug or won't fix.
* **DEFERRED:** Will fix in a later version.
* **DUPLICATE:** Already exists in the system.

---

### 💡 One-Line Takeaway:
**A bug is only dead when the Tester says it's dead.**
