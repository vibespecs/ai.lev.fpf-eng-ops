# OPS.9 - Diagnose and Treat the Current Operating Constraint {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.9:0 - Use This When {#use-this-when}

Use this Method when an operation is not producing its accepted result as required and someone proposes to remove a bottleneck, increase capacity, automate a step or accelerate a team. The question is which relation currently limits completion, and what treatment the evidence supports.

The first useful result is a bounded constraint account: the lost result and observation window, relevant observations, a candidate explanation and a serious rival, discriminating support or an exact probe request, and a treatment or hold decision. It can conclude that the proposed resource addition is unsupported while specifying a useful readiness or measurement action.

Use OPS.8 when a queue policy can be repaired without settling a wider constraint claim. Use OPS.10 when the immediate question is a load/capacity/service comparison with an already adequate causal basis. A safety, clinical, engineering or financial diagnosis remains with the qualified practice that supplies it.

## OPS.9:1 - Problem frame {#problem-frame}

A queue can be long because service capacity is scarce, inputs arrive in bursts, prerequisites are incomplete, acceptance is delayed, or earlier defects return as rework. Several of these mechanisms can obtain together. A resource may be idle for much of a week and still constrain a short critical window.

Here a current constraint is a supported limiting relation for one operating result under a stated arrangement and horizon. It can concern usable capacity, readiness, sequence, quality, access, a decision or another condition. It is not a permanent label attached to the busiest person or machine.

## OPS.9:2 - Problem {#problem}

Local speed and utilization are easy to observe. The causal relation to accepted operating results is harder. An improvement can halve touch time while leaving completion unchanged because work still waits for acceptance, a complementary input or another resource.

The opposite error demands a complete causal model before making any useful decision. A small feasibility bound, a discriminating observation or a reversible probe can sometimes rule out a proposed treatment at much lower effort.

## OPS.9:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| urgent treatment and adequate diagnosis | Delay can be costly, but the wrong treatment consumes resources and can move congestion elsewhere. |
| one focal constraint and distributed delay | Focusing effort helps, while several short waits or alternating regimes can defeat one-resource explanations. |
| local measures and accepted results | Touch time, busy time and queue length can change without changing what the operation delivers. |
| useful probes and protected conditions | A probe can discriminate explanations only while preserving the relevant professional, acceptance and comparison conditions. |
| learning and migration | A useful treatment changes the arrangement; its success can make the former constraint cease to be current. |

## OPS.9:4 - Solution {#solution}

### OPS.9:4.1 - Fix the result and the shortfall {#fix-the-result-and-the-shortfall}

Name the operating result, its accepted unit, demand or commitment being compared, relevant subjects, horizon and acceptance criteria. Reuse current OPS.1–OPS.4 inputs where they fit. Distinguish accepted demand, service attempts and accepted results; a failed test or reopened case can consume capacity without adding a result.

State the shortfall in terms that can change a decision: fewer accepted results, unacceptable time to result, missed qualified service conditions, or another explicit operating consequence. Preserve the result definition and case mix in later comparisons. A changed definition reopens the account rather than silently improving the metric.

### OPS.9:4.2 - Reconstruct where completion is lost {#reconstruct-where-completion-is-lost}

Follow representative matters through the relevant services and joins. Recover entry, eligibility, start, completion, return and acceptance events. Distinguish processing, setup, starvation, blocking, unavailability and rework only where they can explain the shortfall.

Use the event sequence and the resource calendar together. A snapshot identifies a population at one time; it does not explain a week of waiting. A utilization average can hide a critical peak. Record uncertainty and missing events before calculating a causal-looking rate.

If the result is delayed by many small waits, inspect cadence, handoff and decision timing across the path rather than forcing one scarce-resource answer.

### OPS.9:4.3 - State a mechanism and a rival {#state-a-mechanism-and-a-rival}

Express the candidate explanation as a relation: “Under this demand and access pattern, the final test cannot process the required eligible load before the horizon,” or “Late prerequisite delivery leaves the booked rig without eligible packages.”

Name an alternative that could produce the same observation and change treatment. Examples are insufficient usable rig time versus incomplete kits; scarce acceptance effort versus evidence repeatedly missing at acceptance; or slow processing versus arrivals concentrated near the deadline.

Give each explanation an expected observation and a possible defeater. If both predict the same data, the present observation cannot choose between them. Do not rename a queue “the constraint” to close that gap.

### OPS.9:4.4 - Obtain the least burdensome discriminating basis {#obtain-the-least-burdensome-discriminating-basis}

Select the basis appropriate to the claim and decision:

- A resource/precedence bound can establish infeasibility under explicit demand, capability, calendar and acceptance assumptions. Show a feasible schedule as well when claiming that a proposed treatment makes the result achievable.
- Event-history replay can reveal starvation, blocking, rework and timing relations. Its observational explanation remains limited by event quality and unobserved conditions.
- A bounded field probe changes one consequential mechanism under the applicable professional Method and permission. State the comparison cases or windows, preserved conditions, interference, expected observations and stopping rule.
- A specialist causal or scheduling analysis is warranted when uncertainty, confounding or coupled behavior can reverse a consequential decision and the simpler basis cannot resolve it.

For a probe, keep the same accepted-result criteria and record demand, mix, resource availability and consequential conditions. Shared queues or common providers can affect nominal comparison cases too. Use an appropriate time-blocked, matched or other justified comparison; a convenient before/after label does not remove interference or confounding.

Current FPF C.16 governs the measurement chain and C.28 governs what causal use the basis supports. The operation still has to supply the actual measurement or probe, the professional premises and its observations.

### OPS.9:4.5 - Compare treatments from the current arrangement {#compare-treatments-from-the-current-arrangement}

Compare the incumbent with a finite change that acts on the supported mechanism. Candidate treatments include protecting usable constraint time, changing release or dispatch, completing prerequisites earlier, reducing avoidable setup or rework, obtaining capacity, or changing a domain Method.

Account for implementation effort, transition loss, displaced work, downstream congestion, affected commitments and reversibility. Use C.11.CRC for the finite comparison and C.11 for the choice when several admissible alternatives remain. Resource acquisition is not preferred merely because it is easy to count.

A treatment is supported only to the scope of the evidence. A deterministic scenario can show feasibility; it does not establish actual field effectiveness. A probe can support a bounded effect without showing that the same treatment remains useful under another demand regime.

### OPS.9:4.6 - Return the decision and remeasure {#return-the-decision-and-remeasure}

Return the result definition and window, observations, supported explanation or unresolved rival, basis and limits, selected treatment or probe/hold decision, authority, affected decisions and the next observation that can change the conclusion.

After a treatment, inspect the accepted result and the actual load, waiting, quality and resource consequences. Reopen when demand, mix, eligibility, access, acceptance, recovery or a coupled structure changes. Do not keep “improving the bottleneck” after the relation that justified the label has disappeared.

## OPS.9:7 - Conformance Checklist {#conformance-checklist}

1. Is the accepted result and shortfall fixed for the relevant population and horizon?
2. Do observations distinguish the mechanisms that could change treatment?
3. Is there a serious rival with a discriminatory observation or defeater?
4. Does the selected bound, replay, probe or specialist analysis support the claim actually made?
5. Does the treatment act on that mechanism and include consequential interactions and transition costs?
6. Can participants act on the treatment, hold or exact probe request and recognize when it must reopen?

These questions recognize an inspectable diagnosis and decision. Assurance depends on the actual observation quality, comparison validity, professional premises and authority; a complete account is not itself causal evidence.

## OPS.9:9 - Consequences {#consequences}

Effort can be directed to a mechanism that affects accepted results. An exact “not yet justified” treatment decision can prevent waste while leaving a cheap useful policy or probe available.

The cost is some additional measurement and comparison discipline. The appropriate depth depends on the consequence of error: a reversible readiness trial and a major capacity acquisition need not carry the same evidence burden.

## OPS.9:12 - Relations {#relations}

OPS.1–OPS.4 supply matching operating focus, subject identities and current observations. OPS.8 supplies relevant queue, readiness and buffer policy; OPS.10 supplies usable-capacity and service comparisons; OPS.11 exposes couplings that can sustain or move a limiting relation.

OPS.5–OPS.7 consume supported operating-policy consequences under their own admission, continuation, priority and commitment authority. A domain Method change returns to its owner. OPS.16 is available for the separate local operating-Method-improvement question but is not a prerequisite for diagnosing the current constraint.

Current FPF C.16, C.27.TA/C.27, C.28, C.11.CRC and C.11 govern measurement, temporal and causal claims, finite contribution and choice. They do not supply a clinical, engineering, safety, labor or financial diagnosis merely by being cited.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-3#root, spec://ai.lev/fpf-eng-ops/contract/OPS-4#root; conditional spec://ai.lev/fpf-eng-ops/contract/OPS-8#root, spec://ai.lev/fpf-eng-ops/contract/OPS-10#root, spec://ai.lev/fpf-eng-ops/contract/OPS-11#root; FPF spec://ai.lev/fpf-spec/contract/C-16#root, spec://ai.lev/fpf-spec/contract/C-28#root, spec://ai.lev/fpf-spec/contract/C-11-CRC#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-ops/contract/OPS-10#root, spec://ai.lev/fpf-eng-ops/contract/OPS-8#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-9
