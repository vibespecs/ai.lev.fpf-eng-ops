# OPS.11 - Coordinate Interacting Operating Structures: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.11:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.11:5.1 - PumpWorks: a rig plan is not a release decision {#pumpworks-a-rig-plan-is-not-a-release-decision}

PumpWorks continues weekly evidenced controller releases while incident I73, release candidate R42, safety question S19 and provider change P8 coexist. In this constructed use, the four ready test packages carry eight rig-hours of estimated load. The current capacity comparison names actual usable rig windows rather than the number of board cards.

The question is whether a changed readiness and rig-access plan can support the release work without losing another necessary condition.

| Selected structure or relation set | Concrete coupling needed for the decision | Receiving action |
| --- | --- | --- |
| rig-use arrangement | provider access, qualified operator and configuration jointly permit the specified test during the booked window | choose only feasible slots and return changed access to OPS.10 |
| test-evidence relations | T9's result must concern the configuration used for R42's release decision | preserve configuration/result correspondence; a result for another version does not close the evidence gap |
| release-supervision relations | ReleaseSupervisorTeam-S2 uses the required evidence and safety result to issue its authorized release, hold or other decision | obtain that decision separately from completing the test |
| existing service commitments | the evidenced-release horizon has parties, conditions and authority for revision | return changed feasibility to OPS.7 and the commitment holder |

Suppose lab-test permission is current and S19 concerns field release. The coordinated result can permit T9 within its actual test conditions, keep the field release held pending S19 and the release decision, and request the needed provider access. If S19 also governs the lab test, that test lacks a sufficient permission basis and remains held too; the diagram cannot decide that scope.

OPS.8 maintains the ready queue and keeps incomplete matters visible. OPS.9 distinguishes readiness loss from an unsupported rig-bottleneck claim. OPS.10 compares the usable windows with eligible load and recovery scenarios. OPS.11 returns the compatible decisions and the missing safety or provider result to the appropriate owner.

If P8 reduces available rig time, reopen the capacity and dependent admission/release-policy decisions. Do not reinterpret a completed test as approval to bypass S19 or as evidence that the weekly service commitment has been fulfilled.

This case does not require claiming that every row is an independent flow structure. The selected permission, evidence, supervision and commitment relations are sufficient for the stated coordination question.

### OPS.11:5.2 - Chemical make-to-order: material completion and document work {#chemical-make-to-order-material-completion-and-document-work}

In a chemical make-to-order setting, goods issue depends on both available product and required commercial documents. The same order-processing resource can be needed for new-order transactions and invoicing. A material-only plan can therefore produce stock that cannot be shipped under the actual transaction conditions.

The first coordination result names that shared-resource and shipment-prerequisite coupling, then compares a compatible transaction/release policy with the local manufacturing plan. Actual commercial rules, financial consequences and authorization remain supplied inputs. The [Perez et al. (2023) model](https://doi.org/10.1016/j.compchemeng.2023.108363) is a worked comparison of this kind, not proof of a particular plant's realized improvement.

### OPS.11:5.3 - AI-assisted operation: generation, acceptance and deployment {#ai-assisted-operation-generation-acceptance-and-deployment}

An AI-assisted software operation can generate candidate changes faster while human acceptance, test environments or deployment permissions remain unchanged. Candidate changes, tool calls, episodes, evidence and accepted releases have different identities and resource demands.

The practitioner follows only the relevant couplings: which configuration a test supports, who can accept the change, which provider/tool access is available, and what deployment conditions apply. A useful result might reduce admissions to the acceptance capacity, reserve a compatible test environment and return an unresolved release decision. It does not infer agent capability or software assurance from a higher generation count.

## OPS.11:6 - Bias-Annotation {#bias-annotation}

| Bias | Consequence | Countermeasure |
| --- | --- | --- |
| diagram realism | A represented connection is treated as an obtaining relation. | Recover participants, relation basis, constraints and use. |
| one-flow reduction | Money, decisions, materials and evidence are merged because all are drawn as arrows. | State each relation and quantity under its own meaning. |
| department-boundary bias | A provider, customer or neighboring service consequence is omitted. | Select affected participants by the operating consequence. |
| local optimum confidence | A feasible local plan is treated as a feasible end-to-end plan. | Trace the necessary cross-structure conditions and shared resources. |
| authority aggregation | One coordinator appears able to grant every participating decision. | Obtain or return decisions to their actual authority holders. |

## OPS.11:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Failure | Repair |
| --- | --- | --- |
| Call every connected diagram a flow network. | Different structures and descriptions are collapsed. | Apply A.22/E.18/E.18.NET only to the object that meets the corresponding conditions. |
| Optimize material production while ignoring transaction prerequisites. | Product can accumulate without an admissible shipment. | Recover the actual goods-issue and shared-resource coupling. |
| Use evidence from the wrong configuration. | A completed test does not support the current release claim. | Bind the result to the exact subject and conditions. |
| Turn missing information into a negative world claim. | Lack of evidence is mistaken for evidence of absence. | Return the exact unresolved basis and its consequence for use. |
| Treat a coordinated diagram as permission. | The relevant decision-maker may not have authorized the action. | Obtain or return the required decision explicitly. |
| Map the enterprise before answering a small question. | Modeling effort displaces the useful operating result. | Select only relations that can reverse the current choice. |

## OPS.11:10 - Rationale {#rationale}

Cross-structure coordination is needed because one operating result can depend on relations that no single view preserves. The useful unit is not the biggest possible model; it is the set of couplings that can change a concrete decision.

Retaining different relation meanings also preserves responsibility. A financial consequence, a safety permission and a causal explanation can all constrain the same plan while requiring different evidence and different decisions.

## OPS.11:11 - SoTA-Echoing {#sota-echoing}

| Practice question and selected line | Serious alternative, trade-off and pattern change | Source roles, limits and reopen condition |
| --- | --- | --- |
| How can a locally feasible plan fail at completion? **Adapt** coordination of actual material, transaction and shared-resource prerequisites. | A material-only or transaction-only plan is cheaper but can omit a condition that makes its result unusable. Sections 4.3–4.5 and 5.2 retain the coupling and compare only the detail needed for the decision. | [Perez et al. (2023)](https://doi.org/10.1016/j.compchemeng.2023.108363) supplies a coupled-scheduling candidate and modeled failure evidence. Its chemical-supply-chain simulations do not validate every operation or a universal financial objective. Reopen when the business rule, shared resource or material/transaction coupling changes. |
| How much cross-structure representation is useful? **Adapt** a question-relative selection of obtaining relations at the relevant scales. | One universal flow diagram loses relation meaning; an exhaustive enterprise map costs more than some local decisions warrant. Sections 4.1–4.3 and 5.1 use a small actual-coupling account and keep descriptions separate. | [Wassick and Perez (2025)](https://doi.org/10.1002/aic.18688), §§3.2–3.5, supplies the current network-of-networks perspective. A.22 and E.18.NET supply the exact structural distinction. The perspective does not establish realized autonomous coordination or make every relation a flow. Reopen for a missing decision-changing structure or a simpler adequate representation. |
| Can faster software generation be treated as faster service? **Adopt** subject-correct coupling of generation, evidence, acceptance and permission. | Counting episodes or artifacts is cheaper but can omit acceptance capacity and deployment conditions. Section 5.3 retains the accepted-result boundary while 4.4 traces resource and permission consequences. | The existing Operations subject/current-account Methods and current FPF evidence and relation patterns supply the governing distinctions. They do not establish model capability, software assurance or field performance. Reopen when the actual acceptance path, provider constraint or evidence binding changes. |


## OPS.11:End {#end}
