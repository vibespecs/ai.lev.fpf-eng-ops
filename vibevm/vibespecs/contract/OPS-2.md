# OPS.2 - Select Work-Management Views and Coordination Methods {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.2:0 - Use This When {#use-this-when}

Use this pattern when the same continuing Work is being called a project, process, case, workflow, queue, programme, or control loop and that choice changes coordination. Enter when one view hides a decision that another exposes: a process map may not show a permissible next action for an exceptional case, a project plan hides recurring service, a case file hides aggregate load, a queue hides commitments and subject state, or a loop diagram hides the operating account.

The first useful move is a question-to-view decision:

> For decision `D` about subjects `S` at grain `G`, use view `V` and coordination Method `M` under conditions `C`; relate it to views `V2...` through these subject correspondences, commitments, handoffs, coexistence rules, and stop conditions.

This result need not select one permanent mode. It may choose one view, several compatible views, or no new view when the existing coordination already answers the question.

Recognition is cheap: enter when practitioners disagree about “what kind of Work this is” or cannot answer a current question from the existing view. Assurance is heavier: selected structures, direct relations, Work, Methods, planning claims, control claims, rates, authority, safety, and evidence keep their own FPF or specialist tests.

Do not use OPS.2 to classify Work into a universal natural kind, infer performed Work from a plan, select a structure by diagram appearance, or prescribe one lifecycle. If the question concerns only the identity of an already selected structure, mathematical lens, or architecture view, use `A.22`, `C.29`, or `C.30.LCA` directly.

## OPS.2:0.1 - Working Distinctions {#working-distinctions}

| Name used here | Meaning |
| --- | --- |
| Work | Intended or performed activity under its governing FPF pattern. A management view describes or coordinates Work; it does not create another Work occurrence. |
| viewpoint question | The exact question a view must answer for a named user and decision, such as dates and allocation, repeatability, changing subject state, aggregate waiting, or feedback and rate separation. |
| Work-management mode | The selected use of one or more descriptions and coordination Methods for the current Work and questions. It is a decision result, not a Work kind or maturity stage. |
| project view | A description emphasizing a time-bounded undertaking, commitments, intended results, decisions, dates, WorkPlan content, allocation, dependencies, and closure conditions. |
| programme view | A description coordinating several projects or change commitments and their dependencies or intended contributions. The label does not create a containing System, benefit, or authority. |
| process view | A description emphasizing a recurring Method, inputs, results, repeated order or constraints, and control points. It does not prove that every occurrence follows the description. |
| case view | A description organized around a changing subject, current facts, commitments, discretionary or constrained next Work, exceptions, and closure conditions. The case is not its file. |
| queueing view | A description of eligible items, membership, order or service relation, waiting, arrival, departure, resource demand, and policy for one receiving question. The queue is not a board column. |
| control-structure view | A current FPF description of one selected control structure and its actual observation, actuation, reference, supervision, feedback, and rate-relevant relations. It is conditional, not an Operations default. |
| coordination Method | A reusable way of coordinating the Work under stated conditions. A view can expose what the Method needs without being that Method. |
| mixed-mode decision | An explicit co-use account stating subject correspondence, scope and grain, commitments, handoff or coexistence conditions, decision rules, conflicts, and stops among unlike views and Methods. |

## OPS.2:1 - Problem Frame {#problem-frame}

Project, process, and case management are often offered as competing descriptions of reality. Operations practice then chooses a tool or school and lets its default object model decide what exists. Yet one release operation can have a project for platform migration, a recurring process for validation, cases for field incidents, a queue for a scarce test rig, and a control view for observation and intervention at unlike rates.

These views are useful when they supply information needed by the receiving decision. They need not be isomorphic. Select each for the question it can answer and preserve correspondence where decisions cross them.

## OPS.2:2 - Problem {#problem}

One-mode selection loses information. A process-only account can force evolving cases through a route whose next Work depends on new facts. A case-only account can hide repeatable validation and shared capacity. A project-only account can treat continuing service as a temporary deliverable. A queue-only account can optimize waiting while breaking a commitment. A control-only account can turn observation and actuation into a complete management Method.

The opposite failure is an ungoverned hybrid: every tool and view is kept, but subjects, grains, states, and decisions disagree. Participants spend more effort reconciling records than coordinating Work.

## OPS.2:3 - Forces {#forces}

| Force | Tension |
| --- | --- |
| Familiar methods | Teams can act quickly with a known project or process Method, while familiarity can hide the wrong question. |
| Several truths | Unlike views can all be useful, while their subjects and state claims may conflict. |
| Runtime discretion | Some Work can be planned, while new facts require case-responsive continuation. |
| Aggregate coordination | Individual cases need attention, while shared queues and resources require a population view. |
| Control language | Feedback and rate distinctions can change coordination, while a loop diagram can overclaim stability, safety, or authority. |
| Affordability | A full multi-model account is expensive, while one view may omit the next decision. |

## OPS.2:4 - Solution {#solution}

Select views and coordination Methods from the operating questions they must answer. Preserve Work identity across views, select actual structures independently, and combine only those views whose distinct information changes the decision.

### OPS.2:4.1 - Pattern-Use Unfolding {#pattern-use-unfolding}

1. **Recover the operating input.** Start from the OPS.1 operating System, continuing result, commitments, subjects, units, horizon, and decision. Stop if the mode question is only a label preference.
2. **List the viewpoint questions.** Name each user, decision, subject, grain, horizon, and missing information. Separate planning, recurring execution, case continuation, aggregate waiting/capacity, and control questions.
3. **Generate serious view candidates.** Include project or programme, process, case, queueing, and control-structure views only where their questions are current. Include the incumbent as the no-change option, and a simpler view when it is a plausible alternative.
4. **Compare fit to the current Work.** Examine predictability, recurrence, subject identity, decision latency, runtime discretion, plannability, shared-resource coupling, exception frequency, evidence refresh, and authority. These are comparison prompts, not a universal scoring formula.
5. **Select the coordination Method separately.** State which reusable coordination Method is used with each view, its applicability, burden, evidence, and stop. A notation, board, model, or view does not establish a Method.
6. **Select actual structures independently.** Use `A.22` when a transformation-flow, queue/resource-dependency, commitment, event, case-state, control, or other actual structure changes the decision. A mathematical graph or diagram remains a representation.
7. **Use the control branch conditionally.** When observation, decision, actuation, supervision, feedback, or rate separation changes coordination, use `A.22` and `C.30.LCA` to identify one selected control structure and recover the needed view. Use `B.2.5` only for an obtaining two-sided supervisor relation and `C.27.TA`, `C.27`, or `A.3.3` for the exact rate, temporal, or dynamics claim. Stop without a control view when no control relation changes the decision.
8. **Compose views explicitly.** State subject correspondences, scope and grain, governing commitments, state correspondence, handoff or coexistence conditions, decision rights, update rules, conflicts, and stop conditions. Do not rely on a “hybrid” label.
9. **Test with a changing case.** Ask what happens when new evidence defeats the plan, a case crosses a process boundary, queue delay changes a commitment, or control evidence arrives at a different rate. Repair only the affected view or correspondence.
10. **Return and reopen.** Record selected and rejected views, coordination Methods, unresolved correspondences, next subject-account need, and one observation that reopens the decision.

### OPS.2:4.2 - Record the Result {#record-the-result}

| Result position | Required content |
| --- | --- |
| use boundary | Users, decisions, subjects, grains, horizons, and useful stop. |
| viewpoint questions | The planning, recurrence, case-state, aggregate waiting/capacity, control, or other exact questions that remain current. |
| candidate views | Incumbent (no change), serious alternatives, selection reasons, rejected uses, and missing evidence. |
| coordination Methods | Named Methods, applicability, burden, evidence, authority, and stops; no identity with the view or tool. |
| selected structures | Exact actual structures and direct relations relied on, plus representation and mathematical-lens boundaries. |
| mixed-mode correspondences | Subjects, grains, commitments, state correspondence, handoffs/coexistence, update and decision rules, conflicts, and stops. |
| control branch | Selected FPF control view and relied-on relations/rate claims, or an explicit `not current` or return result. |
| continuation | Inputs supplied to OPS.3/OPS.4 and an observable reopen condition. |

### OPS.2:4.3 - What Changes in Practice {#what-changes-in-practice}

The team stops asking whether Work “is” a project, process, or case. It asks which descriptions and coordination Methods answer each decision, then relates them through exact subjects and commitments. A view can be added, narrowed, or retired without retyping the Work or rebuilding every other view.

## OPS.2:7 - Conformance Checklist {#conformance-checklist}

- [ ] The decision begins with an OPS.1 operating focus and exact viewpoint questions.
- [ ] Work identity is preserved across every selected view.
- [ ] Project, programme, process, case, queueing, and control are selected for questions rather than declared natural Work kinds.
- [ ] Coordination Methods, views, actual structures, diagrams, and tools remain distinct.
- [ ] Selection considers predictability, recurrence, subject identity, decision latency, runtime discretion, plannability, and relevant coupling without pretending to use a universal score.
- [ ] Every mixed-mode use states subject and grain correspondence, commitments, coexistence or handoff, update and decision rules, conflicts, and stops.
- [ ] The control branch names actual participants and direct relations only where they obtain and returns rate/dynamics claims to their FPF owners.
- [ ] A changed case or cross-view probe can expose a failed selection or correspondence.
- [ ] Rejected views, unresolved gaps, next inputs, and a reopen condition are explicit.

## OPS.2:9 - Consequences {#consequences}

The pattern lets an operation combine familiar management practices without letting any one practice define the ontology. It makes view debt visible: missing correspondences, duplicated state, stale mappings, and coordination cost become explicit decision inputs.

The cost is maintaining subject and state correspondence where several views are genuinely useful. Some integrations are rejected because the views answer no different question or cannot preserve identity and commitments reliably.

## OPS.2:12 - Relations {#relations}

- `OPS.1` supplies the operating System, continuing result, commitments, subjects, units, horizon, and control concern.
- `A.22` governs selected structures; `C.29` governs mathematical-lens use; `C.30.LCA`, `B.2.5`, `C.27.TA`, `C.27`, and `A.3.3` govern the conditional control branch.
- `OPS.3` receives selected subjects, grains, view correspondences, direct-relation questions, and representation gaps. `OPS.4` receives the selected participant views and their state-correspondence obligations.
- `OPS.5` later consumes the selected coordination form for admission. `OPS.6` later consumes case-state and continuation needs. `OPS.8`–`OPS.11` later consume queue, constraint, capacity, and interacting-structure questions without making those structures values of one mode taxonomy.
- Project Management, case management, BPM, Kanban, SRE, and other practices offer candidate coordination Methods. Select a particular Method using its applicability conditions and evidence.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-1#root; FPF spec://ai.lev/fpf-spec/contract/A-22#root, spec://ai.lev/fpf-spec/contract/C-29#root; conditional spec://ai.lev/fpf-spec/contract/C-30-LCA#root, spec://ai.lev/fpf-spec/contract/B-2-5#root, spec://ai.lev/fpf-spec/contract/C-27-TA#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-ops/contract/OPS-3#root, spec://ai.lev/fpf-eng-ops/contract/OPS-4#root, spec://ai.lev/fpf-eng-ops/contract/OPS-5#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-2
