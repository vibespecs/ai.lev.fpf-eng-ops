# OPS.8.1 - Choose Work-Release Rules When Earlier Work Can Return: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.8.1:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.8.1:5.1 - An analysis returns during the next client session {#an-analysis-returns-during-the-next-client-session}

A specialist finishes report X at hour zero. A review at hour one will either accept it or identify a correction requiring two uninterrupted specialist-hours. If a correction is needed, the corrected report is required by hour three. These are the two stated possibilities; the correction input becomes usable at hour one.

New job Y is a four-hour live session using the same specialist throughout. It is ready at zero, can start at any suitable time, must finish by hour seven and cannot be paused to perform X. Other resources do not change these conditions.

Releasing Y to run at 0–4 on X's first completion gives X no correction window before three. In the return case, the earliest correction is 4–6. The completion signal did not remove X's possible resource need.

A rule that preserves X's 1–3 correction window works as follows:

| Feedback at hour one | Specialist's next work | Completion of Y |
| --- | --- | ---: |
| X accepted | Start Y at 1 and finish at 5. | 5 |
| X needs correction | Correct X at 1–3; run Y at 3–7. | 7 |

The same observable rule handles both possibilities. It costs one hour of delayed Y completion in the no-return case relative to starting at zero. Holding a loop place until review and returning the place earlier while separately preserving the correction window can implement the same resource decision.

If Y instead needs one uninterrupted hour, with the other conditions unchanged, it can run at 0–1 and leave the same 1–3 correction window. Waiting for review before starting that Y would add delay without improving the stated protection of X.

Change the review time to hour two while retaining X's deadline three and its two-hour correction. Even an idle specialist can now finish that correction only at four. Keeping Y outside the system does not repair this obstruction. The operation needs earlier usable feedback, a genuinely shorter correction or a changed commitment.

### OPS.8.1:5.2 - A free place and a full receiving resource {#a-free-place-and-a-full-receiving-resource}

A manufacturing resource S is available continuously from 0 to 5. Job A is already running there from 0 to 2. A part X undergoing inspection elsewhere may need one additional two-hour visit to S; the answer becomes available at hour one, and any such visit must be complete by five.

A new job Y would require two uninterrupted hours at S and is also wanted by five. Its upstream activity has space and emits a release signal. There are no other operations needed for these completions.

Protecting the stated return and promising Y requires 2 + 2 + 2 = 6 hours in a five-hour window. The free upstream place does not remove this obstruction.

At hour one, one hour of A remains. If X is accepted, the remaining requirement is one hour of A plus two of Y; A finishes at two and Y runs 2–4. If X returns, its visit can run 2–4, but Y cannot also finish by five. Replacing the two-hour return allowance with X's known visit preserves this result; adding both would falsely claim eight original hours of demand.

This example uses full occupied hours and a finite deadline. A workload norm based on a different weighted quantity would need its own interpretation. If Y instead used an independent resource, holding it because of S's protected hours would require another reason.

### OPS.8.1:5.3 - Waiting for an event that cannot consume the resource {#waiting-for-an-event-that-cannot-consume-the-resource}

An operation completes a job inside a machining loop. The remaining customer acknowledgment will use a separate administrative service, and the operating arrangement excludes any further use of the machining loop for this job in the horizon under consideration. The next eligible part has the required resources and fits the loop's release rule.

Keeping the machining-loop card until that acknowledgment would postpone the part without protecting any machining work in the stated horizon. Return the card at the loop's completion and retain the customer's outstanding acknowledgment in its own account. If inspection can instead return the part to that machine, this premise is lost and the release decision reopens.

## OPS.8.1:6 - Bias-Annotation {#bias-annotation}

A board or card encourages attention to visible membership. Keep the resource work that survives a boundary crossing. Conversely, a policy designed around a painful return can retain every item until remote final acceptance; test whether that event can still change the protected resource use.

Expected load can make correlated returns appear manageable. Use the return pattern needed for the actual consequence. The cases above establish conditional consequences under stated inputs; they do not estimate how often corrections occur in a real operation.

## OPS.8.1:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Mistake | Consequence | Repair |
| --- | --- | --- |
| Treating a local completion as the end of resource responsibility | A new long job displaces an earlier correction. | Retain the remaining and contingent resource demands after that event. |
| Holding every place until remote final acceptance | Unrelated acknowledgment delays useful service. | Choose the controlled loop and retain obligations outside it in their own account. |
| Reserving for a return and then adding the same work again | Artificial overload blocks usable capacity. | Replace the matching allowance when the return becomes known. |
| Calling a mean return load protective | A burst or correlated return defeats the promised deadline. | Test the scenario, bounded family or joint probability required by that promise. |
| Resetting the customer's clock when work returns | A policy appears faster by losing earlier waiting. | Separate visit intervals from the original receiving interval. |

## OPS.8.1:10 - Architectural Rationale {#architectural-rationale}

A release rule can permit new work at local completion while the customer's result still requires another resource or a later visit. The method therefore couples that event with the work still needed and with the consequence of the next start.

The comparison works in both directions. Requirements of the receiving result constrain local starts; actual readiness and resource windows constrain the delivery that can be supported. A specialist's service, a loop's population and the customer's result can retain different boundaries without becoming inconsistent.

The rule need not model every future complaint. Its horizon and service question determine which returns matter. Distinguishing a known visit, a contingent allowance and new work makes updates local and keeps counts from replacing the work they are intended to regulate.

## OPS.8.1:11 - SoTA-Echoing {#sota-echoing}

For the question “may this new job start while earlier work can return?”, the selected line combines a defined release signal with the remaining resource demand and the required service. Two simpler alternatives are one-in/one-out counting and waiting for final acceptance. The first can omit consequential load; the second can delay work without protecting that service. Sections 4.1–4.5 add the event, load, timing and feedback operations needed to decide between them. Cases 5.1–5.3 demonstrate different outcomes, including a condition under which holding capacity cannot help.

Hopp and Spearman, *Factory Physics*, third edition, §10.4 and §§14.3.1–14.3.2, supply CONWIP's controlled-loop construction and the distinction between counting jobs and accounting for unequal resource demands. Adopt the loop boundary and adapt the treatment of work diverted for rework: freeing a card requires retaining whichever other admission and load rules govern that work. No universal final-customer-acceptance boundary is inferred.

Steve Tendon, *The Book of TameFlow* (2022), printed pp. 117 and 138, supplies a concrete contrast: a constrained team's completion triggers replenishment, while the teaching exercise also permits a customer return for reprocessing and retains elapsed project time. Adopt the separate signal and customer-clock operations. Adapt the release choice to the actual return resource and timing through sections 4.2–4.5; the exercise does not establish that every operation can absorb any later correction.

[Thürer and Stevenson, *Workload Control in Job Shops with Re-entrant Flows: An Assessment by Simulation*](https://eprints.lancs.ac.uk/id/eprint/78334/1/Thurer_and_Stevenson_IJPR_Manuscript_Text_Figures_and_Tables.pdf), §§3.2 and 4.3–4.4, compare load accounting and release behavior for known repeated visits. Their corrected load weights route positions, and a starvation-triggered exception can exceed a norm. Adopt explicit repeated-visit accounting; distinguish that congestion policy from the finite occupied-hours test in 4.3. The study does not supply the timing or distribution of an as-yet-undiscovered correction.

[Prabhu and colleagues (2024)](https://doi.org/10.2478/mspe-2024-0014), the REM subsection on printed p. 149 and comparison on pp. 152–153, combine regular and re-entrant workload in a release rule. Adapt that combined-load comparison in 4.2–4.3: possible corrections still awaiting discovery need an allowance or scenario in addition to known visits, and resource-specific time limits remain. The study's rankings differ for flow time, throughput and modeled profit, supporting the receiving-question comparison in 4.4. Its rotor-blade simulation does not select a universally best rule. The occupied-hours screen here is an accounting bound followed by placement, rather than a protection claim inferred from an average population-time relation.

Reopen the selection when another signal or accounting method supports the same receiving result with less delay, information or coordination, or when returns, resource sharing, interruption, feedback timing or service requirements change. Compare outcomes at the original customer boundary; changing that boundary is not evidence that the rule improved service.


## OPS.8.1:End {#end}
