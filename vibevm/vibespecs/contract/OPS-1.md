# OPS.1 - Identify the Operating System, Commitments, and Flow Units {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.1:0 - Use This When {#use-this-when}

Use this pattern when people want to improve a process, clear a backlog, raise utilization, accelerate flow, or redesign a board but cannot yet name the operation whose result must continue. Typical warning signs are an organization name used as the operating boundary, one ticket called the customer need, a queue column treated as the Work, or a service promise discussed without its parties, conditions, or horizon.

The first useful move is to write one bounded operating-focus statement:

> For this decision and horizon, `OperatingSystem-X` must continue supplying `Result-or-Service-Y`; current demand and commitments are `...`; the decision-bearing subjects and counted units are `...` under these identity rules; the unresolved boundary, authority, evidence, or control question is `...`.

That statement is useful before a workflow, target, priority, or policy is chosen. It gives `OPS.2` a real coordination question and gives `OPS.3` exact subjects to distinguish.

Recognition is cheap: enter when a practical decision cannot name its operating System, continuing result, commitments, or tracked unit. Assurance is claim-specific: System identity, commitment, Work, subject identity, authority, evidence, safety, value, and effectiveness use their own governing patterns and specialist Methods before reliance.

Do not use OPS.1 merely to rename an already bounded operation, classify every object as a System, approve a strategy, design a product, authorize Work, or choose an improvement Method. If the current blocker is a product or asset change, organization change, one person's capability, finance, law, safety, or another specialist result, obtain that result and return only if it changes the operating focus.

## OPS.1:0.1 - Working Distinctions {#working-distinctions}

| Name used here | Meaning |
| --- | --- |
| operating System | One actual System whose continuing operation and results are current for the decision. It is not inferred from an organization name, process diagram, product label, software tool, or reporting boundary. |
| continuing result or service | The result, service, or preserved condition the operation must keep supplying to a named receiver under stated conditions. Continuation does not prove value, quality, acceptance, or fulfilment. |
| demand | A request, need, condition, candidate Work claim, arrival, or other input entering the operating decision. Demand is not automatically admitted Work or a commitment. |
| commitment | A promise or obligation with parties, promised result or service, conditions, horizon, authority, and current status. A due date or priority label alone is not a commitment. |
| operating subject | The exact System, item, case subject, material, service relation, account, or other entity whose state or relation can change the operating decision. |
| flow or case unit | A decision-specific counted or tracked unit with an identity rule and receiving use. Treat Work items, cases, physical items, batches, transactions, commitments, and results as different units unless their identity rules and evidence establish that the labels denote the same counted or tracked unit for this use. |
| operating boundary | The included subjects, Work, resources, relations, environments, and time horizon needed for this decision, plus explicit exclusions and specialist returns. |
| control-relevant operating concern | A question in which observation, decision, actuation, supervision, feedback, or unlike rates can change current coordination. It is an entry cue for an FPF control view, not a kind of operation. |
| operating-focus result | The bounded result returned by OPS.1: operating System, continuing result, demand, commitments, subjects and units, boundary, evidence or authority gaps, next pattern, and reopen condition. |

## OPS.1:1 - Problem Frame {#problem-frame}

Operations work begins in the middle. Demand has arrived, commitments already exist, cases are open, resources are shared, records disagree, and service must continue while changes are considered. Familiar representations make that situation look simpler than it is. A board foregrounds Work items, an organization chart foregrounds positions, a process map foregrounds recurring order, and a product model foregrounds the engineered object.

Answering the operating question may require several of these representations. A useful starting boundary therefore comes from the continuing result and present decision, then identifies the actual operating System, commitments, subjects, and units needed to decide.

## OPS.1:2 - Problem {#problem}

Without an operating focus, later optimization can improve the representation while degrading the operation. A team can shorten one board column while customer cases age, increase resource utilization while service commitments fail, count ticket closures while the field condition persists, or optimize product-control performance while release and incident-response Work remain blocked.

The failure propagates. Queue, constraint, capacity, quality, service, finance, and Method-improvement decisions inherit the wrong boundary and unit.

## OPS.1:3 - Forces {#forces}

| Force | Tension |
| --- | --- |
| Urgency | A visible backlog invites immediate action, while an incorrect operating boundary makes the action locally efficient and globally harmful. |
| Familiar names | Company, team, product, service, platform, and process names help orientation, while none alone identifies the operating System. |
| Several commitments | Customer, safety, provider, release, support, and financial commitments can coexist without one being the universal priority. |
| Countability | Boards and logs offer convenient units, while convenience does not establish identity or receiving use. |
| Continuing service | The operation must act with incomplete evidence, while uncertainty does not license invented state or authority. |
| Bounded entry | The first result must be affordable, while later decisions need enough identity and boundary precision to avoid rework. |

## OPS.1:4 - Solution {#solution}

Limit the operating focus to what the current decision needs; identify the actual System, continuing result, relevant commitments, and subject/unit boundary. Begin from the result that must continue, not from a preferred board, workflow, metric, or school.

### OPS.1:4.1 - Pattern-Use Unfolding {#pattern-use-unfolding}

1. **Name the first user and decision.** State who needs the focus, what decision it enables, the relevant horizon, and the first useful result or honest blocker.
2. **List materially different operating-System candidates.** Consider the whole organization, a service operation, production cell, development operation, hospital function, supply relation, personal operation, product or asset, and coordination software when each is plausible. Use `A.1.SCR` only when System identity changes the decision; otherwise name the actual subject and leave through its pattern.
3. **State the continuing result or service.** Name its receiver, conditions, horizon, and the observation that would show interruption or degradation. Keep value, quality, acceptance, fulfilment, safety, and causal effect as separate claims.
4. **Recover demand and commitments.** Distinguish requests and candidate Work from admitted Work. For each decision-bearing commitment, name parties, promised result or service, conditions, horizon, authority, current status, and evidence gap.
5. **Name operating subjects.** Identify the customers, cases, physical items, release candidates, incidents, transactions, materials, services, accounts, or other subjects whose state or relation changes action.
6. **Define every tracked unit.** State the unit's identity rule, start and finish when it is a Work item, subject/result relation, counted interval, and receiving use. Do not call every unit a flow item merely because a board counts it.
7. **Draw the operating boundary.** Include only the Work, resources, relations, environments, and time horizon needed by the decision. Name excluded product, organization, asset, finance, legal, safety, capability, and other specialist questions with their return conditions.
8. **Check the control branch.** If observation, decision, actuation, supervision, feedback, or rate separation can change coordination, record the control-relevant operating concern for `OPS.2`. Do not construct a control view or infer a feedback relation here.
9. **Recover authority and evidence limits.** Name who may use the focus for which decision, what evidence supports it, what remains uncertain, and which missing fact blocks reliance.
10. **Return, dispose, and reopen.** State the selected operating focus, rejected candidates, next pattern, truthful stop, and one observable change that reopens the boundary, commitment, subject, or unit. When a change reopens any focus field, list the known downstream views, accounts, policies, and later decisions that consumed that field; mark each `recheck`, `still usable`, or `return`, and give the decision-local reason. Leave an unrelated consumer intact.

### OPS.1:4.2 - Record the Result {#record-the-result}

| Result position | Required content |
| --- | --- |
| use boundary | First user, decision, horizon, first useful result, and truthful stop. |
| operating-System candidates | Candidate referents, decisive identity and boundary facts, selected System or subject-pattern return, and rejected alternatives. |
| continuing result or service | Receiver, result or preserved condition, operating conditions, interruption observation, and unresolved value, quality, safety, or acceptance claims. |
| demand and commitments | Demand classes; commitment parties, contents, conditions, horizons, authority, status, and evidence gaps. |
| subjects and units | Exact subjects, unit identity rules, Work-item start/finish where relevant, subject/result relations, and receiving uses. |
| boundary and returns | Included Work, resources, relations, environments, horizon, exclusions, and specialist results needed. |
| control concern | The decision-changing observation, actuation, supervision, feedback, or rate question, or an explicit `not current` result. |
| continuation | Next useful pattern and an observable reopen condition. |
| downstream disposition | Every known view, account, policy, or later decision that consumed a changed focus field, marked `recheck`, `still usable`, or `return` with its reason; unrelated consumers remain intact. |

### OPS.1:4.3 - What Changes in Practice {#what-changes-in-practice}

The practitioner stops treating “the process”, backlog, service label, or reporting unit as self-evident. Every later view, queue, capacity measure, or intervention must refer to one operating System, a continuing result, explicit commitments, and units whose identity and use are known. A missing boundary or commitment becomes a useful blocker before a policy change accumulates cost.

## OPS.1:7 - Conformance Checklist {#conformance-checklist}

- [ ] The opening names a first user, operating decision, horizon, and useful stop.
- [ ] The operating System is selected from materially different candidates or the result truthfully returns to another subject pattern.
- [ ] The continuing result or service names its receiver and conditions without declaring value, quality, safety, acceptance, or fulfilment by wording.
- [ ] Demand, commitments, admitted Work, subjects, records, and units remain distinct.
- [ ] Every decision-bearing commitment names parties, content, conditions, horizon, authority, status, and evidence limits.
- [ ] Every counted or tracked unit has an identity rule and receiving use.
- [ ] The boundary names included Work and relations, exclusions, specialist returns, and evidence or authority gaps.
- [ ] A control concern is recorded only when it can change the decision; no diagram or controller label establishes it.
- [ ] The next pattern and one observable reopen condition are explicit.
- [ ] A reopened focus gives every known consumer of the changed field a `recheck`, `still usable`, or `return` disposition and leaves unrelated consumers intact.

## OPS.1:9 - Consequences {#consequences}

The pattern prevents premature optimization and gives later patterns stable subjects, commitments, units, and return conditions. It also exposes when the useful next result belongs to product engineering, organization change, maintenance, finance, safety, law, capability development, or another specialist practice.

The cost is early boundary and identity work. Some urgent requests stop because no one can support the operating System, commitment, unit, authority, or evidence claim. That is cheaper than optimizing a proxy whose relation to the continuing result is unknown.

## OPS.1:12 - Relations {#relations}

- `A.1.SCR` governs conditional System recognition; OPS.1 consumes that result and adds the operating continuation, commitment, subject, and unit boundary.
- `A.6.REL` and direct subject patterns govern obtaining relations. `C.2.1` governs persisted claim-bearing accounts; a focus statement creates neither relation nor world state.
- `OPS.2` consumes the operating System, commitments, subjects, units, decision questions, and any control-relevant concern. `OPS.3` consumes subject candidates, commitments, evidence questions, and identity gaps.
- `OPS.5` later consumes the eligible demand and current commitments for admission; `OPS.15`, `OPS.17`, and `OPS.19` later consume the operating scope for account, repertoire, and simultaneous-Work decisions.
- Product engineering, OCE, Maintenance, HCD, finance, governance, administration, safety, law, medicine, and other specialists retain their subjects, Methods, evidence, and authority.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): FPF spec://ai.lev/fpf-spec/contract/A-1-SCR#root, spec://ai.lev/fpf-spec/contract/A-6-REL#root, spec://ai.lev/fpf-spec/contract/C-2-1#root, spec://ai.lev/fpf-spec/contract/A-10#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-eam/contract/EAM-2#root, spec://ai.lev/fpf-eng-eam/contract/EAM-4#root, spec://ai.lev/fpf-eng-ops/contract/OPS-19#root, spec://ai.lev/fpf-eng-ops/contract/OPS-2#root, spec://ai.lev/fpf-eng-ops/contract/OPS-3#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-1
