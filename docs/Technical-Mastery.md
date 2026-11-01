# 🟨 Technical Mastery

Mastery is the ability to see the system through the syntax. Syntax lets you use a language. Mastery lets you predict what the running system will do, which other parts it touches, and under which conditions.

---

## 🔬 Low-level understanding

An abstraction moves complexity. It does not remove it. You do not need the source of every library you call. You do need the layer your solution depends on, well enough to judge quality and maintenance.

| Abstraction | The layer underneath |
|:---|:---|
| ORM | The SQL it emits, the plan, the indexes, the round trips, change tracking, and what two transactions do to the same row |
| HTTP client | Pools, timeouts, retries, and cancellation |
| Message broker | Delivery guarantee and ordering |
| Dependency injection | Lifetimes, scope, and disposal |
| Async code | Scheduling and synchronization |
| Distributed cache | Consistency, expiry, and invalidation |

An abstraction speeds the work. It does not stand in for the knowledge under it.

---

## 📚 Constant R&D

Spend about 10% of the working week on the How behind the What. The share moves with the role. The rule is that learning sits inside the work week, not only in leftover evenings.

Study one of these:

* How a framework feature actually behaves.
* An architecture you have not operated.
* A performance problem, down to the measurement.
* A small proof of concept.
* The limits of a library already in production.
* A newer tool only where it would change a current design.

Reading is the start. A small experiment is the check. Write down what you saw.

1. **Question.** Name the thing you cannot yet predict.
2. **Research.** Read the manual and the discussion around that mechanism.
3. **Experiment.** Build the smallest prototype that can fail.
4. **Evaluate.** Compare what you expected with what ran.
5. **Documentation.** Record where it applies, and where it breaks.

Not every experiment becomes production code. Learning that a candidate does not fit is a finished result.

---

## 🏗️ Architectural reasoning

A local implementation choice can bind the rest of the system. A new abstraction adds a dependency. A convenient integration adds a failure mode. A simple data shape can be expensive to change later. Reason about those consequences. Do not promote every task into an architecture review.

Judge the trade-off, not only the time to implement. Ask:

* What problem is this solving?
* Which assumptions does it require?
* What happens when one part fails?
* What changes when the system grows?
* What must operators do to run it?
* Can another engineer support it?
* When does this choice stop fitting?

There is no universal winner. The fitting option is the one whose costs the current system can carry.

When the decision will outlive the task, write it down. Use the [ADR template](../templates/ADR-Template.md): context, alternatives, the chosen shape, why, and the risk that remains. A decision that lives only in a chat does not exist for the next engineer.

---

## ⚠️ Anti-pattern: copy-paste engineering

Reusing a sample, a library, or generated code is normal. Shipping it without knowing why it works is the anti-pattern named on the T card.

The code can pass today's tests and still leave you unable to say:

* Why the original choice was made.
* Which assumptions it needs.
* Whether those assumptions hold here.
* Which dependencies it pulls in.
* How it fails.
* Whether it fits this architecture.

That shows up as lost context, extra layers, hidden assumptions, and debugging by guessing. The same risk applies to code an assistant generated. The engineer still checks the style of the system, the new dependencies, concurrency and failure, and whether the change fits the domain.

The check is one question: can you explain what this does, which assumptions it needs, and what breaks when those assumptions change? If not, stop and learn the layer before you merge it.

---

## What mastery is not

* Knowing every framework.
* A stack of finished courses.
* A count of lines written.
* A substitute for [Cognitive Clarity](../CRAFTER.md) or [Focus](../CRAFTER.md). Clarity names the problem. Focus protects the time. Mastery is the judgment that solves it.

---

## Where this shows up

* **Measure it** with Complexity Handling, Solution Quality, and Automation Ratio in [Metrics](../Metrics.md). These are diagnostic signals, not a scoreboard.
* **Check the week** against the T items in [Self-Assessment](../Self-Assessment.md).
* **Who carries it:** engineers, in [Roles](./Roles.md).
* **Record the decision** in an [ADR](../templates/ADR-Template.md).
