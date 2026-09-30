# OPS.9 - Diagnose and Treat the Current Operating Constraint: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.9:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.9:5.1 - PumpWorks: readiness or rig capacity? {#pumpworks-readiness-or-rig-capacity}

PumpWorks coordinates weekly evidenced releases. In the constructed history, five eight-hour rig-access windows contain 20 test hours, 4 setup hours, 4 unavailable hours and 12 hours with no eligible job. Twelve matters appear on local boards at the final snapshot, but only four ready test packages require eight rig-hours.

A proposal to buy more rig time cites the twelve cards. The practitioner identifies the claimed result—accepted evidence-complete releases—and distinguishes it from test attempts and ready packages. The history supports a late-readiness explanation, but it does not rule out insufficient rig time in a later peak window.

The initial account is:

| Element | Bounded result |
| --- | --- |
| observed loss | twelve open hours without an eligible job; accepted-release shortfall still requires its own event and acceptance account |
| candidate explanation | prerequisite delivery misses usable rig windows |
| serious rival | eligible demand exceeds usable rig time in the relevant deadline windows |
| discriminating next observation | timestamp package eligibility, usable rig slots, starts, results, returns and final acceptance for the same release population |
| bounded probe | where engineering and test permissions allow, prepare the next-test inputs earlier for a comparable class; preserve test/acceptance criteria and record mix, access and shared-resource effects |
| present decision | do not infer a rig-capacity treatment from card count; operate the supported ready-queue policy and obtain the missing discriminatory basis |

If earlier readiness reduces starvation but accepted releases remain unchanged, that result does not establish completion improvement. Inspect acceptance waiting, rework and the next consequential coupling. If usable access is then reduced by ProviderChange-P8, re-evaluate the capacity explanation under the new window.

This is a completed diagnostic/probe decision. It is not a claim that the constructed probe has been performed or that late readiness has already been established as the sole cause.

### OPS.9:5.2 - A narrow capacity treatment with a feasible witness {#a-narrow-capacity-treatment-with-a-feasible-witness}

A different constructed service must finish five ready jobs within twelve hours. All upstream inputs are complete. Each job requires two hours of final verification and then ten minutes of certification; the certificate service has reserved slots after each possible verification completion. Acceptance requires both results, with no failures or rework in this stated scenario.

The verifier is available for eight hours. Verification completions occur at hours 2, 4, 6 and 8, so no more than four jobs can be accepted. Extra upstream processing capacity cannot change that bound: the five inputs are already ready.

The resource owner can supply two additional verifier-hours within the same twelve-hour horizon. With that change, the fifth verification completes at hour 10 and certification at hour 10 plus ten minutes. The comparison therefore returns a feasible five-job treatment candidate under the stated conditions. Its selection still uses the supplied resource cost, permission and protected consequences.

If certification availability later falls to two reserved slots, the old verifier treatment no longer supports five accepted jobs. The same result definition now exposes another limiting relation. Adding further verifier time cannot repair that missing certification capacity.

### OPS.9:5.3 - Faster automation without more accepted cases {#faster-automation-without-more-accepted-cases}

An operation automates a repeatable step and halves its touch time, but the same accepted-case rate remains. The practitioner keeps the accepted-case criteria, mix and observation window fixed and inspects waiting and returns at acceptance.

If cases repeatedly lack the evidence the acceptor needs, “hire more acceptors” and “complete evidence before presenting the case” are distinct treatments. The next result is the smallest justified comparison that separates those explanations. A model score or automation benchmark does not settle it.

## OPS.9:6 - Bias-Annotation {#bias-annotation}

| Bias | How it misdirects treatment | Countermeasure |
| --- | --- | --- |
| busy-resource attribution | High utilization becomes the causal explanation. | Relate usable capacity and timing to the accepted-result shortfall. |
| queue-length attribution | Visible waiting is treated as sufficient proof of the constraint. | Test eligibility, arrivals, returns and a serious rival. |
| preferred-solution bias | Automation, hiring or acquisition is selected before diagnosis. | State a defeater and compare a treatment that acts on another plausible mechanism. |
| before/after confidence | Coincident changes are attributed to the intervention. | Preserve comparison conditions and account for interference and confounding. |
| permanent-bottleneck identity | Attention remains on a resource after conditions change. | Remeasure the current limiting relation and accepted result. |

## OPS.9:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Failure | Repair |
| --- | --- | --- |
| Every operation has one permanently named bottleneck. | Distributed delay and changing regimes are excluded before observation. | State the result-relative limiting relation and allow unresolved or multiple mechanisms. |
| A fast local step proves whole-operation improvement. | Acceptance, joins and rework may dominate the result. | Preserve the accepted unit and inspect the whole relevant path. |
| A capacity ratio is a feasible schedule. | Precedence, access and simultaneous-resource conditions can defeat it. | Supply the timed witness or retain an infeasibility bound only. |
| A generic causal checklist replaces the field probe. | No actual admissible change or observation is specified. | Name the professional Method, changed action, comparison and stop. |
| A successful treatment remains the answer forever. | The arrangement and limiting relation have changed. | Reopen the account after the material change. |

## OPS.9:10 - Rationale {#rationale}

A constraint claim connects an arrangement to an operating result. Its meaning therefore depends on demand, acceptance, time and complementary resources. A resource label cannot retain that meaning when those conditions change.

Diagnosis and treatment belong together, but they are different conclusions. Keeping the rival and evidence limit visible permits action at the smallest justified scope without turning either caution or urgency into a universal rule.

## OPS.9:11 - SoTA-Echoing {#sota-echoing}

| Practice question and selected line | Serious alternative, trade-off and pattern change | Source roles, limits and reopen condition |
| --- | --- | --- |
| What should be treated when local speed does not improve accepted output? **Adapt** result-relative diagnosis followed by mechanism-specific treatment. | Constraint-focused improvement is useful, but a forced single-resource answer can miss many waits or incomplete inputs. Sections 4.1–4.3 and 5.1/5.3 preserve the accepted result and require a serious rival. The extra event discrimination is worthwhile when it can reverse treatment. | Tendon, *The Book of TameFlow* (2022), constraint and complete-kit reasoning, is a mechanism candidate. Reinertsen, *The Principles of Product Development Flow* (2009), E8's accumulated small waits, is the action-changing rival. Neither proves the current case's cause. Reopen for a different waiting mechanism or demand regime. |
| How much evidence is enough before acting? **Adapt** the least burdensome bound, replay or admissible probe that can distinguish the live alternatives. | Pure utilization ranking is cheaper but cannot support the causal move; a complete optimizer or experiment is unnecessarily costly for some bounded decisions. Sections 4.4–4.6 and 5.2 separate infeasibility, feasible scenario and actual effect. | Current FPF C.16 and C.28 supply measurement and causal-use discipline; C.11.CRC supplies finite comparison. The professional operational data, probe and authority remain case inputs. Reopen when confounding, interference or consequence makes the selected basis insufficient. |
| Should the former constraint keep receiving improvement effort? **Adopt** remeasurement of the accepted result and current arrangement after change. | A fixed improvement programme can keep optimizing a relation that no longer limits completion. Section 4.6 and the changed certification case make migration observable at modest extra comparison effort. | The constraint-refocusing line in Tendon and the changing-information reasoning in Reinertsen are compatible mechanism candidates, not guarantees of improvement. Reopen if the result, acceptance conditions or connected resources change. |


## OPS.9:End {#end}
