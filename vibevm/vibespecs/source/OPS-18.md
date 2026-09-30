# OPS.18 - Control Operating Quality and Reliability: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.18:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.18:5.1 - A process signal calls for containment and investigation {#a-process-signal-calls-for-containment-and-investigation}

In this constructed recurring inspection operation, the supplied stable reference proportion of nonconforming items is p₀ = 0.02. Samples contain n = 200 independent, comparable items under the stated binomial basis. The local monitoring policy uses a three-standard-deviation p-chart rule and calls for segregation of the affected output and investigation when the upper limit is exceeded.

The upper limit is p₀ + 3√(p₀(1 − p₀)/n) = 0.02 + 3√(0.02 × 0.98 / 200), approximately **0.0497**, or 4.97%. The corresponding lower value is negative and is truncated to zero.

The next sample contains twelve nonconforming items: 12 / 200 = **0.06**, or 6%. This exceeds the specified upper limit. The practitioner applies the policy's containment and investigation response and identifies the sampled output, source process and current configuration.

The arithmetic establishes the signal under that rule. It does not identify why the items failed, determine another lot's disposition or show that the process is capable of meeting a product specification. The three-standard-deviation calculation defines the limit for this rule; it does not supply an exact confidence or false-alarm probability. With this low reference rate, a claim about false-alarm or missed-detection probability needs an appropriately qualified binomial or other statistical design.

Suppose the investigation finds a changed setup condition. Returning to the earlier setup and obtaining the required process and output evidence can support restart under the responsible authority. A single subsequent point below the limit is insufficient to establish every one of those claims. A persistent smaller shift may call for a monitor such as an exponentially weighted moving average (EWMA), which retains information from successive observations, if its detection properties fit the need.

### OPS.18:5.2 - Service loss exceeds the agreed budget {#service-loss-exceeds-the-agreed-budget}

In a constructed software service, the objective is **99.9% successful requests** over the defined window. The account includes 1,000,000 eligible requests, with success and eligibility measured at the service boundary relevant to users. The allowance is:

- 1,000,000 × (1 − 0.999) = **1,000 unsuccessful requests**;
- observed unsuccessful requests = **1,500**;
- budget consumed = 1,500 / 1,000 = **150%**.

The observed success proportion is 99.85%. The service has exceeded the stated allowance by 500 unsuccessful requests.

Its previously authorized local policy pauses discretionary feature releases when the budget is exceeded, permits the specified urgent recovery and security work, and requires investigation of the affected service. The practitioner applies that policy, names the eligible population and affected service, and directs the authorized recovery work. This is the policy of the constructed case; another service needs its own objective and permitted response.

A total of 1,500 also needs timely interpretation. If most failures occurred in the last few minutes or affected one important user group, the aggregate alone can understate the current incident. Inspect the relevant time and group breakdown where it changes containment.

Now suppose a calendar boundary starts a new reporting window while the failing request path remains impaired. The operation still lacks restoration evidence. Later, the recovery team restores a known working configuration, verifies the previously failing user path and obtains the live observations required by the agreed restart criteria. The responsible service owner can then decide whether to resume discretionary changes. Keep any unresolved causal or recurrence question visible.

The responsible owner uses budget consumption in the stated service policy. Independent safety and acceptance conditions still apply, and recovery work requires qualified people with the appropriate assignment.

### OPS.18:5.3 - The lot decision uses its own plan {#the-lot-decision-uses-its-own-plan}

A separate constructed supplier lot arrives after the process signal above. The supplied product-acceptance plan defines the lot, defects, sampling and disposition authority. For this illustration, it specifies a random sample of fifty items and acceptance only if at most one is nonconforming. Its qualification for the actual product and producer/consumer risks belongs to the supplied plan.

The sample contains two nonconforming items. The acceptance practitioner rejects or segregates the lot as the plan requires and obtains the prescribed rework or supplier response. Even if a process chart for that producer has no current signal, the lot fails this stated acceptance rule.

If the lot had passed, the result would support its disposition under the plan's risks. It would not settle the earlier process investigation. If the plan or its risk qualification is missing for the actual use, obtain that result before relying on this sample rule; these illustrative numbers do not provide a general acceptance plan.

### OPS.18:5.4 - Human service and AI assistance need their actual result {#human-service-and-ai-assistance-need-their-actual-result}

In a hospital operation, the due-request account can show missed service times while clinical priority changes the permissible response. The operating coordinator uses qualified clinical decisions and the current service authority to choose additional cover, rescheduling or another permitted intervention. A low average waiting time cannot clear an individual case whose required condition is unmet.

After an intervention, the coordinator observes the affected service and support work under the selected continuation conditions. A clinical outcome or health-effect claim requires its own evidence. OPS.12 helps preserve human conditions when recovery work adds demand.

In an assisted production service, a monitor may show fewer detected defects after a model change while the current sample excludes difficult requests. Recover that population before interpreting the improvement. Continue or contain the affected use according to the requirement and policy for accepted outputs.

A changed model can also alter the relevant failure modes. Qualification of the current acceptance method, actual accepted results and any affected customer promises may therefore need reconsideration. A passed sample from the earlier version is reusable only for the claims and conditions it still supports.

### OPS.18:5.5 - An unresolved cause need not delay a supported correction {#an-unresolved-cause-need-not-delay-a-supported-correction}

In this constructed print-shop incident, the customer approved proof P2, but the booklets reproduce P1. Records and participant accounts establish that the operator followed the work card containing P1; P2 was unavailable at the station, and the admission check asked only whether a proof was attached. The quality rule requires the affected order to be held.

Trace how P1 reached the station and why P2 was unavailable. Two explanations remain plausible: the preparer copied the earlier attachment, or the station received it from a stale synchronized folder. The records do not distinguish those paths. Both leave the same exposed condition: production can start without checking the proof against the customer's approved edition.

For this case, a qualified proof-control procedure is available for both paths: retrieve the approved proof through the authorized source, check its edition at the station and require first-article acceptance before releasing the order. The responsible production manager has authority and the necessary staff and access to apply it; its effort fits the continuing service commitments. These are supplied premises of the example, not results inferred merely because both explanations sound plausible.

The manager applies that correction. Staff verify that P2 is available, perform the edition check and obtain the required first-article acceptance for restart. Selecting between the copying and synchronization explanations is not a prerequisite to this adequately supported response. Their difference would become relevant if, for example, a proposed automatic retrieval change protected only one path; that proposal would need the missing discrimination or a protection covering both.

OPS.16 addresses any resulting decision to change the recurring operating Method; OPS.17 is needed only for a repertoire choice among competing ways. Completion of the proof-control change is observed separately from recurrence over the later orders and exposure that the prevention claim covers. A clean first article does not establish a long-term recurrence rate.

If the edition check catches P1 before printing, no booklets are spoiled: the check has protected this order. Whether further change is needed depends on the remaining exposure and available protection.

## OPS.18:6 - Bias-Annotation {#bias-annotation}

Visible control limits can look authoritative even when their model or baseline does not fit the operation. Keep the required product or service result beside the monitoring claim and inspect the assumptions before extending its use.

A recent repair can also encourage early closure. Verify restored service at the affected scope, and distinguish that result from identification of the cause and evidence about recurrence. Acknowledging the remaining question allows useful recovery without overstating it.

## OPS.18:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Misuse | Working repair |
| --- | --- |
| Treat statistical stability as product conformity. | Compare output with its requirement and obtain the applicable capability or acceptance result. |
| Use a chart signal as proof of a specific cause. | Contain as required and investigate the actual mechanism. |
| Let an error budget authorize every kind of loss. | Preserve independent safety, human, clinical and acceptance conditions. |
| Accept a lot because the process chart looks normal. | Apply the lot's qualified acceptance plan and risks. |
| Resume normal work when the reporting window resets. | Verify the actual restart conditions and obtain the authorized continuation decision. |
| Reuse an old monitor after the population or failure modes change. | Requalify the affected observation and detection method for the new use. |

## OPS.18:10 - Rationale {#rationale}

Monitoring, acceptance, restoration and prevention regulate different moves. Selecting the evidence from the current decision preserves the meaning of a statistical limit, a product requirement, a service objective and a supported protective change.

The separation between containment, restored service and causal knowledge also supports proportionate action. A practitioner can act on sufficient operating evidence while obtaining the stronger result needed for prevention, wider use or a more consequential commitment.

## OPS.18:11 - SoTA-Echoing {#sota-echoing}

The practice question is how to control operating quality and reliability from evidence suited to the required action. The selected best-known line uses qualified statistical monitoring, user-relevant service indicators and explicit acceptance or recovery criteria. Compared with one aggregate quality status, it exposes the distinct decisions in the worked cases.

| Source and practice question | Selected move and alternative | Operative contribution and limit |
| --- | --- | --- |
| [NIST proportions control charts](https://www.itl.nist.gov/div898/handbook/pmc/section3/pmc332.htm) and [process stability](https://www.itl.nist.gov/div898/handbook/ppc/section4/ppc45.htm) | Use a monitor suited to recurring variation, instead of reacting to every raw fluctuation. | Sections 4.2–4.3 and 5.1 preserve baseline, population and model. The three-sigma example establishes its rule's signal, not an exact risk guarantee. |
| [NIST EWMA guidance](https://www.itl.nist.gov/div898/handbook/pmc/section3/pmc324.htm) | Consider a memory-bearing monitor when persistent small shifts matter more than one large point. | Sections 4.5 and 5.1 retain detection delay and assumptions as reasons to change the method. A new chart requires a suitable design and reference basis. |
| [NIST process capability](https://www.itl.nist.gov/div898/handbook/pmc/section1/pmc16.htm) and [acceptance sampling](https://www.itl.nist.gov/div898/handbook/pmc/section2/pmc21.htm) | Select specification/capability or lot-disposition evidence for that question, instead of reusing a monitoring verdict. | Sections 4.2–4.3 and 5.3 keep the lot, defect and producer/consumer risk basis separate. |
| [SRE service objectives](https://sre.google/workbook/implementing-slos/), [error-budget policy](https://sre.google/workbook/error-budget-policy/) and [alerting on SLOs](https://sre.google/workbook/alerting-on-slos/) | Relate user-relevant observed loss to an agreed action and timely detection, instead of using infrastructure availability alone. | The service case adopts the loss calculation and policy relation. Local targets, exceptions, authority and restart evidence are supplied for the actual service. |
| Ries, *The Lean Startup* (2011), chapter 11; [Lean Enterprise Institute, Five Whys](https://www.lean.org/lexicon-terms/5-whys/); [Google SRE, Postmortem Culture](https://sre.google/sre-book/postmortem-culture/) (2016) | Recover contributing conditions and assign supported prevention, instead of stopping at the first symptom or treating a question count as causal proof. | Sections 4.4 and 5.5 adapt incident reconstruction, knowledgeable participation, countermeasure selection and follow-up. The historical accounts and practice guidance do not prove a particular causal chain or a recurrence reduction; those claims need their own evidence. |

The NIST handbook provides standing technical models; retrieval dates do not make them new methods. The SRE Workbook supplies software-service guidance and a dated 2018 policy example. Their contributions are adapted to the stated operating decisions; broader effectiveness across every service is not established.

For an individual known failure, immediate qualified containment can be the stronger response than developing a new statistical monitor. For recurring uncertain behavior, a designed monitor can reduce reactive disturbance and improve timely detection. Reopen the selected method when the population, baseline, loss consequence, detection need or authorized policy changes.


## OPS.18:End {#end}
