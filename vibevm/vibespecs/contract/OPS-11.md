# OPS.11 - Coordinate Interacting Operating Structures {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.11:0 - Use This When {#use-this-when}

Use this Method when a local operating change depends on, or changes, another arrangement: material processing and order transactions, test work and release evidence, resource access and service commitments, or observation and supervisory decisions. Typical symptoms are a feasible local plan that cannot be completed in practice, a faster resource followed by more waiting elsewhere, or incompatible decisions by people responsible for different parts of the operation.

The first useful result is a bounded coordination decision: the affected structures and concrete couplings, feasible alternatives and consequences, decisions required from their respective owners, unresolved relations, and a return condition. Start from one operating question or proposed change, not from a map of the whole enterprise.

Use OPS.8 for a queue-policy question that does not require wider coordination, OPS.9 for an unresolved constraint diagnosis, and OPS.10 for a capacity/service calculation. Product or organization redesign belongs to the corresponding engineering practice when that is the object being changed.

## OPS.11:1 - Problem frame {#problem-frame}

An operation depends on several actual structures. Its resource participation, material transformation, case and commitment relations, information production/use, financial settlement and decisions may be described in different views. Those structures overlap through particular subjects and relations; the views need not be isomorphic.

Here the Method governs coordination of an operating change across the selected structures. It does not make their diagrams into the structures, reduce them to one “flow,” or give one coordinator authority over every participating decision.

## OPS.11:2 - Problem {#problem}

A local plan can omit a necessary coupling. Product is made but goods cannot be issued without documents. Tests complete but the evidence does not apply to the release configuration. Capacity exists but access is not granted in the required window. A resource-saving change transfers cost, risk or burden to another participant.

The opposite error builds an elaborate network description without changing any decision. The operation needs the smallest set of actual couplings that can reverse the proposed action, together with a usable coordination result.

## OPS.11:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| local clarity and cross-structure effects | A narrow view makes one decision easy while hiding a prerequisite or consequence elsewhere. |
| end-to-end coordination and independent authority | The result depends on several decisions, but their authority does not merge. |
| unlike quantities and comparison | Material, time, money, risk and human burden can all matter without having one valid scalar measure. |
| model detail and useful action | More represented relations can increase effort without improving the current choice. |
| stable agreements and changing conditions | A coordinated plan can become infeasible after access, evidence, demand or commitment changes. |

## OPS.11:4 - Solution {#solution}

### OPS.11:4.1 - Start from the proposed operating change {#start-from-the-proposed-operating-change}

Name the operating result, current arrangement, proposed change and horizon. State which consequence would make the change useful or unacceptable. Reuse the current OPS.1–OPS.4 account and a matching OPS.8–OPS.10 result where available.

Select the affected Systems and participants by the actual consequences, not by the organizational chart alone. A supplier, customer, operator or neighboring service can matter without appearing inside the local department boundary.

If one direct pattern already settles the decision and no cross-structure relation can change it, use that result and stop.

### OPS.11:4.2 - Identify the structures needed for this question {#identify-the-structures-needed-for-this-question}

For each selected structure, recover the actual constituents, obtaining relations, applied constraints and use. Say what the current view shows and which material features it omits.

Use A.22 for the general structural question. Use E.18 for one transformation-flow structure and E.18.2 for a mathematical description when that lens is useful. Select an E.18.NET network only when at least two transformation-flow structures are independently identified and obtaining cross-flow relations connect their positions under the applicable constraints and use frame.

A branching process, several views of one flow, and several independently identified flows are different cases. Financial or decision relations need not be reclassified as a transformation flow to be relevant. If a required relation or identity cannot be recovered, retain the proposed description and name the missing basis.

### OPS.11:4.3 - Recover each decision-changing coupling {#recover-each-decision-changing-coupling}

For each coupling, state what depends on what, through which relation, under what condition and timing. Keep subject correspondence separate from production, supply, permission, evidence support, commitment or causal influence.

A useful working statement is: “This shipment can use this product only after these required documents are available”; “this test result applies to this configuration”; or “this provider grant permits this resource use during this interval.” Name the basis and responsible decision-maker when reliance on that statement matters.

Distinguish a missing fact from evidence that a proposed relation does not obtain. Missing permission does not establish forbiddenness; it means the action lacks the required permission basis. Conversely, a positive relation claim can still be unusable when an endpoint, scope or time binding is missing.

Follow only the couplings that can change the current decision. If another step is unaffected, leave its details with its own account rather than reconstructing it here.

### OPS.11:4.4 - Compare coordinated alternatives {#compare-coordinated-alternatives}

Trace the finite change through the selected couplings. Compare the current arrangement with feasible alternatives, preserving the operating-result unit, horizon, acceptance conditions and protected consequences.

Include resource demand, service effects, financial timing, recovery, human burden and other consequences only when they can change the choice. Obtain financial quantities from the responsible financial Method and assumptions; a generic “value” label cannot stand in for cash, cost, obligation or benefit. Do not add unlike quantities into one score without an applicable comparison rule.

Check that the proposed decisions can coexist. A new release limit can overload a shared acceptance activity; a batch change can delay the information needed for another decision; an earlier delivery can require funding or access that has not been supplied. Use OPS.10 for the relevant load/service question and OPS.9 when the claimed limiting mechanism is still uncertain.

When the operating model itself needs to be built or reconciled, use OPS.11.1 to connect activities, shared resources, branch joins and completion at the required scales. Reuse an adequate model when the needed couplings are already represented.

Keep modeling assumptions and evidence limits visible. A simulation can compare its modeled alternatives; it does not establish that the actual operation has the same relations or effects.

### OPS.11:4.5 - Obtain or return the coordinated decisions {#obtain-or-return-the-coordinated-decisions}

Name which operating policies can change within existing authority, which decisions must be obtained from other holders, and what remains held until an unresolved result is supplied. Distinguish an agreed coordinated plan, a proposed plan awaiting decisions, and the observed implementation.

Return the smallest actionable account: the selected change or alternatives, operative couplings, affected decision-makers, conditions and sequence needed for compatibility, protected consequences, unresolved inputs and next review. Use the existing operating account where it can carry that meaning.

A coordination result can be a partial agreement plus an exact missing return. Do not hide a missing clinical, safety, legal, financial, capability or release decision behind a complete-looking network diagram.

### OPS.11:4.6 - Observe the consequences and reopen the affected part {#observe-the-consequences-and-reopen-the-affected-part}

After authorized implementation, inspect the accepted result and the affected coupling assumptions. Reopen the relevant decision when a provider changes access, evidence applies to another configuration, an acceptance condition changes, a resource becomes unavailable or an affected party's commitment changes.

When observation, actuation, supervision or feedback changes the operating choice, recover those actual relations and their delays through the current FPF control and temporal patterns. A shared dashboard does not establish the two-sided relations or response properties.

An organization-design, capability-realization or product/service-engineering change returns to its owning practice. Keep a bounded operating adjustment local when that larger change is not needed.

## OPS.11:7 - Conformance Checklist {#conformance-checklist}

1. Is one operating change or conflict and its intended result clear?
2. Are the selected actual structures distinguished from their views and mathematical descriptions?
3. Does each consequential coupling have recoverable participants, relation, conditions, timing and basis?
4. Are incompatible units and protected consequences retained in the comparison?
5. Can the proposed decisions coexist under the actual resource, evidence and authority conditions?
6. Does the result distinguish agreed change, proposed change, missing return and implementation evidence?
7. Is the next change that reopens each affected decision explicit?

Recognition means a practitioner can produce this bounded coordination result. Assurance requires the obtaining relations, qualified consequences and authority on which the chosen action relies; a complete map supplies none of them by itself.

## OPS.11:9 - Consequences {#consequences}

The operation can coordinate a change without making local gains invisible to affected participants. A small coupling account can prevent incompatible schedules, unsupported release claims and displaced costs.

The cost is recovering the relations and obtaining decisions across boundaries. Some outcomes remain partial because another practice owns a necessary result. That partial result is useful when it identifies the exact next decision and preserves what can already proceed.

## OPS.11:12 - Relations {#relations}

OPS.1–OPS.4 supply the operating focus, relevant views, subject distinctions and qualified current claims. OPS.8–OPS.10 supply queue, diagnostic and capacity results that can require coordination. OPS.5–OPS.7 consume the resulting conditions within their own admission, continuation, priority and commitment questions.

Current FPF A.22, E.18, E.18.2 and E.18.NET govern selected structures and their descriptions; A.6.REL governs direct relation questions. C.11.CRC and C.11 govern finite comparison and choice. B.2.5 and the current control/temporal patterns apply when actual supervision, feedback and response timing affect the choice.

Organization Change Engineering supplies a relevant organization or coexistence Method only at its current scope; a case-specific result still has to exist. Engineering, clinical, safety, labor, legal, financial and other practices retain their direct decisions. OPS.12–OPS.18 provide their own human-condition, service, financial, account, Method-improvement, repertoire and quality Methods. OPS.19 consumes an OPS.11 coupling result only when several otherwise valid operating results conflict across subjects, scales, or horizons. OPS.16 local Method improvement and OPS.20 cultural continuation remain separate questions with their own evidence and authority.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-3#root, spec://ai.lev/fpf-eng-ops/contract/OPS-4#root; conditional spec://ai.lev/fpf-eng-ops/contract/OPS-8#root–spec://ai.lev/fpf-eng-ops/contract/OPS-10#root; FPF spec://ai.lev/fpf-spec/contract/A-22#root, spec://ai.lev/fpf-spec/contract/E-18-NET#root, spec://ai.lev/fpf-spec/contract/C-11-CRC#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-eam/contract/EAM-14#root, spec://ai.lev/fpf-eng-eam/contract/EAM-6#root, spec://ai.lev/fpf-eng-ops/contract/OPS-10#root, spec://ai.lev/fpf-eng-ops/contract/OPS-11-1#root, spec://ai.lev/fpf-eng-ops/contract/OPS-19#root, spec://ai.lev/fpf-eng-ops/contract/OPS-8#root, spec://ai.lev/fpf-eng-ops/contract/OPS-9#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-11
