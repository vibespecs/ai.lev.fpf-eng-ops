# OPS.14 - Relate Throughput, Cash, and Operating Consequences: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.14:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.14:5.1 - PumpWorks compares the same third package on one horizon {#pumpworks-compares-the-same-third-package-on-one-horizon}

This constructed comparison runs from the start of month 1 through the end of month 2. Four test packages are ready. Each needs two rig-hours. In the supplied adverse case, one of the two packages retained in both alternatives needs one immediately available two-hour repeat and then passes. The third package passes first time in either alternative.

The two retained packages have the same costs and receipts in both alternatives, so they cancel in this incremental comparison. Their work uses the current six-hour window, including the repeat. The decision concerns when to complete the third package.

The customer permits either date below. It pays 900 currency units at the end of month 2 if the third package's evidence meets the stated test-service acceptance criteria by day 20 of that month. Laboratory permission is supplied. Customer acceptance of this test service has its own scope; R42's field release still requires applicable T9 evidence, S19's safety result and release authority.

| Alternative | Work and acceptance | Payments that differ | Receipt | Net cash through month 2 |
| --- | --- | --- | --- | --- |
| Complete now. | Extend from six to eight rig-hours in month 1; complete the two retained packages, their repeat and the third package. The third package's evidence is accepted in month 1. | Pay 300 for extra rig access, 400 for qualified relief and 100 for consumables before the extra work in month 1: 800 total. | Receive 900 at the end of month 2. | 900 − 800 = +100. |
| Defer the third package. | Complete the two retained packages and repeat in the six-hour window. Use a confirmed two-hour spare slot on day 10 of month 2 for the third package; its evidence is accepted by day 20. | Pay 100 for consumables before the deferred test. The supplied resource account confirms that already-paid rig/staff arrangements stay unchanged and the spare slot displaces no accepted job or other foregone contribution. | Receive 900 at the end of month 2. | 900 − 100 = +800. |

Completing now minus deferring gives +100 − (+800) = **−700 currency units** over the stated horizon. Earlier test service costs 700 more under these assumptions. The financial comparison favors deferral; the responsible practitioner may still value earlier service enough to justify that cost if the governing conditions allow the choice.

The immediate option needs 800 before any receipt. Only 500 is currently available under the supplied cash allowance, so this option has a **300 funding gap**. Its eventual +100 net cash does not fill that earlier gap. The practitioner must obtain the additional authorized funding or choose a funded alternative. The deferred option still requires its 100 payment when due.

Qualified relief preserves the original operator's recovery and incident coverage in the proposed extension. Its 400 payment is part of making that alternative feasible. The resource owner's access and displaced-use decision is also required. Paying the fee cannot supply either the staffing result or permission to release the product.

### OPS.14:5.2 - A moved receipt changes the short-horizon result {#a-moved-receipt-changes-the-short-horizon-result}

Now suppose the deferred package misses the month-2 acceptance cutoff and its 900 receipt moves to month 3. Keep every other fact the same.

| Comparison horizon | Complete now | Defer with month-3 receipt | Now minus defer |
| --- | --- | --- | --- |
| Start of month 1 through end of month 2 | +100 | −100 | +200 |
| Start of month 1 through end of month 3 | +100 | +800 | −700 |

The +200 difference is a cash-timing advantage inside the shorter horizon. The account shows the excluded 900 receipt and the cost of completing earlier. Extending the horizon reveals the original −700 difference; no lasting gain was created by ending the account sooner.

If the immediate package instead misses acceptance or payment, its 900 receipt also moves or disappears while the spent 800 remains. The practitioner therefore checks the acceptance and payment premise for both alternatives. A new failure or financing consequence requires a changed comparison rather than reuse of these totals.

### OPS.14:5.3 - One resource can still require a discrete choice {#one-resource-can-still-require-a-discrete-choice}

Suppose two indivisible jobs compete for three usable machine-hours. Under the stated contribution model, job A yields 70 currency units and needs two hours; job B yields 100 and needs three. Demand exists for one of each, both are otherwise feasible, and partial jobs have no accepted result.

A has the higher ratio: 35 per hour versus approximately 33.33. Choosing A leaves one unusable hour and yields 70. Choosing B yields 100. The feasible alternatives, not the ratio order alone, settle this decision.

With several scarce resources or service obligations, the practitioner uses the appropriate scheduling or optimization method. This small example establishes the effect of indivisibility; it supplies no general optimal scheduling algorithm.

### OPS.14:5.4 - Hospital and assisted-service choices retain their purpose {#hospital-and-assisted-service-choices-retain-their-purpose}

A hospital can compare the payments required for two qualified staffing arrangements after the responsible practitioners establish clinical priority, care requirements and protected conditions. If one arrangement violates a required condition, a lower payment cannot make it feasible. If both satisfy the service, their resource and financial consequences can inform the operating choice. The comparison supports the hospital's stated service purpose.

Consider one constructed working day with four accepted outputs due. Both options produce sixty charged drafts for the same demand under unchanged human and acceptance conditions; the salaried team completes six individual review decisions. All payments use the same currency.

| Generator | Generation payment | Additional rework payment | Accepted / rejected after six reviews |
| --- | --- | --- | --- |
| Current | 60 at 1 per draft | 0 | 4 / 2 |
| Alternative | 30 at 0.5 per draft | 10 | 2 / 4 |

Both leave fifty-four drafts unreviewed; rejected work and the paid rework remain unaccepted. The same 240 salary is paid today, with no other payment or receipt. Total payments are 300 versus 280: the alternative saves 20 cash, while payments per output accepted that day rise from 75 to 140. These are daily payment ratios; they do not close the unfinished work. The unchanged salary yields no cash saving, and qualified review capacity remains six decisions per day. Retain the current arrangement for the four due outputs under confirmed funding and decision authority; qualify any later generator or service change before relying on it.

## OPS.14:6 - Bias-Annotation {#bias-annotation}

An attractive option is easier to defend when its comparator is absent. Describe the same service result, horizon and changed flows for every serious alternative, including deferral where it is real.

A budget category or unit-cost display can also dominate attention because it is already reported. Recover the amount that actually changes and the authority needed to act. Show a material delayed receipt even when it lies outside the chosen reporting window.

## OPS.14:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Misuse | Working repair |
| --- | --- |
| Recommend an option because its own net cash is positive. | Calculate the same result for the actual alternatives over a common horizon. |
| Call reduced allocated cost an avoidable payment. | Recover what payment changes, when it changes and why. |
| Rank indivisible jobs only by contribution per hour. | Compare feasible whole-job combinations or obtain the needed scheduling result. |
| Subtract displaced contribution twice. | Trace whether the lost receipts and avoided costs already appear in the comparison. |
| Use an eventual receipt to justify an unfunded advance payment. | Identify the amount and authority required before work starts. |
| Treat a receipt outside the horizon as permanently lost. | Show its expected date and test a horizon adequate to the receiving decision. |

## OPS.14:10 - Rationale {#rationale}

Accepted operating results, accounting recognition and cash occur through different events and rules. Following the actual consequences between them prevents a local production measure from standing in for the receiving financial decision.

Comparing alternatives on one basis makes an incremental claim intelligible. Separating final net cash from timing and funding then preserves the conditions under which the chosen work can actually begin.

## OPS.14:11 - SoTA-Echoing {#sota-echoing}

The practice question is how to choose operating work when output, scarce resources and financial timing interact. The selected strongest line uses relevant future differences between feasible alternatives, with a constrained-throughput model only where its assumptions fit. Compared with a single unit-cost or utilization figure, this line explains both PumpWorks' cheaper deferred service and the immediate funding gap.

[ACCA's treatment of relevant costs](https://www.accaglobal.com/my/en/student/exam-support-resources/fundamentals-exams-study-resources/f5/technical-articles/relevant-costs.html) supplies the future incremental cash and opportunity-cost reasoning used in sections 4.3–4.4. PumpWorks adapts that reasoning to explicit acceptance dates and two alternatives. The instructional model does not supply tax, financing permission, discounting or statutory recognition rules.

[ACCA's throughput-accounting treatment](https://www.accaglobal.com/gb/en/student/exam-support-resources/fundamentals-exams-study-resources/f5/technical-articles/throughput-constraints2.html) contributes the scarce-resource mix question under short-horizon cost assumptions. Section 4.2 retains the useful contribution comparison while the whole-job case shows a limit of using the ratio as a decision rule. Variable cloud or labor payments require the actual cost model.

The [Beyond Budgeting principles](https://www.afponline.org/docs/librariesprovider7/default-document-library/bb-principles-handout-2020-%281%29.pdf?sfvrsn=157d3a6b_2), in a 2020-named handout citing Hope, Bunce and Röösli's 2011 work, support resource decisions responsive to current need. Section 4.4 adapts that move when a fixed allocation no longer describes the operating situation. It preserves the separate funding decision; a refreshed forecast is not authorization. The source is practitioner guidance, not proof that every operation benefits from the whole management model.

For a money-bearing choice with significant long-term or financing effects, a qualified investment or financial model is the stronger alternative to this simple account. Use it when those consequences can change the decision. Reopen the comparison when demand, avoidability, acceptance, displacement, funding or horizon changes.


## OPS.14:End {#end}
