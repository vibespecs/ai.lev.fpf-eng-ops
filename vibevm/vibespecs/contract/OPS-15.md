# OPS.15 - Build a Decision-Specific Operating Account {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.15:1 - Problem frame {#problem-frame}

**Use this when** an operating decision cannot be supported by the available account: figures disagree, a denominator excludes important work, events from different services are combined, or a dashboard does not show the fact that could change the next action.

Begin by writing the decision and the observation that could change it. Then recover the actual subject, population and time basis. The first useful result is an operating account: the selected observations, their meaning and limits, and the claim they support for that decision. It can be a short table, an existing record or a view in the current tool.

This pattern governs the construction and maintenance of that account within continuing operations. It does not choose every action the account can inform. Use an adequate existing account directly when its meaning and evidence fit. Statistical estimation, causal investigation or a professional acceptance judgment needs its own method when the receiving claim requires it.

Suppose forty service requests have all reached their due dates. Twenty-seven finished on time, three finished late and ten remain open. Reporting 27 out of 30 completed requests as “90% on time” leaves the overdue open work out of the service judgment. The due-request account shows 27 out of 40, or 67.5%. Recovering the question changes which of these true calculations is useful.

## OPS.15:2 - Problem {#problem}

Available records often reflect the tool that generated them. A board counts matters, a rig log counts attempts, an invoice records an amount due and a payment account records a receipt. Combining them without their subject and event meanings can produce an apparently precise but unusable conclusion.

More collection can make the problem worse when it increases reporting effort without resolving the choice. The practitioner needs enough evidence to support the actual decision and preserve necessary assurance or recovery.

## OPS.15:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| useful summary and retained meaning | A compact number can hide the population, exceptions or source loss that determines its use. |
| common subjects and unlike views | Several readers can need different accounts of the same operation. |
| current information and collection cost | Fast refresh matters only where the decision or evidence can change quickly enough to use it. |
| comparable values and changed conditions | A new definition, work mix or measurement method can make old and new values incomparable. |
| sufficient decision evidence and unresolved detail | A bound can settle the choice even while some observations remain unknown. |

## OPS.15:4 - Solution {#solution}

### OPS.15:4.1 - Start from the receiving decision {#start-from-the-receiving-decision}

Name who needs to decide, what choice is open and when the answer can still change action. State the fact or comparison that would distinguish the choices. “Should we retain this service promise?” requires different evidence from “Which rig should receive the next ready package?”

Identify the operating subject and the result of concern. For each needed claim, recover its population: requests, test attempts, accepted packages, shifts, incidents or another explicitly defined set. Preserve the service boundary relevant to the recipient, including work that waits before entering the visible internal workflow.

Inspect existing accounts and observations before adding collection. Reuse one whose subject, conditions, time and definition fit. If a current qualified result already determines the next action, return it with its limit. Building a new dashboard is unnecessary for that choice.

### OPS.15:4.2 - Define the claims and measures {#define-the-claims-and-measures}

For each decision-bearing quantity, make its meaning recoverable. A ratio needs its numerator, denominator and eligibility rule. A duration needs its start, end, unit and treatment of unfinished cases. A count needs its event or result identity, observation window and duplication rule.

Choose the interpretation with the receiving use. Completed-only cycle time may describe completed work; it cannot by itself describe how all admitted work is progressing. A due-date cohort contains work whose required completion date falls within the selected period. Open work whose deadline has passed differs from open work whose deadline lies in the future.

Use the following questions only where their answers affect the claim:

| Question | Consequence for the account |
| --- | --- |
| What belongs to the population? | Inclusion, exclusion, cancellations, diverted work and service classes change the denominator or reach. |
| When is the event observed? | Clock origin, cutoff, timezone where material, and reporting delay change the time claim. |
| What constitutes completion or acceptance? | Attempts, completed work, accepted service and a later release can be counted differently. |
| How is the value obtained? | Source, measurement rule, sampling and missing data determine what the number supports. |
| Can the values be compared? | Changed definitions, methods, mix or conditions may require recalculation on a common basis. |

Keep uncertainty explicit when it can change the decision. Use an interval, separate unknown category or qualified estimate appropriate to the claim. A precise display does not remove missing observations.

### OPS.15:4.3 - Reconcile source events and subjects {#reconcile-source-events-and-subjects}

Trace the quantities to the events or observations that establish them. Recover which request, case, configuration, test, resource and result an event concerns. One event can concern several subjects, and one subject can have many events. Use their actual relationships when joining accounts. If the decision depends on which configuration or provider relation held at a particular time, obtain evidence for that interval; a relation record alone may not supply it.

For example, a second test attempt may add rig-hours while leaving the number of accepted test packages unchanged. Issuing an invoice for a package and receiving its payment are different events. A release can depend on several test results and a safety decision. Counting these records as interchangeable “completed items” loses the question the account must answer.

Inspect material gaps at the boundary of the measuring system. Server logs can omit failures that occurred before a request reached the server. A queue view can omit rejected, diverted or blocked requests. Obtain another source or narrow the claim where that loss matters.

Use OPS.15.1 when the account needs intervals or aggregates derived from those events. Its construction retains shared batch occupancy, repeated visits, cancellations and the portions of unfinished visits inside an observation window. Reuse a quantity already derived on the required population and boundary.

Reconcile disagreement before aggregating it away. Recover whether two totals use different cutoffs, populations or definitions. If the underlying observations permit it, recalculate on a common basis. Otherwise preserve the disagreement and state the narrower supported comparison or missing result.

### OPS.15:4.4 - Present the account for its actual readers {#present-the-account-for-its-actual-readers}

Lead with the claim supported for the decision, then show the observations and qualifications needed to assess it. Retain the source and time basis in the existing account at the detail the use requires. Distinguish observed state, an interpretation, a forecast and the decision made from them.

Several views can be useful. A coordinator needs current readiness and service risk; a finance practitioner needs accepted service, payable amounts and receipts; a release practitioner needs evidence applicable to a particular configuration. Keep the correspondence between their subjects explicit where the decision crosses views.

A shared table is appropriate when it preserves these meanings. Separate views are appropriate when they answer different questions. The account's form follows its use; an attractive common display cannot make unlike quantities interchangeable.

### OPS.15:4.5 - Stop collection at the decision-relevant boundary and refresh on change {#stop-collection-at-the-decision-relevant-boundary-and-refresh}

Ask whether unresolved detail can still change the decision. If even the favorable bound misses the criterion, the uncertainty need not be resolved for that conclusion. Other work may still need the detail for recovery, fairness, required assurance or a different decision; keep those uses separate.

Choose refresh timing from the decision window, rate of relevant change, observation delay and cost of stale information. A live incident can require rapid updates. A stable resource decision may need an update only when demand, configuration, access or another relied-on condition changes.

Remove recurring collection that has no current decision, assurance or recovery use, applying A.11.OP. Before stopping it, identify any real consumer that would lose a necessary result. Reuse a current observation only for the conditions and claims it still supports.

Return the account with the supported claim, remaining action-changing uncertainty and next useful observation. Use the appropriate operating method to decide admission, commitment, financial choice or control action from it.

## OPS.15:7 - Conformance Checklist {#conformance-checklist}

| Check | Evidence sufficient for the declared use |
| --- | --- |
| The account serves a live decision. | The choice, recipient, time for action and distinguishing observation are clear. |
| Subjects and populations are stable. | The relevant work, events, results, inclusions and exclusions can be recovered. |
| Quantities have a meaning. | Units, numerator/denominator where needed, start/end rules, cutoff and interpretation are explicit. |
| Sources support the claim. | Observation method, missingness, delay and comparability fit the receiving use. |
| Views can be related without conflation. | Shared subjects and unlike event meanings are preserved where decisions cross views. |
| Collection and refresh have a purpose. | Each retained observation serves the decision, necessary assurance or recovery, with a relevant change or expiry condition. |

## OPS.15:9 - Consequences {#consequences}

The reader can recover what a reported value says about the operating decision. Different practitioners can use unlike views of the same work while retaining the connections needed for a service, resource or release choice.

Some apparent disagreements remain after their meanings are clarified because the evidence is incomplete or incomparable. The account exposes that limit. A smaller set of relevant observations can reduce recurring effort, although repairing a lost event population may require work on the source system.

## OPS.15:12 - Relations {#relations}

OPS.4 guides shared operating attention using qualified state claims; this pattern helps construct the account when those claims are not yet supported. OPS.3 helps identify the operating subjects that source events concern.

OPS.5–OPS.10 provide admission, continuation, aging, queue, constraint and capacity questions that can select the account's observations. OPS.12–OPS.14 provide human-condition, commitment and financial uses. OPS.18 guides the control action based on quality and reliability evidence, while OPS.17 helps reconsider a failed method assumption.

FPF C.16 governs the measurement characteristics, units and comparison basis used here. A.10 keeps evidence reach explicit, and E.13 helps examine a proxy when its relationship to the intended value is in question. A.11.OP limits recurring account work to its actual contribution.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-3#root; conditional spec://ai.lev/fpf-eng-ops/contract/OPS-4#root, spec://ai.lev/fpf-eng-ops/contract/OPS-12#root–spec://ai.lev/fpf-eng-ops/contract/OPS-14#root, spec://ai.lev/fpf-eng-ops/contract/OPS-18#root; FPF spec://ai.lev/fpf-spec/contract/C-16#root, spec://ai.lev/fpf-spec/contract/A-10#root, spec://ai.lev/fpf-spec/contract/E-13#root, spec://ai.lev/fpf-spec/contract/A-11-OP#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-adm/contract/ADM-10#root, spec://ai.lev/fpf-eng-ma/contract/MA-1#root, spec://ai.lev/fpf-eng-ma/contract/MA-4#root, spec://ai.lev/fpf-eng-ops/contract/OPS-12#root, spec://ai.lev/fpf-eng-ops/contract/OPS-13#root, spec://ai.lev/fpf-eng-ops/contract/OPS-14#root, spec://ai.lev/fpf-eng-ops/contract/OPS-15-1#root, spec://ai.lev/fpf-eng-ops/contract/OPS-16#root, spec://ai.lev/fpf-eng-ops/contract/OPS-17#root, spec://ai.lev/fpf-eng-ops/contract/OPS-18#root, spec://ai.lev/fpf-eng-ops/contract/OPS-19#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-15
