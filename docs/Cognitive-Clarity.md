# 🟦 Cognitive Clarity

The quality of the code cannot exceed the quality of the mental model. Real engineering starts before the editor, when two boundaries are explicit: what is being built, and how anyone will know it is done.

Clarity is a protocol, not a mood. If you cannot explain the why and the how, you are not ready to write the code.

---

## 🧱 First-principles thinking

Take the task apart into the constraints that are actually true. A pattern from the last project, or a sample found online, is not one of those constraints.

Separate the domain problem from the tools wrapped around it. Name where this task ends and the next service begins. An error is a signal that a boundary or a contract is wrong, not only a line to patch.

A task is ready to design when its invariants can be stated without the framework in the sentence.

---

## ✂️ Radical simplification

If the logic cannot be explained in about two minutes, it is not understood yet. Map the flow, the states, or the steps on paper or in a short note before opening the editor. A task that cannot be mapped is not ready.

When the map has been spinning for more than 20 minutes without a path, stop. Remap it, then ask for the missing fact. The daily form of that stop is in the [Playbook](../Playbook.md).

---

## ✅ Definition of Done awareness

The finish line is agreed before the first line of code. A two-line ticket is not that agreement.

* **Product.** Which invariants must hold, and which edge cases are in scope?
* **Process.** Which gates are required: tests, review, a migration, docs?

Questions about a basic business rule after implementation has started, a scope that moves because an edge case was never named, and a pull request rewritten because two people read the domain differently are signs the definition was missing.

---

## ⚠️ Anti-pattern: guess-driven development

Guess-driven development starts from a vague problem and expects the code to reveal the requirement. It sounds like "I think it should work something like this," or "the ticket already says it" when the ticket is two unverified lines.

The cost is code and reviews that get rewritten, temporary fixes that stay, and delivery promises that shrink after release. Pasting that thin ticket into an assistant and accepting a large change you cannot explain is the same anti-pattern.

An assistant can draft options and a record. It does not own the decision. The engineer checks that the result respects the invariants, then writes the choice in an [ADR](../templates/ADR-Template.md) when the decision will outlive the task.

---

## What clarity is not

* A burst of inspiration.
* A long design document for every small change.
* A substitute for [Focus](./Focus.md) or [Technical Mastery](./Technical-Mastery.md). You cannot protect time on a problem you have not named, and you cannot judge a layer you have not understood.

---

## Where this shows up

* **Measure the conditions**, not the person: Focus Level, Context Switches, and Requirement Latency in [Metrics](../Metrics.md). A low understanding of the task means stop and remap before writing more code.
* **Check the week** against the C items in [Self-Assessment](../Self-Assessment.md).
* **Run the day** from the pre-flight in the [Playbook](../Playbook.md): name the outcomes, give each a definition of done, then protect the block.
* **Who carries it:** architects, in [Roles](./Roles.md). The written decision itself is the [ADR template](../templates/ADR-Template.md).
