# OPS.3 - Distinguish Operating Subjects, Cases, Queues, Resources, and Records {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.3:0 - Use This When {#use-this-when}

Use this pattern when one card, ticket, order, object identifier, case file, event row, or status label is being asked to stand for several different things. Enter when a measure cannot say what it measures, a queue cannot say what waits, an incident record is treated as the incident, a resource is treated as its availability, or two views cannot agree because they identify their subjects differently.

The first useful move is to choose one decision-bearing subject and write:

> Subject `S` is of `kind K`, with identity condition `I`. The decision-bearing claim `Q` about `S` and its relations `R` to Work and commitments is qualified for time or horizon `T`, supported by evidence `E`, and represented in record or view `V`. Missing identity or relation governor: `G`.

Repeat only for items whose distinction changes the decision. The result is a small operating-subject account, not a universal data model.

Recognition is cheap: enter when a record label, metric denominator, queue item, or “work object” has several plausible referents. Assurance is claim-specific: entity kinds, Work, relations, commitments, state, evidence, event occurrence, control participation, resource availability, and representation each retain their FPF or specialist tests.

Do not use OPS.3 to model every object in the operation, redesign a database, declare an event log complete, infer a case from a ticket, or create a catch-all `operational object` kind. If an existing subject pattern already answers the identity or relation question, use it and record only the Operations correspondence needed here.

## OPS.3:0.1 - Working Distinctions {#working-distinctions}

| Name used here | Meaning |
| --- | --- |
| operating subject | The exact entity, relation, case subject, material, service, account, or other concern whose state or relation changes the operating decision. This is a reading position, not a new universal kind. |
| case | One bounded continuing Work situation organized around a named subject, commitments, current facts, evidence, authority, permissible next Work, and closure conditions. The case is neither its file nor every Work item within it. |
| Work occurrence | Actual dated Work admitted through its governing pattern. A ticket, plan, or event record does not establish that Work occurred. |
| Work item | A bounded item admitted to a selected workflow or coordination account with stated start, finish, subject/result relation, and receiving use. |
| queue membership | An obtaining relation placing one eligible item in one named waiting or service order under a policy and time window. A column or list is a representation. |
| buffer membership | An obtaining relation to a bounded protective or coordination reserve with purpose, policy, extent, and receiving use. It is not inferred from spare inventory or a board column. |
| resource relation | The exact availability, access, consumption, support, allocation, or other relation through which a System, capability, material, information, time, or condition is used by Work. The resource and relation remain distinct. |
| event | An occurrence or change under its subject rule and time boundary. An event record or timestamp is evidence about it, not the event by identity. |
| record or trace | A claim-bearing episteme about subjects, Work, events, relations, or decisions, recorded on an identified carrier. Its claims have stated sources and scope limits. |
| state claim | A qualified claim about one subject at a stated time or horizon with provenance, uncertainty, conditions, and authority. A status label is one possible representation. |
| control participant meaning | Observer, controller, plant, or supervisor as the participant meaning in one actual direct relation and selected control structure. The label is not a universal kind or proof that the relation obtains. |
| operating-subject account | The smallest relation-specific set of identities, direct relations, records, state claims, and explicit gaps needed by the current operating decision. |

## OPS.3:1 - Problem Frame {#problem-frame}

Operational tools compress the world so people can coordinate. That compression is useful until one row is read as the customer, order, case, Work, queue position, resource claim, event history, and current state at once. Object-centric and case-responsive approaches repair parts of this problem, but their own records and identifiers still need receiving-use limits.

The practitioner needs a small account that restores identity and obtaining relations before measures and policies are applied. The account can use several records and views while keeping the world-side subjects and claim-bearing epistemes distinct.

## OPS.3:2 - Problem {#problem}

When identities collapse, flow measures acquire false denominators, cases close while the conditions they were meant to resolve persist, queue policies compare unlike items, resources are double-counted, and events are reconstructed into Work that may never have occurred. A record update can then masquerade as an operational change.

The opposite failure is an enterprise ontology project. It delays action, imports tool categories as truth, and still may omit the few direct relations that the current decision consumes.

## OPS.3:3 - Forces {#forces}

| Force | Tension |
| --- | --- |
| Coordination shorthand | One ticket or identifier is affordable, while it can hide several subjects and relations. |
| Measurement | Stable units enable comparison, while identity changes and joins can silently change the measured population. |
| Several records | Logs, trackers, files, and physical observations can complement one another, while their claims may conflict. |
| Runtime change | Cases and subjects evolve, while records arrive late or use stale identity rules. |
| Resource scarcity | Capacity decisions need resource relations, while people and machines must not be reduced to scalar capacity. |
| Minimality | The operation needs decisive distinctions now, while a complete domain model is expensive and brittle. |

## OPS.3:4 - Solution {#solution}

Build the smallest operating-subject account that preserves exact identities, obtaining relations, time, evidence, and representation for the current decision. Start from the subjects and views selected by OPS.1 and OPS.2; add no item merely because a source schema contains it.

### OPS.3:4.1 - Pattern-Use Unfolding {#pattern-use-unfolding}

1. **Name the receiving decision and suspected compression.** Name the two items being treated as the same, the measure, queue, case continuation, commitment, control question, or account use that depends on that identity assumption, and what fails if the assumption is false.
2. **Select the primary subject.** Name the entity or relation whose state changes action and its identity condition across time. Use its direct subject pattern when kind membership is load-bearing.
3. **Separate case, Work, and Work item.** Name the case subject and closure conditions; admit actual Work independently; define each coordination Work item by start, finish, subject/result relation, and receiving use.
4. **Recover queue and buffer relations.** Name eligible item, queue or buffer, membership interval, order or protective purpose, policy, resource/service relation, and evidence. A drawn position creates none of these facts.
5. **Recover resources through exact relations.** Distinguish the System, capability, material, information, access condition, or time from availability, access, allocation, support, consumption, or other obtaining relation. Preserve authority and human-condition questions.
6. **Separate events, records, and state claims.** Identify the occurrence or changed subject; identify each record and carrier; state what claim it supports, source, time, uncertainty, and limit. Do not reconstruct Work from event order alone.
7. **Recover commitments and direct relations.** Use `A.6.REL` or the direct governor for each relied-on relation. Keep promise, obligation, fulfilment, responsibility, authority, assignment, and evidence distinct.
8. **Apply the control branch only when selected.** Preserve actual Systems or holons and direct observation, actuation, reference, supervision, and feedback relations. Treat observer, controller, plant, and supervisor as relation-specific meanings. Use `B.2.5` only when both observation/report and returned influence/constraint sides obtain.
9. **Reconcile records by subject and claim, not by row.** State correspondences, conflicts, missing joins, identity changes, currentness limits, and which source can support which decision. Keep unresolved claims visible.
10. **Stop at the smallest sufficient account.** Return exact subjects, direct relations, records, state claims, gaps, and reopen conditions to OPS.4. Leave unrelated objects outside.

### OPS.3:4.2 - Record the Result {#record-the-result}

| Result position | Required content |
| --- | --- |
| use boundary | User, decision, horizon, suspected compression, and useful stop. |
| subjects and identity | Exact primary and related subjects, governing kinds or predicates, identity conditions, and unresolved referents. |
| cases and Work | Case subject and closure; actual Work basis; Work-item start/finish, subject/result relation, and receiving use. |
| queue, buffer, and resource relations | Participants, membership or access interval, purpose/policy, order or extent, direct relation, and evidence. |
| events and records | Occurrences, claim-bearing records and carriers, source, scope, time, uncertainty, and non-admissible inferences. |
| state and commitments | Qualified state claims, commitment relations, provenance, authority, conflicts, and currentness. |
| control relations | Actual participant meanings and observation/actuation/reference/supervision/feedback relations, or an explicit `not current` result. |
| continuation | Account content supplied to OPS.4, explicit gaps, and observable reopen conditions. |

### OPS.3:4.3 - What Changes in Practice {#what-changes-in-practice}

Measures, queues, and dashboards acquire named subjects and relation semantics. A card move updates the record. Separately establish any change in the subject or relation that the updated record represents. Teams can keep several tools while knowing which claim each can support and where a missing identity or relation blocks action.

## OPS.3:7 - Conformance Checklist {#conformance-checklist}

- [ ] The account begins from one receiving decision and a named suspected compression.
- [ ] Each decision-bearing subject has an identity condition and direct subject governor when needed.
- [ ] Case, actual Work, Work item, queue membership, buffer membership, resource, event, record, and state claim remain distinct.
- [ ] Work items state start, finish, subject/result relation, and receiving use.
- [ ] Queue, buffer, and resource claims name exact participants, purpose or policy, interval, and obtaining relation.
- [ ] Records state source, carrier, claim scope, time, uncertainty, and non-admissible inference.
- [ ] Direct relations use current governors; a representation or co-occurrence creates none.
- [ ] Control participants and two-sided feedback are recorded only where actual relations obtain.
- [ ] The result is the smallest account sufficient for the decision and names gaps and reopen conditions.

## OPS.3:9 - Consequences {#consequences}

The pattern produces trustworthy units for measurement and policy and makes cross-view reconciliation possible. It also localizes repairs: a stale record source, changed identity rule, missing relation, or uncertain state claim can reopen without rebuilding the whole operating account.

The cost is refusing convenient conflations. Some metrics and historical analyses become unusable because their unit identity or source coverage cannot be recovered. That loss is explicit rather than hidden in a precise-looking chart.

## OPS.3:12 - Relations {#relations}

- `OPS.1` supplies operating scope, subject candidates, commitments, units, and evidence questions. `OPS.2` supplies selected views, grains, correspondences, and conditional control questions.
- `A.6.REL` and direct subject patterns govern obtaining relations and identities; `C.2.1` governs claim-bearing accounts; `B.2.5` and `C.30.LCA` govern the conditional control relation/view boundary.
- `OPS.4` consumes exact subjects, direct relations, records, state claims, provenance, conflicts, permissions, and gaps.
- `OPS.8`, `OPS.9`, `OPS.10`, `OPS.11`, `OPS.12`, and `OPS.18` later consume the exact subjects and relations whose queue, constraint, capacity, interaction, human-condition, or quality claim is current.
- Data engineering, process mining, product engineering, safety, finance, law, medicine, and other specialists retain their schemas, inference Methods, evidence, and authority.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-1#root, spec://ai.lev/fpf-eng-ops/contract/OPS-2#root; FPF spec://ai.lev/fpf-spec/contract/A-6-REL#root, spec://ai.lev/fpf-spec/contract/C-2-1#root; conditional spec://ai.lev/fpf-spec/contract/B-2-5#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-adm/contract/ADM-1#root, spec://ai.lev/fpf-eng-chk/contract/CHK-5#root, spec://ai.lev/fpf-eng-ops/contract/OPS-10#root, spec://ai.lev/fpf-eng-ops/contract/OPS-11#root, spec://ai.lev/fpf-eng-ops/contract/OPS-12#root, spec://ai.lev/fpf-eng-ops/contract/OPS-15#root, spec://ai.lev/fpf-eng-ops/contract/OPS-19#root, spec://ai.lev/fpf-eng-ops/contract/OPS-4#root, spec://ai.lev/fpf-eng-ops/contract/OPS-5#root, spec://ai.lev/fpf-eng-ops/contract/OPS-8#root, spec://ai.lev/fpf-eng-ops/contract/OPS-9#root, spec://ai.lev/fpf-eng-syse/contract/SYSE-38#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-3
