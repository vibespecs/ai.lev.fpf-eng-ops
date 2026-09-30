# OPS.2 - Select Work-Management Views and Coordination Methods: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.2:5 - Archetypal Grounding — PumpWorks Mixed Operating Views {#archetypal-grounding-pumpworks-mixed-operating-views}

`PumpWorks-ControlServiceOps` coordinates several unlike questions:

| Current question | Selected view and Method contribution | Boundary |
| --- | --- | --- |
| How should `FieldIncident-I73` continue after new field evidence? | Case view over the field installation, incident state, commitments, evidence, authority, and permissible next Work. | The ticket is a record; safety and product decisions retain their owners. |
| How is release evidence repeatedly produced and checked? | Process view of the recurring validation Method and its input/result relations. | A process description does not establish that an occurrence happened or conformed. |
| How is a time-bounded provider-platform migration coordinated? | Project and, when several projects are coordinated, programme views of commitments, WorkPlan content, decisions, allocations, and closure. | The plan is not performed Work, adoption, or benefit. |
| How is scarce rig access coordinated across eligible requests? | Queueing view over exact request membership, order/service relation, waiting, resource access, and policy. | Establish request membership, service order, and resource access for this queueing view; a board column alone does not establish them. |
| Which observations and interventions matter at unlike rates? | Conditional control-structure views for the product-side plant/controller/observer/supervisor relations and the operating-supervision relation. | FPF owns the generic structures and rate claims; the diagram is neither the account nor the Operations Method. |

The views preserve correspondences to `ReleaseCandidate-R42`, `FieldIncident-I73`, `SafetyQuestion-S19`, `ProviderChange-P8`, the test rig, commitments, evidence results, and decisions. The incident case can request a validation-process occurrence; that occurrence can consume rig capacity; its evidence can inform the weekly release decision; a platform-migration project can change provider access. None of these relations makes the views one structure.

The product-control structure has `FieldPumpInstallation-P4` as plant, `FieldTelemetryObserver-O4`, `DeployedController-C17`, and `FieldModeSupervisor-S1` only where their direct relations obtain. The operating-supervision structure has `ReleaseSupervisorTeam-S2` receive operating-state reports and return release, hold, rollback, or permitted-mode constraints to the operating System. The timing claims remain separate: sub-second product control, minute-to-hour field observation, daily incident triage, weekly release, and slower provider change. OPS.2 selects their use; it establishes no feedback closure, stability, safety, or authority.

Reopen the mode decision when a new subject cannot be related across views, a plan repeatedly fails after new facts, queue policy changes a commitment, a control relation becomes decisive, or maintaining one view costs more than the decision value it supplies.

## OPS.2:6 - Bias-Annotation {#bias-annotation}

| Recurring bias | Likely drift | Repair |
| --- | --- | --- |
| one-true-kind bias | Work is declared inherently project, process, or case. | Recover the question, subject, and selected view; preserve Work identity. |
| tool ontology bias | The tracker schema decides which objects and states exist. | Identify subjects and relations first; treat the schema as representation. |
| hybrid-label bias | “Hybrid” hides missing correspondences and decision rules. | State subject/grain mappings, commitments, coexistence, conflicts, and stops. |
| process-normality bias | Exceptions are forced back into the designed route. | Use a case view when new facts change permissible next Work. |
| project-temporariness bias | Continuing operation is treated as a project deliverable. | Keep the time-bounded change view separate from ongoing service Work. |
| loop-as-method bias | A feedback diagram becomes the whole Operations Method. | Use the conditional FPF control branch and retain the operating decision separately. |

## OPS.2:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Repair |
| --- | --- |
| “Everything is a process.” | Identify changing subjects and ask whether discretionary or constrained case continuation is needed. |
| “Every initiative is a project.” | Separate time-bounded change commitments from recurring and continuing operation. |
| “Case management means no process.” | Retain reusable Methods and recurring subwork while letting subject state govern permissible next Work. |
| “Put all work in one queue.” | Name eligibility, service/resource relation, commitment effects, and the subjects that must remain separate. |
| “Use one integrated model.” | Preserve non-isomorphic views and relate only the claims the decision consumes. |
| “The loop proves control.” | Recover actual relations and use direct rate, dynamics, evidence, safety, and assurance patterns. |

## OPS.2:10 - Rationale {#rationale}

Different views earn their place by changing a decision. Project, process, case, queueing, and control descriptions foreground unlike structures, times, and questions. Treating them as views preserves their strengths and avoids a false taxonomy of Work. Explicit mixed-mode rules then make coexistence testable without requiring one universal model.

## OPS.2:11 - SoTA-Echoing {#sota-echoing}

| Practice question | Selected current line and serious alternative | Defect overcome and governed loci | Source roles and limits | Reopen condition |
| --- | --- | --- | --- | --- |
| Which management views should coordinate one operation when project, process, case, queueing, and control questions coexist? | The selected current line is **question-relative multi-view selection with explicit subject, state, commitment, and decision correspondence**. The serious alternatives are one canonical project/process/case taxonomy and an ungoverned overlay of tool views. | A single view suppresses questions it cannot answer; an ungoverned overlay produces incompatible status, identity, and authority claims. **Adapt:** `OPS.2:4.1` selects each view from its question, `OPS.2:4.2` records correspondence and unresolved conflicts, `OPS.2:4.3` permits local addition or retirement, and `OPS.2:5` tests coexistence. **Reject:** treating a view name as the Work's ontological kind or combining views without a receiving decision. | Select each view of Work for its question, using FPF distinctions for actual structures, representations and control. CMMN, DCR, Kanban and layered-control sources address different case, workflow and control questions; compare their contributions for the views needed by the operation. | Reopen if a current integrated Method answers the unlike questions with no worse subject/state correspondence, authority clarity, repair locality, and application effort, or if repeated use changes a view's decision contribution or the minimum correspondence rule. |

The selected comparison is supported by the following bounded source roles and limits.

Project, process, case, queueing and issue-tracking descriptions can provide different views of the same Work. Select the views for their practical questions and preserve the correspondences needed to use their answers together.

| Source line | Retained contribution | Use boundary |
| --- | --- | --- |
| Current FPF `A.22`, `C.29`, `C.30.LCA`, `B.2.5`, `C.27.TA`, `C.27`, and `A.3.3` | Select actual structures and views, keep mathematical representations distinct, recover control relations, and govern rate/dynamics claims. | FPF does not choose the Operations questions, domain coordination Methods, commitments, or service consequences. |
| [CMMN 1.1](https://www.omg.org/spec/CMMN/1.1/PDF) and [DCR](https://doi.org/10.4204/EPTCS.69.5) | Case planning, runtime discretion, declarative conditions, milestones, and responses can support continuation after new facts. | The specifications supply different case and constraint formalisms, not one complete Operations Method or universal case ontology. |
| [The Kanban Guide 2025.5](https://kanbanguides.org/the-kanban-guide/2025.5/) | Define a workflow, Work items, states, active-item management, and flow measures for a bounded Kanban use. | Kanban is one Method that can coexist with project, case, control, or other views; it does not establish comparative dominance. |
| Layered-control and LCA sources, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Make observer, controller, plant, supervisor, observation, actuation, feedback, and unlike rates visible. | Current FPF owns the generic control structure and claim discipline; source labels establish neither operating Method nor stability or safety. |


## OPS.2:End {#end}
