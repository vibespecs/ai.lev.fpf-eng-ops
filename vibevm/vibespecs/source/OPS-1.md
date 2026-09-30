# OPS.1 - Identify the Operating System, Commitments, and Flow Units: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.1:5 - Archetypal Grounding — PumpWorks Continuing Control Service {#archetypal-grounding-pumpworks-continuing-control-service}

PumpWorks must continue weekly evidenced controller releases while field incidents, provider changes, test-rig access, safety questions, and service commitments coexist.

| Candidate | Disposition for this decision |
| --- | --- |
| PumpWorks company | Too broad; corporate, financial, and legal questions remain specialist returns. |
| controller product | An engineered product and possible plant/controller participant, not the operation coordinating its continuing service. |
| field installation | A product-use and service subject whose state matters, not the whole release-and-incident operation. |
| board and issue tracker | Representations and records used by the operation; neither acts as the operating System. |
| `PumpWorks-ControlServiceOps` | Selected operating System because its continuing Work coordinates evidenced releases, incident response, provider change, rig access, and service commitments. |

The continuing results are usable evidenced releases and truthful incident/service responses, not card movement or software deployment alone. Current demand includes `ReleaseCandidate-R42`, `FieldIncident-I73`, `SafetyQuestion-S19`, `ProviderChange-P8`, and test-rig requests. They are not one unit kind.

The weekly release commitment names the product/service receivers, required evidence, release horizon, release authority, and hold conditions. Incident response has different parties and horizons. Provider access and safety review have their own commitments and authority. OPS.1 records each without ranking them by label.

The operating subjects include the release candidate, field installation, incident case, safety question, provider change, rig booking, evidence results, and service relation. A release-candidate Work item may be counted for one workflow; the incident case and field pump remain separately identified. The selected boundary excludes product redesign, safety acceptance, corporate finance, and provider-contract decisions except as named returns.

Unlike rates make a control concern current: sub-second product control, minute-to-hour field observation, daily incident triage, weekly release, and slower provider change can affect the release decision. OPS.1 passes that concern to OPS.2 without declaring a control structure, feedback closure, stability, safety, or a universal control Method.

Reopen the focus if the operation's continuing result changes, field-service Work makes another System the decision bearer, a commitment's parties or authority change, or the current units cannot preserve subject identity across the next decision.

Suppose `ProviderChange-P8` becomes a separately authorized provider-transition operation rather than Work inside `PumpWorks-ControlServiceOps`. Recheck the OPS.2 migration-project view and the OPS.4 provider-access and authority claims because they consumed that boundary. Keep the release-validation process view and the `FieldIncident-I73` case account usable while their subjects, commitments, and relations remain unchanged. Return provider-contract authority to its specialist owner. The focus record carries these three dispositions instead of discarding every downstream result.

## OPS.1:6 - Bias-Annotation {#bias-annotation}

| Recurring bias | Likely drift | Repair |
| --- | --- | --- |
| process-name bias | “The release process” becomes the operating System. | Start from the continuing result and compare exact System candidates. |
| organization-boundary bias | A department or company name fixes the operation. | Recover the Work and relations that make the bounded operation relevant. |
| ticket-as-subject bias | The record becomes the customer, product, incident, or commitment. | Name the represented subject and the record relation separately. |
| commitment-by-date bias | A due date or service target is treated as an obtaining promise or authority. | Recover parties, content, conditions, horizon, status, and authority. |
| unit-of-value bias | Every counted item is called value or flow. | State identity and receiving use; use the source-local term only within its boundary. |
| controller-name bias | A controller product makes every operating question a control question. | Enter the control branch only when control relations or rates change coordination. |

## OPS.1:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Repair |
| --- | --- |
| “Optimize the whole value stream.” | Name the operating System, receiver, result, subjects, and exact selected transformation-flow structure before optimizing. |
| “The backlog is demand.” | Distinguish external demand, candidate Work claims, admitted Work, deferred demand, and records. |
| “One ticket equals one customer outcome.” | Recover the customer or service subject, case, Work items, results, and record relations. |
| “All urgent items have commitments.” | Recover the actual promise or obligation and its authority; urgency and queue rank are separate. |
| “The board is our operating model.” | Treat the board as a representation; select the operation and decision before choosing views. |
| “The controller is the operation.” | Keep the engineered controller, controlled plant, service operation, control structure, and operating account distinct. |

## OPS.1:10 - Rationale {#rationale}

Continuing operation is coordinated through actual Systems, Work, relations, commitments, and results. A board, process description, metric, or school can help only after its subject and use are fixed. Beginning from the continuing result and decision makes the boundary small enough to use while preserving the distinctions later queue, constraint, capacity, quality, service, and improvement decisions consume.

## OPS.1:11 - SoTA-Echoing {#sota-echoing}

| Practice question | Selected current line and serious alternative | Defect overcome and governed loci | Source roles and limits | Reopen condition |
| --- | --- | --- | --- | --- |
| How should a practitioner establish the first operating focus before changing a board, policy, measure, or flow? | The selected current line is **subject-, commitment-, and decision-first**: bound the operating System or subject, continuing result, commitments, operating subjects, tracked units, authority, and evidence before selecting a management Method or representation. The serious default is **workflow- or school-first**: take an existing process, value-stream, backlog, board, or branded Method as the operation and its items as the units. | The default can optimize a representation or convenient count while the service, case, product, or commitment degrades. **Adapt:** `OPS.1:4.1` and `OPS.1:4.2` require a decision-bounded focus and consumer disposition; `OPS.1:5` demonstrates selection and local reopening; `OPS.1:7` checks that downstream consumers are rechecked without discarding unaffected results. **Reject:** a board, school, or source-local unit as the operating boundary by default. | FPF supplies System, relation, account and evidence distinctions. This pattern connects Work, Methods and the viewpoints needed for the operating decision. The Kanban Guide describes a bounded workflow. TameFlow and DEMO also examine commitments, hidden queues, interactions and coordination Work. Use these accounts to compare proposed operating boundaries. | Reopen if a stronger current comparison or repeated unlike use shows that a workflow-first entry preserves the same subject identity, commitments, specialist returns, downstream repair locality, and decision value at lower effort, or if a relied-on source changes one of those moves. |

The selected comparison is supported by the following bounded source roles and limits.

Relate Methods, performed Work, resources and the structures selected for the operating question. Projects, processes, cases and queues can expose different features of that Work.

| Source line | Retained contribution | Use boundary |
| --- | --- | --- |
| Current FPF `A.1.SCR`, `A.6.REL`, `C.2.1`, and `A.10` | Conditional System recognition, obtaining relations, claim-bearing accounts, and evidence reliance. | FPF does not select the Operations result, commitments, domain units, intervention, or service consequence. |
| [The Kanban Guide 2025.5](https://kanbanguides.org/the-kanban-guide/2025.5/) | Define a workflow and its Work items explicitly before using flow measures or active-item policies. | One minimal Kanban Method does not identify every operating System, case, commitment, physical subject, or suitable management view. |
| TameFlow 2022 and its precursor, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Distinguish optional demand from committed Work and make hidden queues, constraint, financial, interaction, and human-condition questions visible. | The four concerns do not create four transformation-flow kinds or one universal operating boundary. |
| DEMO 2020/2024, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Make production and coordination Work, commitments, parties, responsibility, and transaction structure visible. | DEMO constructs remain organization-specific source contributions and do not become FPF ontology or a complete Operations Method. |


## OPS.1:End {#end}
