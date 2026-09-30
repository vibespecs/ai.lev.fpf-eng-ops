# OPS.8 - Coordinate Queues and Buffers: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.8:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.8:5.1 - PumpWorks: twelve matters, four ready test packages {#pumpworks-twelve-matters-four-ready-test-packages}

In this constructed case, PumpWorks coordinates weekly evidenced controller releases and incident response. Across five eight-hour rig-access windows, its history shows 20 hours of test execution, 4 of setup, 4 of unavailability and 12 with no eligible job. The final board snapshot contains twelve matters. Four test packages are ready and require eight rig-hours under their current estimates.

The practitioner obtains two different results from these inputs. The snapshot supports a ready queue of four packages with eight rig-hours of estimated load. The history shows lost open time with no eligible job. Neither establishes that twelve matters form one service queue or that rig capacity limits accepted releases.

The immediate policy is to book and dispatch only packages whose next-test inputs, permission and access are current; track the remaining matters by their missing inputs; and retain their waiting in the end-to-end account. The existing authorized priority rule orders the eligible packages. No new buffer quantity is claimed until replenishment and shortage consequences are known.

ReleaseCandidate-R42 lacks test evidence T9. If the inputs and lab-test permission for T9 are current, that missing output is not a reason to mark the test itself ineligible. SafetyQuestion-S19 and release authority remain separate conditions for the later release decision.

The return to OPS.9 is precise: distinguish late readiness from insufficient usable rig time as explanations for lost accepted releases. The return to OPS.10 is the eligible-load and access-window comparison, including recovery and rework. OPS.11 handles ProviderChange-P8 when its access decision changes those windows. The first policy can be used while those wider questions remain bounded and explicit.

### OPS.8:5.2 - A small protection calculation {#a-small-protection-calculation}

A service has one qualified resource, consuming one unit of ready service load per open hour. Its coordinator has a supported planning scenario in which replenishment can be interrupted for two open hours, and no other resource can serve that class. A two-unit ready buffer covers that interruption if service demand and eligibility remain as stated.

Keeping only one unit leaves one open hour exposed in that scenario. Keeping four units adds no protection needed for the specified two-hour interruption, although another supported disturbance might justify it. If the replenishment gap can instead be four hours, the two-unit conclusion reopens. The result is a scenario-qualified policy choice; a service-probability claim would need a different basis.

### OPS.8:5.3 - Patient waiting is not one interchangeable queue {#patient-waiting-is-not-one-interchangeable-queue}

A hospital coordinator receives qualified clinical eligibility and priority for a particular resource class. The operating queue includes only cases that can use that service under those conditions. Patients awaiting a different clinical decision or capability remain visible in the wider waiting account.

OPS.8 can coordinate the resource queue and readiness information. It does not supply the clinical eligibility, triage rule, consent or treatment decision. Pooling unlike service classes is not justified merely because the combined list is shorter.

## OPS.8:6 - Bias-Annotation {#bias-annotation}

| Bias | Consequence | Countermeasure |
| --- | --- | --- |
| board-boundary bias | Waiting disappears when an item leaves a local column. | Retain the operation's population and waiting origin. |
| zero-buffer ideal | Protection is removed together with avoidable congestion. | State the disturbance and shortage consequence before changing the amount. |
| complete-kit absolutism | Every future result is demanded before any useful action can start. | Define readiness for the next service, not for the whole case's eventual completion. |
| local-utilization pressure | More starts create incomplete kits and downstream waiting. | Inspect the accepted result and receiver-ready inputs. |
| pooling optimism | Mean efficiency hides class-specific or failure-related loss. | Compare the actual service criterion and resource assumptions. |

## OPS.8:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Why it fails | Repair |
| --- | --- | --- |
| Count every board item as ready supply. | Some items lack prerequisites or use another service. | Recover membership and missing-input populations. |
| Treat commitment as buffer membership. | A promise does not establish eligibility or physical protection. | State the two relations separately. |
| Size a “never empty” buffer from averages. | A mean relation does not establish the shortage tail. | Qualify replenishment scenarios and consequences through OPS.10. |
| Improve the metric by moving its start boundary. | The customer can wait just as long outside the reported queue. | Preserve the end-to-end origin and show local waiting separately. |
| Use one pooling or batch rule everywhere. | Compatibility, failure, setup and service objectives differ. | Compare the concrete alternative under the receiving operation's conditions. |

## OPS.8:10 - Rationale {#rationale}

Queue coordination works at the receiver's service boundary and at the wider result boundary together. The first prevents dispatch of unusable inputs; the second prevents hidden waiting and local improvement from replacing the actual purpose.

Protection and concurrency control are therefore selected by their effects, not by a shared label or a management school. A cheap eligibility rule can be useful before a numerical buffer study, while a numerical guarantee cannot borrow that rule's adequacy.

## OPS.8:11 - SoTA-Echoing {#sota-echoing}

| Practice question and selected line | Serious alternative, trade-off and pattern change | Source roles, limits and reopen condition |
| --- | --- | --- |
| How should local completion and downstream readiness be coordinated? **Adapt** whole-operation ready-supply and complete-kit reasoning. | Local column limits are cheaper but can miss joins; a complete-kit rule applied to the whole case can block useful investigation. Sections 4.1–4.4 and 5.1 instead bind readiness to the next service while retaining total waiting. The added input matching is justified when it changes dispatch or starvation. | Tendon, *The Book of TameFlow* (2022), complete-kit example and time-buffer discussion, printed pp. 135–137 and 141–143, is a mechanism candidate. [The Kanban Guide 2025.5](https://kanbanguides.org/the-kanban-guide/2025.5/) is the serious workflow-policy comparator. Neither establishes one policy for every operation. Reopen when the join, eligibility or receiving result changes. |
| How much protection or batching is useful? **Adapt** disturbance-specific protection and the setup-versus-delay comparison. | Minimizing every queue or batch ignores the cost of shortage or repeated setup. Sections 4.3–4.5 and 5.2 require a purpose and supported scenario instead of a universal optimum. This costs an explicit consumption/replenishment account, not necessarily a full optimizer. | Tendon's time-buffer account and Reinertsen, *The Principles of Product Development Flow* (2009), E6–E9 and Figure 5-4, supply competing mechanism candidates. Their models do not establish a protection tail or transferable batch optimum. Reopen when setup, replenishment, feedback or shortage consequences change. |
| Should eligible demand be pooled? **Adapt** model- and service-criterion-specific comparison. | Pooling can improve one mean measure while worsening a protected tail or class. Section 4.4 keeps the service criterion and failure assumptions explicit; no pool-all default is selected. | [Andradóttir, Ayhan and Down (2017)](https://doi.org/10.1016/j.ejor.2016.05.009) and [Cao et al. (2021)](https://doi.org/10.1287/opre.2019.1976) supply counterexamples under different modeled conditions. Their results do not prescribe a rig or clinical queue. Reopen for the actual routing, failure, abandonment or service-class change. |


## OPS.8:End {#end}
