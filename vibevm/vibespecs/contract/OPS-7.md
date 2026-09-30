# OPS.7 - Manage Aging, Urgency, and Service Commitments {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.7:0 - Use This When {#use-this-when}

Use this pattern when age, time remaining, a promised horizon, dependency change, new risk or consequence evidence, a progressed case state, or an unmet condition can change current priority or an existing bounded operating commitment. Typical cues are “this is old, so put it first”, “the deadline means we must release”, “the queue score escalated it”, “the patient has waited longest”, or “the issue is urgent” without a named consequence, authority, commitment, or decision horizon.

The first useful result is one bounded priority-and-commitment disposition:

> For exact subject or case `S` in qualified state `Q`, temporal claim `T`, existing commitment `C` with parties, conditions, horizon, and commitment authority `A_C`, and decision-bearing dependency, risk, consequence, recovery, and evidence `E`, current priority is `P` for coordination use `U` under priority authority `A_P`; commitment disposition is `K` when it changes; immediate coordination action or truthful blocker is `N`; affected parties, effective horizon, evidence limits, and next review are explicit.

Name the Systems holding `A_P` and `A_C`; the same System may hold both. Record any missing required authority in blocker `N`.

Recognition is cheap: enter when a temporal or consequence fact can reverse a current priority or commitment decision. Assurance is stronger: state, age, rate, trend, urgency, priority, queue rank, clinical triage, legal or safety permission, and commitment authority remain separate claims.

Do not use OPS.7 to sort every queue by age, create a universal urgency scale, identify the current constraint, size capacity, design service levels, perform clinical triage, authorize release, or establish a credible whole-service commitment account. Return those results to `OPS.8`–`OPS.13`, `OPS.18`, or their specialist owners. Use `C.27` only when the claim concerns intervention-sensitive rate, rhythm, recovery, or regime change; ordinary state, age, rate, or trend readings do not require it.

## OPS.7:0.1 - Working Distinctions {#working-distinctions}

| Name used here | Meaning |
| --- | --- |
| exact subject or case | The incident, patient case, user issue, release candidate, service relation, request, or other subject whose temporal and consequence claims matter. It is not automatically the queue item or record. |
| state claim | A qualified claim about the subject and relevant relations at a stated time or horizon. |
| age | Elapsed time since a defined event for an exact subject under a stated clock and conditions. Age is not urgency, priority, or rank. |
| time remaining | The interval between the current reference time and one relevant horizon under stated assumptions. A deadline alone creates no permission. |
| rate or trend | A relation concerning change per interval or a supported direction across observations. It is not an intervention effect by default. |
| intervention-sensitive temporal claim | A claim that an intervention changes a rate, rhythm, recovery, inertia, or regime. It requires the stronger discipline of `C.27`. |
| urgency | A decision-relative judgement that delay can change a named consequence, commitment, risk, recoverability, or supported use. It is not a durable kind or scalar by default. |
| priority | A current relation used for one coordination decision. It may inform but does not automatically equal queue position, admission order, clinical triage, economic value, authority, or service promise. |
| queue rank | A position under one queue policy and unit definition. It is not the universal expression of priority and can remain outside this pattern. |
| bounded commitment | An existing promise or obligation with parties, result or service, conditions, horizon, authority, and current status. |
| commitment disposition | Preserve, clarify, renegotiate, or withdraw an existing bounded commitment under the applicable authority and conditions. |
| whole-service commitment account | A wider account relating demand, resources, capability, uncertainty, service outcomes, and credible promises. It remains with `OPS.13`, not OPS.7. |
| priority-and-commitment result | The current priority disposition and reason, changed commitment disposition where authorized, immediate coordination action or blocker, parties, horizon, evidence, and next review. |

## OPS.7:1 - Problem Frame {#problem-frame}

Time matters in operations because delay can alter consequences, commitments, dependencies, recoverability, and the usefulness of later action. Yet the same elapsed time can mean different things for an incident, patient, release candidate, provider change, user issue, maintenance condition, or administrative request.

The practical problem is to make the temporal claim decision-bearing without converting it into automatic urgency, rank, or authority. The operation needs a current disposition that can preserve or revise priority and, where authority exists, maintain or change one bounded existing commitment.

## OPS.7:2 - Problem {#problem}

Age dashboards and escalation scores compress distinct claims. The oldest item appears most urgent; urgency appears to dictate queue position; a missed horizon appears to authorize release, treatment, staffing, or spending; and one local reprioritization appears to settle a system-wide service promise.

The opposite failure treats time as display-only. Practitioners notice age or deterioration but do not connect it to consequence, recovery burden, dependency, affected parties, existing commitment, authority, or next review. Avoidable delay then becomes visible only after a promise or protected condition has failed.

## OPS.7:3 - Forces {#forces}

| Force | Tension |
| --- | --- |
| simple age signal versus decision relevance | Age is cheap to compute, while consequence and commitment meaning depends on subject, conditions, and horizon. |
| fast escalation versus authority | Delay can demand attention, but priority and commitment changes require their respective authorized Systems. |
| local coordination versus system policy | One priority disposition can change immediate Work without designing queue order, capacity, constraint, or whole-service promises. |
| current evidence versus forecast | Deterioration, delay cost, and recovery burden may be uncertain; unsupported projections should not become urgency facts. |
| fairness versus unlike consequences | A common waiting rule can be legible, while clinical, safety, service, economic, and recovery consequences remain unlike and separately governed. |
| preserving promises versus truthful renegotiation | Keeping a commitment can matter, but hiding infeasibility harms affected parties and later recovery. |
| measurement versus intervention claim | State, age, rate, and trend can be observed directly; claimed intervention effects require stronger temporal and causal discipline. |

## OPS.7:4 - Solution {#solution}

### OPS.7:4.1 - Recover the exact subject, state, and existing commitment {#recover-the-exact-subject-state-and-existing-commitment}

Name the exact subject or case, its current qualified state, configuration and horizon, and the existing bounded commitment. Record the commitment's parties, promised result or service, conditions, horizon, authority, current status, and evidence limits. If no such commitment exists, do not create one by calling a target, service label, or desired date a promise.

Treat a matching `OPS.6` progressed state or unmet condition as evidence input only where it remains current for this decision. It neither authorizes nor entails priority or commitment revision.

### OPS.7:4.2 - Qualify the temporal claim before interpreting it {#qualify-the-temporal-claim-before-interpreting-it}

State the defining event, clock, observation time, horizon, and conditions. Decide whether the claim is current state, age, time remaining, rate, trend, or an intervention-sensitive temporal claim. Keep ordinary readings ordinary. Use `C.27` only when an intervention is claimed to change rate, rhythm, recovery, inertia, or regime; keep the `C.27.TA` time-window, cadence, and currentness discipline for all temporal uses.

### OPS.7:4.3 - Relate time to the decision-bearing consequences {#relate-time-to-the-decision-bearing-consequences}

Recover only what can change this decision: promised service, dependency state, risk, consequence of further delay, reversibility, recovery burden, affected parties, evidence and uncertainty, current comparison basis, and any feasible probe that could still reverse the result. Name clinical, safety, legal, security, financial, or other specialist claims without replacing their owners.

Age alone does not prove urgency. Express urgency as “delay can change `X` for decision `Y` under evidence `Z`”, or leave it unsupported.

### OPS.7:4.4 - Separate priority authority from commitment authority {#separate-priority-authority-from-commitment-authority}

Name the System authorized to maintain or change priority for the selected coordination use. Separately name the System authorized to preserve, renegotiate, withdraw, or otherwise alter the existing commitment. A coordinator may have one authority but not the other. Rank, expertise, responsibility, impact, and visibility grant neither by themselves.

### OPS.7:4.5 - Decide the bounded dispositions {#decide-the-bounded-dispositions}

For priority, preserve, raise, or lower it only when current evidence is sufficient and the decision is authorized; state the reason and intended coordination use. If the decision cannot be made, name the unresolved priority question, its intended recipient, and the condition for resuming the decision.

For the commitment, preserve it when support and conditions remain adequate; otherwise trigger authorized clarification, renegotiation, or withdrawal. When escalation or specialist return is needed, send the unresolved priority or commitment question to the participant with the relevant authority and state the decision expected from that participant. Include each unresolved question in the immediate coordination action or truthful blocker recorded in `OPS.7:4.6`.

Use `C.11` only where several real admissible dispositions need comparison. A bounded probe is suitable only when it can change the disposition before the relevant horizon.

### OPS.7:4.6 - State immediate action, parties, horizon, and review {#state-immediate-action-parties-horizon-and-review}

Record the current priority disposition, commitment disposition when one changes, immediate coordination action or truthful blocker, affected parties, effective horizon, supporting evidence and uncertainty, and next review or reopen trigger. Notify or coordinate with affected parties through the established relation; this pattern does not invent notification authority or prove receipt.

### OPS.7:4.7 - Return wider policy and specialist questions {#return-wider-policy-and-specialist-questions}

Do not convert the local result into queue rank, buffer or constraint policy, capacity, clinical triage, legal permission, safety acceptance, financial value, release authority, service design, or a credible whole-service commitment account. Return those questions to `OPS.8`–`OPS.13`, `OPS.18`, or the competent specialist practice.

## OPS.7:7 - Conformance Checklist {#conformance-checklist}

- [ ] The exact subject or case, qualified state, configuration, and horizon are named.
- [ ] The existing commitment has parties, content, conditions, horizon, authority, status, and evidence limits.
- [ ] Any `OPS.6` result is used as evidence only at the matching configuration and horizon.
- [ ] State, age, time remaining, rate, trend, and intervention-sensitive temporal claims are distinguished.
- [ ] `C.27` is used only for an intervention-sensitive rate, rhythm, recovery, inertia, or regime claim.
- [ ] Urgency names the consequence, commitment, risk, recovery, or supported use that delay can change.
- [ ] Priority, queue rank, clinical triage, economic value, permission, and commitment remain distinct.
- [ ] Priority authority and commitment authority are separately established.
- [ ] The current comparison basis and any useful probe are explicit.
- [ ] Priority and commitment dispositions, immediate action or blocker, parties, horizon, evidence, and next review are recorded.
- [ ] The local result is not presented as queue, capacity, constraint, service-design, assurance, or whole-service commitment result.
- [ ] Specialist questions return to their direct owners.

## OPS.7:9 - Consequences {#consequences}

The operation gains a disciplined way to act before avoidable delay becomes failure while resisting automatic escalation. Practitioners can explain why priority changed, whether a bounded commitment changed, who held each authority, which parties are affected, and when the result must be reviewed.

The cost is that age, urgency, rank, and promise can no longer be carried by one convenient score. Some cases return to queue, capacity, clinical, safety, legal, finance, release, or whole-service owners. The pattern establishes no optimal ordering, patient outcome, released change, fulfilled commitment, or operational effectiveness.

## OPS.7:12 - Relations {#relations}

- `OPS.6` supplies a progressed state or unmet condition only as evidence where it changes this decision at the same configuration and horizon. It does not authorize a priority or commitment revision.
- `C.27.TA` governs temporal aspect, window, cadence, and currentness. `C.27` governs intervention-sensitive rate, rhythm, recovery, inertia, or regime claims; neither supplies Operations priority or authority.
- `C.11` governs comparison only when several admissible live dispositions require choice. `A.10` governs evidence reliance.
- `OPS.5` retains admission and explicit-start conditions. A current priority relation neither admits demand nor establishes start permission or Work.
- `OPS.8`–`OPS.11` retain queue, buffer, constraint, capacity, variability, and interacting-structure decisions. `OPS.13` retains the credible whole-service commitment account. `OPS.18` retains operating quality and reliability questions.
- Clinical triage, consent, medical safety, law, privacy, security, finance, product assurance, release, provider authority, and other specialist results remain with their direct owners.
- Pattern order is not a lifecycle. Practitioners may enter OPS.7 directly when its current evidence and authority exist, repeat it as conditions change, or return without using OPS.5 or OPS.6 in the same episode.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-6#root evidence; FPF spec://ai.lev/fpf-spec/contract/C-27-TA#root; conditional spec://ai.lev/fpf-spec/contract/C-27#root, spec://ai.lev/fpf-spec/contract/C-11#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-ops/contract/OPS-10-2#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-7
