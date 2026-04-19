# 📊 Metrics Layer (CRAFTER)

> **"If you can't measure it, you can't improve it."** > Metrics in CRAFTER OS are used as **signals**, not as surveillance. They serve to diagnose the system and identify bottlenecks in execution.

---

## 🟦 C — Cognitive Clarity
*Measuring the quality of the mental model.*

* **Focus Level (1–10):** Subjective daily rating of how well you understood your tasks.
* **Context Switches:** Number of times you shifted between unrelated projects/tasks per day.  
    * *Target: < 3 major switches.*
* **Requirement Latency:** Time spent waiting for clarification before execution can start.

---

## ⬜ R — Reputation
*Measuring reliability and trust.*

* **Predictability Score:** Ratio of "Tasks Committed" vs. "Tasks Completed" per sprint.  
    * *Target: > 85%.*
* **Deadline Variance:** The average delta between the estimated and actual delivery date.
* **Stakeholder Trust Index:** Qualitative feedback on the clarity and frequency of updates.

---

## 🟩 A — Adaptation
*Measuring systemic flexibility.*

* **Pivot Speed:** Time taken to integrate a major change in requirements and resume execution.
* **Success Rate of Changes:** % of new processes or tools that were successfully adopted and improved the workflow.
* **Recovery Time:** How quickly the system returns to "Deep Work" after an unexpected incident (firefighting).

---

## 🟥 F — Focus
*Measuring the protection of cognitive resources.*

* **Deep Work Hours:** Total hours spent in a "No-Noise" environment.  
    * *Target: 2–4 hours daily.*
* **WIP Limit (Work In Progress):** Current active tasks.  
    * *Hard Rule: ≤ 3 tasks at any time.*
* **Notification Interruptions:** Count of unscheduled pings/distractions during deep work blocks.

---

## 🟨 T — Technical Mastery
*Measuring the evolution of craft.*

* **Complexity Handling:** Tracking the successful delivery of tasks with increasing architectural difficulty.
* **Solution Quality:** Number of regressions or bugs found in "Done" tasks within 30 days of release.
* **Automation Ratio:** Percentage of repetitive manual tasks successfully automated this month.

---

## 🟧 E — Execution
*Measuring raw output and velocity.*

* **Completion Rate:** Number of tasks moved to "Done" per cycle.
* **Lead Time:** Time from "Task Started" to "Task Delivered."
* **Stall Rate:** Number of tasks that stayed in "In Progress" for more than 48 hours without a commit.

---

## 🟪 R — Responsibility
*Measuring the depth of ownership.*

* **End-to-End Ownership:** % of tasks where the engineer handled everything from design to deployment/monitoring.
* **Proactivity Score:** Number of "Broken Windows" or technical debt items fixed outside assigned tasks.
* **System Stability:** Uptime or performance metrics of the specific components owned by the engineer.

---

## 📈 Metric Diagnostic Table

| Signal | Meaning | Action Required |
|:---|:---|:---|
| **Low Clarity + High Switches** | Burnout Risk | Stop all execution. Re-plan the week. |
| **High Execution + Low Quality** | Tech Debt Accumulation | Slow down. Focus on **Mastery**. |
| **Low Predictability** | Over-Promising | Reduce commitments. Fix **Reputation**. |
| **Low Deep Work** | Meeting Overload | Implement **Calendar Defense**. |

---

## 🛠 Tools for Tracking
- **Time Tracking:** (e.g., Toggl, RescueTime) for Deep Work hours.
- **Git Analytics:** (e.g., Linear, Jira, or custom scripts) for Lead Time and Predictability.
- **Self-Audit:** Use the [Daily Template](./templates/Daily-Checklist.md) to log Focus Levels.