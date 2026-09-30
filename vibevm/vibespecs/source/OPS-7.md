# OPS.7 - Manage Aging, Urgency, and Service Commitments: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.7:5 - Archetypal Grounding — Three Aging and Commitment Replays {#archetypal-grounding-three-aging-and-commitment-replays}

### OPS.7:5.1 - PumpWorks incident and release horizon {#pumpworks-incident-and-release-horizon}

`FieldIncident-I73` has an exact age and current incident state; PumpWorks also has a weekly evidenced-release horizon, dependencies on test `T9`, rig access and a safety return, service consequences, reversibility, recovery burden, and distinct release and safety authorities. OPS.7 relates those facts to the existing commitments and to the coordination decision.

The result may raise the incident's current priority and trigger authorized clarification or renegotiation of the weekly release commitment, while naming the immediate diagnostic, access, or stakeholder coordination action. Incident age alone does not dictate rig queue rank. The weekly horizon does not create release permission. The local revision establishes no rig policy, current constraint, capacity, safety acceptance, release, or credible service-wide commitment account.

### OPS.7:5.2 - Public-hospital waiting and deterioration {#public-hospital-waiting-and-deterioration}

One clinical case has a defined waiting age, current observations, possible deterioration evidence, dependencies on clinicians, beds and other resources, a service horizon, affected patient and care participants, and explicit clinical and operating authorities. OPS.7 makes those relations available to the authorized priority and commitment decision.

It does not equate waiting age with clinical urgency or triage. A qualified clinical System retains medical judgement and treatment authority. The Operations result may preserve or change the current coordination priority and prompt an authorized service-commitment return, but queue redesign, staffing and capacity, consent, privacy, medical safety, statutory permission, treatment efficacy, and patient outcome remain with their direct owners.

### OPS.7:5.3 - AI-assisted software issue and service promise {#ai-assisted-software-issue-and-service-promise}

One user issue has an exact age and state, user and service consequence, dependency on tool or model access, current trace and test evidence, integration load, recovery burden, bounded concurrency, and a promised horizon. OPS.7 relates those facts without treating model score, episode count, or dashboard severity as automatic urgency.

The authorized System may revise the issue's coordination priority or trigger an authorized commitment renegotiation, with an immediate check, integration action, fallback, or stop and next review. The result does not establish software assurance, security, model capability, provider authority, agenthood, causal effectiveness, integration, release permission, or service fulfilment.

## OPS.7:6 - Bias-Annotation {#bias-annotation}

| Bias or pressure | How it distorts temporal decisions | Countermeasure |
| --- | --- | --- |
| age-equals-urgency bias | Elapsed time substitutes for consequence and decision context. | Relate delay to one named risk, commitment, dependency, recovery, or supported use. |
| score reification | A severity or priority number appears to be an objective property. | Recover the comparison basis, intended coordination use, evidence, and authority. |
| deadline authority | A date is treated as permission to release, treat, spend, or bypass a condition. | Keep commitment horizon, priority, and specialist permission separate. |
| queue-rank collapse | Current priority becomes one universal queue position. | Bound the disposition and return queue policy to its owner. |
| commitment-preservation bias | An earlier promise is preserved despite unsupported conditions. | Revalidate parties, content, conditions, horizon, authority, and feasibility evidence. |
| local-to-system overreach | One reprioritization is reported as a service-wide promise or capacity result. | State the local result and return to `OPS.13` or the wider owner. |
| intervention-story bias | A change in rate or recovery is attributed to the chosen action without adequate temporal support. | Apply `C.27` only to the intervention-sensitive claim and preserve evidence limits. |

## OPS.7:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Failure | Repair |
| --- | --- | --- |
| oldest first by nature | Age becomes a universal priority rule. | State the subject, consequence, commitment, comparison basis, and policy owner. |
| urgency score as fact | A representation hides assumptions, evidence, and receiving use. | Reconstruct the decision-relative claim and uncertainty. |
| deadline grants permission | Commitment pressure bypasses clinical, safety, legal, security, or release authority. | Keep horizon, priority, and permission as separate results. |
| local escalation becomes queue policy | One disposition silently reorders every item. | Bound the coordination result and return the queue decision. |
| promise by label | A service target or desired date is treated as an obtaining commitment. | Recover parties, content, conditions, authority, and status. |
| record change becomes stakeholder agreement | A revised field is treated as renegotiation or receipt. | Use the established commitment and communication relations and preserve evidence of acceptance. |
| temporal overanalysis | Ordinary age or rate triggers unnecessary dynamics modelling. | Keep ordinary temporal claims ordinary; use `C.27` only when the intervention-sensitive claim is current. |

## OPS.7:10 - Rationale {#rationale}

Temporal facts become useful only through a receiving decision. Age is broadly observable, but urgency depends on what delay changes; priority depends on one coordination use; and commitment alteration depends on parties, conditions, and authority. Keeping these relations separate prevents time pressure from becoming unearned permission.

The pattern is intentionally local. It can preserve or revise one current priority and one existing bounded commitment without waiting for a complete queue, capacity, or service-design account. Explicit returns keep queue, buffer, constraint, capacity, service-design, whole-service commitment, and specialist questions with their governing patterns or competent participants.

## OPS.7:11 - SoTA-Echoing {#sota-echoing}

| Practice question | Selected current line and serious alternative | Defect overcome and governed loci | Source roles and limits | Reopen condition |
| --- | --- | --- | --- | --- |
| How should age and changing consequence inform current priority or an existing commitment without becoming automatic rank or authority? | The selected line is a **decision-relative temporal and commitment account with separate state, age, urgency, priority, authority, bounded commitment, immediate action, and review**. The serious default is an **age, deadline, or priority score used as universal queue rank and escalation authority**. | The default hides subject identity, unlike consequences, permission, and the local-versus-system boundary. **Adapt:** `OPS.7:4.1`–`OPS.7:4.7` qualify the temporal claim, relate it to consequences and commitments, separate authorities, decide bounded dispositions, and return wider policy. **Reject:** age as urgency, urgency as rank, or local revision as whole-service commitment. | Current FPF `C.27.TA` supplies temporal aspect, window, cadence, and currentness discipline; `C.27` governs intervention-sensitive rate, rhythm, recovery, and regime claims. The Kanban Guide supplies bounded Work-item age and flow measures. Reinertsen supplies delay and economic trade-off mechanisms. DEMO supplies bounded commitment and responsibility distinctions. None sets operating priority, queue rank, clinical triage, specialist permission, or whole-service commitment authority. | Reopen if a stronger current disposition preserves subject, temporal, consequence, authority, commitment, local/wider, and specialist-return boundaries with less burden, or if a source changes an action-bearing temporal or commitment relation. |

The selected comparison is supported by these bounded source roles.

| Source line | Retained contribution | Use boundary |
| --- | --- | --- |
| Current FPF [`C.27.TA`](spec://ai.lev/fpf-spec/contract/C-27-TA#root) | Temporal subject, event, interval, horizon, window, cadence, and currentness discipline. | Supplies no Operations priority, queue rank, commitment, authority, or intervention. |
| Current FPF [`C.27`](spec://ai.lev/fpf-spec/contract/C-27#root) | Discipline for intervention-sensitive effort, inertia, rate, rhythm, recovery, and regime claims. | Ordinary age and rate readings need not invoke it; it supplies no operating decision or causal result by itself. |
| [The Kanban Guide 2025.5](https://kanbanguides.org/the-kanban-guide/2025.5/) | Bounded Work-item age, cycle time, throughput, WIP, active-item management, and explicit policy. | Supplies no universal priority rule, queue rank, service guarantee, or specialist authority. |
| Reinertsen, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Delay, queue, variability, feedback, batch, and economic trade-off mechanisms. | Supplies no universal cost-of-delay value, fixed score, permanent optimum, or local authority. |
| DEMO, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Bounded commitment, responsibility, production, and coordination distinctions. | Source-local transaction constructs do not assign authority, prove acceptance, or establish a service-wide commitment elsewhere. |


## OPS.7:End {#end}
