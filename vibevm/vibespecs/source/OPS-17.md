# OPS.17 - Compare and Refresh Operations Methods: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.17:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.17:5.1 - PumpWorks chooses what to change {#pumpworks-chooses-what-to-change}

This constructed case concerns the engineering test service, `PumpWorks-ControlServiceOps`. Its board includes release candidate R42, incident I73, safety question S19 and provider change P8. They are unlike matters requiring different actions. Four packages are ready for testing and need eight rig-hours.

A historical forty-hour rig log contains twenty execution hours, four setup hours, four unavailable hours and twelve hours with no eligible job. The next service window has six usable rig-hours. The team compares three responses:

| Response | What the evidence supports | Result of the comparison |
| --- | --- | --- |
| Extend the rig window immediately | The four ready packages exceed the current window; more usable time could help this peak. Historical idle time does not remove that fact. | Keep a capacity alternative for OPS.10/.13, conditional on actual access, qualified cover, rework and the service horizon. |
| Admit only test-ready packages to the rig queue and make the next eligible package visible | The board count mixes unlike matters; the log also shows lost opportunities when no eligible package was available. | Select the existing readiness criteria for queue admission and make readiness timestamps available for the next operating review. |
| Treat the rig as the persistent constraint and impose a new protective buffer | The supplied log does not settle whether readiness failures, peak demand or rig access limits accepted service over the relevant horizon. | Return the constraint question to OPS.9 before choosing the buffer policy. |

The result combines a usable admission move with an unresolved capacity choice. It does not erase the four-package peak. Readiness and rig-access evidence answer different parts of the problem, so both remain in the repertoire.

The resulting instruction for the next window is concrete: use the established readiness criteria to populate the test queue; compare the six-hour plan with any authorized extension using OPS.13; reopen constraint protection if matched demand, readiness and rig-use histories show the rig consistently limiting accepted service. S19's field-release decision remains with the authorized safety and release practitioners. A permission for laboratory testing has the scope supplied by those practitioners.

### OPS.17:5.2 - A hospital continues an evolving discharge case {#a-hospital-continues-an-evolving-discharge-case}

In a constructed hospital service, a standard checklist works for the recurring discharge subprocedure, but a newly discovered home-support need changes one patient's case. Repeating the checklist cannot decide the next action. The practitioner compares a fixed sequence with conditional case planning.

The local care plan requires a qualified clinical decision and confirmation of necessary home support before discharge. The selected case rule allows the responsible practitioner to arrange assessment and support in the order the situation permits, while keeping both conditions visible. A change in support can reopen planning. The standard medication-check subprocedure remains applicable when the case reaches it.

This is a method comparison about continuing the case. The clinical judgment and the patient's actual readiness come from their own qualified work. The case account supplies the conditions and the evidence needed by the operating decision.

### OPS.17:5.3 - Faster AI drafting changes the constraint {#faster-ai-drafting-changes-the-constraint}

Suppose an assisted drafting service generates twenty candidates per day while qualified readers can accept six. A tool update raises generation to sixty; the acceptance capability stays at six. The old rule of keeping every generator busy now increases waiting and review burden.

Compare a controlled generation rate, extra qualified acceptance capacity, and a changed acceptance method. Limiting starts to the demonstrated acceptance capacity can be a current operating response. The other two choices need capability, burden and quality evidence. OPS.12 checks the transferred reading burden, OPS.13 qualifies the service commitment and OPS.18 supplies the acceptance and reliability conditions.

The repertoire refresh concerns the claim that more generation improves accepted throughput. ME.15 distinguishes a changed generation method from a support-only update. That distinction preserves what existing evidence still supports without assuming that either kind of update improves the whole service.

### OPS.17:5.4 - A current comparison and a later worthwhile trial {#a-current-comparison-and-a-later-worthwhile-trial}

For a later PumpWorks decision, admitted Method R continues to meet the package-admission requirements for the same permitted use. Proposed N combines its readiness check with a different sequencing rule. The sources and proposed interaction are traceable, but whether N preserves the permission-expiry hold while reducing repeat checks remains unsupported. No rig slot or trial permission is available before the decision window. The operating note retains R for current use and N as a candidate account with that precise gap. This completes the current comparison and lineage return.

Later, twenty-four planned package admissions make the repeated checking burden consequential. N now has a credible estimated saving of ten to fifteen minutes per admission, but preservation of the permission-expiry hold is still uncertain. A comparison of R and N on representative ordinary and expired-permission inputs can change the choice. A rig slot, qualified people and the appropriate trial permission are available. Design, performance, interpretation and return together need three of five available hours and displace no required operating Work; the potential four to six hours saved across the planned admissions makes that inquiry worthwhile.

The team selects the bounded comparison, with the permission-expiry hold as a required result and a stop if supplied support or permission ceases. R remains selected pending the result. The trial permission does not supply Method admission or authority for normal service use. Any later fit, transfer or causal claim still needs evidence adequate for that claim.

## OPS.17:6 - Bias-Annotation {#bias-annotation}

People who have invested in a school or tool can find its benefits easier to see than its operating costs. Include current practice and a simpler adequate response, and ask affected practitioners where the proposed gain creates additional work.

Available telemetry also favors measurable activity over accepted service. Inspect omitted work, blocked cases and receiving practitioners' effort before choosing comparison characteristics. The repertoire can remain small when those observations identify the only live choice.

## OPS.17:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Misuse | Working repair |
| --- | --- |
| Choose a school from a general maturity score. | Compare its actual moves against the current service problem at comparable adoption effort. |
| Protect the apparently busiest resource. | Establish which mechanism limits the named accepted result and horizon before choosing the protection. |
| Add an expedite lane while claiming an unchanged WIP policy. | State the exception authority, displaced work and recovery, and requalify the combined policy. |
| Keep evidence attached to a method name after its conditions change. | Reassess the affected applicability or effect claim and retain unaffected evidence. |
| Call a promising combination proven because its components are familiar. | Examine the available interaction evidence and keep the unproved claim as a gap in the current candidate account. Obtain more operating evidence only when its attainable contribution is worth the whole burden for the receiving decision. |

## OPS.17:10 - Rationale {#rationale}

Method-level comparison preserves the connection between a working problem and the action intended to change it. It is especially useful where several traditions overlap in vocabulary but act on different objects: a ready queue, a case, a scarce resource, a service-event population or a cash consequence.

The separate feasibility and preference steps preserve non-negotiable conditions while allowing a real choice among useful alternatives. Directed refresh then follows the claim that failed, making evidence reuse possible without treating the method as timeless.

## OPS.17:11 - SoTA-Echoing {#sota-echoing}

The practice question is how to select and maintain operating methods when demand, constraints and evidence change. The best-supported line for the uses shown here is a conditional composition of explicit work control, case continuation and decision-specific evidence. Its advantage over whole-school adoption is recoverable in the cases: it retains the ready-queue move, the peak-capacity question, case discretion and the new acceptance bottleneck separately. This is a reasoned synthesis for those uses; comparative superiority across all operations has not been established.

| Source contribution | Adopted or adapted move and serious alternative | Change in this pattern and limit |
| --- | --- | --- |
| [The Kanban Guide 2025.5](https://kanbanguides.org/the-kanban-guide/2025.5/) | Adopt explicit workflow boundaries, WIP control and elapsed-time evidence; compare with an unrestricted start policy. | Sections 4.2–4.4 require the item boundary and the consequence protected by a limit. The guide's knowledge-work metric set is not imposed on every method. |
| Steve Tendon's *The Book of TameFlow* (2022), pp. 25–27, 135 and 142, and Donald Reinertsen's *The Principles of Product Development Flow* (2009), chapters 2–9 | Adapt constraint protection and cost-of-delay questions; compare with maximizing each resource's utilization. | The PumpWorks comparison needs a diagnosed limiting mechanism and an actual service horizon. These are historical mechanisms; their age or continued use does not establish superiority. |
| [CMMN 1.1](https://www.omg.org/spec/CMMN/1.1/PDF) and the [DCR condition/response line](https://doi.org/10.4204/EPTCS.69.5) | Adopt explicit case conditions and permitted discretion where a fixed sequence cannot cover the evolving facts. | The hospital case preserves obligatory conditions while allowing a different next action. A notation does not supply clinical authority or evidence. |
| [SRE service objectives](https://sre.google/workbook/implementing-slos/), [NIST process monitoring](https://www.itl.nist.gov/div898/handbook/pmc/section3/pmc332.htm) and [lot acceptance](https://www.itl.nist.gov/div898/handbook/pmc/section2/pmc21.htm) | Select evidence by the operating question; compare with one aggregate quality dashboard. | Section 4.2 distinguishes service loss, recurring variation and lot disposition, with OPS.18 as the receiving control method. |
| [ACCA relevant-cost comparison](https://www.accaglobal.com/my/en/student/exam-support-resources/fundamentals-exams-study-resources/f5/technical-articles/relevant-costs.html) and [throughput accounting](https://www.accaglobal.com/gb/en/student/exam-support-resources/fundamentals-exams-study-resources/f5/technical-articles/throughput-constraints2.html) | Retain constrained-resource contribution and incremental cash as different comparisons; compare with a general local-efficiency ranking. | Section 4.3 preserves horizon, actual costs and accepted demand. OPS.14 develops the financial consequence; statutory or investment uses need their own methods. |
| [NIOSH's hierarchy of controls for Total Worker Health](https://www.cdc.gov/niosh/twh/php/hierarchy/index.html) | Prefer removal or redesign of harmful conditions to relying first on individual coping. | Feasibility and the OPS.12 receiving result preserve affected groups and supplied protections. |

These sources contribute different strengths: formal rules, practitioner guidance, technical models and worked financial reasoning. The repertoire preserves those evidence limits. Reopen a selected claim when a better-supported competing move, changed source meaning or changed operating condition affects the choice.


## OPS.17:End {#end}
