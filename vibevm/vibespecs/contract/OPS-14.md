# OPS.14 - Relate Throughput, Cash, and Operating Consequences {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.14:1 - Problem frame {#problem-frame}

**Use this when** an operating alternative appears worthwhile because it raises output, lowers unit cost, releases capacity or brings money sooner. Examples include buying an extra resource window, changing a service mix, deferring work or automating preparation.

Begin with the actual alternatives and the horizon of the decision. Ask which accepted service, resource use, payments and receipts differ. The first useful result is a comparison that lets the responsible practitioner choose a feasible alternative, make an explicit trade-off or request the missing financial or resource decision.

This pattern governs the operating and financial consequences of a bounded operations choice. Use financial statements, investment appraisals or funding decisions supplied by qualified practitioners when the comparison needs them. If producing one of those results is the main unresolved work, obtain it for the named choice. An operating throughput calculation cannot settle them by itself.

In PumpWorks, completing a third test package now yields positive eventual net cash. Deferring the same package can yield more net cash over the same horizon, and the immediate option can still lack money for its advance payments. The comparison must make all three statements visible.

## OPS.14:2 - Problem {#problem}

A local efficiency measure can hide what the operation gains or loses. More completed attempts may create no accepted output; accepted output may have no paying demand; recognized revenue may arrive before cash; and lower allocated cost per unit may leave every actual payment unchanged.

Comparing only one attractive option compounds the problem. Its positive net cash gives no answer about the alternative, while a short horizon can make delayed receipts disappear from view.

## OPS.14:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| local output and accepted value | A faster resource can create unfinished work, rework or output the recipient does not accept. |
| resource contribution and complete feasibility | A useful contribution-per-hour ranking can fail when jobs are indivisible or several resources are scarce. |
| eventual net cash and funding | A positive result can require payments before the operation has authority or cash to make them. |
| current horizon and later consequences | A short decision window can obscure delayed receipts, commitments and recurring costs. |
| money and other operating conditions | Cash consequences matter within the service, human and quality conditions governing the choice. |

## OPS.14:4 - Solution {#solution}

### OPS.14:4.1 - Name the alternatives and the operating change {#name-the-alternatives-and-the-operating-change}

State the decision, recipient of the comparison, alternatives and horizon. Include current practice or deferral when either is a real option. Establish which alternatives satisfy applicable service, protection and authority conditions; use OPS.12/.13 where those conditions need development.

Describe the operational difference: what accepted result changes, which demand it serves, what work and resources it requires, which work is delayed or displaced, and what happens after failure. Use a schedule or bounded scenarios when timing matters. Keep unresolved assumptions visible.

Follow the proposed gain to its receiving use. Saving preparation time can matter because it changes a payment, frees a resource for another accepted job or protects service. Name the actual consequence before attaching a monetary value to the saved time.

### OPS.14:4.2 - Choose quantities that answer the decision {#choose-quantities-that-answer-the-decision}

Keep the accounting basis with the quantity being compared.

| Quantity | What the practitioner needs to recover |
| --- | --- |
| Physical throughput | The physical output counted, its unit and period, keeping completed service results separate from the attempts needed to obtain them. |
| Monetary throughput or contribution | The selected model of proceeds less specified variable costs, with its cost assumptions and demand basis. |
| Recognized revenue or accounting profit | The accounting period and recognition rules supplied for that purpose. |
| Cash receipts and payments | The amounts that actually enter or leave, their timing, conditions and authority. |
| Released resource capacity | The usable time or capability released and the next service or avoided payment that could use it. |

Choose only the quantities whose difference can change the decision. A throughput-accounting model can be useful for a short-horizon product or service mix when one resource is limiting and its assumptions fit. The common direct-material treatment presumes that other costs remain largely fixed over that horizon. Per-use cloud charges, contracted labor or changed support costs can defeat that presumption.

For a suitable model, compare contribution per unit of the scarce resource together with demand limits. With coupled resources, indivisible jobs, sequencing requirements or binding commitments, obtain the feasible schedule or corresponding optimization result. A ranking alone does not determine the feasible mix.

### OPS.14:4.3 - Build the incremental financial comparison {#build-the-incremental-financial-comparison}

For each alternative, identify future payments and receipts that differ because of the choice. State amount, time and the condition that produces the flow. The same unchanged amount in both alternatives cancels in their difference; keep it elsewhere if the receiving account needs the whole operation's cash position.

Inspect avoidability. A historical payment is not saved by declining future work. An allocated share of rent may remain unchanged, whereas an additional contracted shift or per-use charge can be avoidable. A cost that is fixed this week can become avoidable at a later renewal, so use the decision's actual horizon.

Include displaced use when it is real. Identify the best relevant foregone alternative and its consequence, or state the qualified premise that no material contribution is displaced. Count that loss once. If the cash comparison already includes the missing receipts and avoided costs of displaced work, do not subtract the same foregone contribution again as an extra opportunity cost.

Connect receipts to demand, delivered service, acceptance and payment conditions. Consider the adverse cases that can change the choice: repeat work, delayed acceptance, nonpayment or a lost resource window. A claimed receipt needs its stated basis even when its arithmetic is simple.

### OPS.14:4.4 - Check timing, funding and horizon effects {#check-timing-funding-and-horizon-effects}

Calculate each alternative's net cash within the horizon, then the difference between alternatives. State the direction: completing now minus deferring, for example. Keep this difference distinct from the net cash of either option.

Lay out consequential advance payments and later receipts. Determine whether available authorized funds cover each payment when due, taking prior payments, receipt dates and other obligations on the same funds into account. A favorable final balance can coexist with an earlier funding gap.

Show material flows just outside the horizon and test whether extending it changes the conclusion. A timing advantage can be useful for the receiving cash decision; describe its duration and effect. For longer-lived assets, financing, taxes, discounting or statutory accounting, request the qualified result needed by that use. The simple undiscounted comparison below does not answer those questions.

A fixed annual allocation can be an inadequate description of current need. Refresh the operating forecast and request a resource or funding decision where conditions have changed. A revised forecast itself grants no spending authority.

### OPS.14:4.5 - Return the choice, trade-off or exact missing result {#return-the-choice-trade-off-or-exact-missing-result}

Present the feasible alternatives with the consequential service, resource, human, quality and financial differences. State the assumptions that could reverse the comparison and the observation or decision that would resolve them.

If one alternative is better on the receiving decision's criteria, recommend it with that basis. If earlier service costs more, make the price of that service visible to the authorized decision maker. Preserve mandatory conditions before comparing preferences.

The result can be a short operating account rather than a permanent dashboard. Use OPS.15 when the source events or definitions need repair. After action, compare actual flows and operating results with the assumptions needed for continuation; reopen the affected method or service decision if they change.

## OPS.14:7 - Conformance Checklist {#conformance-checklist}

| Check | Evidence sufficient for the declared use |
| --- | --- |
| The comparison has a real choice. | Alternatives, receiving decision, service result and horizon are explicit. |
| Quantities retain their meaning. | Physical output, contribution, accounting amounts, cash and released capacity have their own units and basis. |
| Operating feasibility is preserved. | Demand, resource windows, human conditions, acceptance, rework and displacement fit each alternative. |
| The incremental account is causal enough for the choice. | Changed payments and receipts follow from stated actions and conditions; unchanged amounts cancel only in the difference. |
| Timing is visible. | Advance payments, receipts, funding gaps and material flows outside the horizon are shown. |
| The result supports the actual decision. | The preference or trade-off, uncertainty, authority gap and reopen condition can be recovered. |

## OPS.14:9 - Consequences {#consequences}

The practitioner can explain why an operating alternative changes service, resources or money and what premise could reverse the choice. A worthwhile release of capacity remains visible even when it does not immediately reduce payments.

The comparison can require information from resource owners, customers or finance. A wider horizon may need a different model. Keeping the account bounded to the live decision reduces unnecessary work while preserving material later consequences.

## OPS.14:12 - Relations {#relations}

OPS.10 helps establish the feasible resource alternatives. OPS.12 supplies a method for comparing human conditions, and OPS.13 guides the commitment and resource decisions that can make an alternative usable. OPS.15 helps construct the operating account where events or definitions need reconciliation.

OPS.18 guides action when quality or reliability changes the expected result or recovery work. OPS.17 helps select a different operating or financial method when the current model's assumptions fail. Qualified finance and accounting practitioners supply the result needed for investment, financing, tax or statutory use.

FPF C.16 preserves comparison characteristics, units and model assumptions; A.10 keeps their evidence reach explicit. A.11.OP limits account detail to what contributes to the decision, required assurance or recovery.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): conditional spec://ai.lev/fpf-eng-ops/contract/OPS-10#root, spec://ai.lev/fpf-eng-ops/contract/OPS-12#root, spec://ai.lev/fpf-eng-ops/contract/OPS-13#root, spec://ai.lev/fpf-eng-ops/contract/OPS-15#root; FPF spec://ai.lev/fpf-spec/contract/C-16#root, spec://ai.lev/fpf-spec/contract/A-10#root, spec://ai.lev/fpf-spec/contract/A-11-OP#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-ma/contract/MA-1#root, spec://ai.lev/fpf-eng-ma/contract/MA-3#root, spec://ai.lev/fpf-eng-ops/contract/OPS-13#root, spec://ai.lev/fpf-eng-ops/contract/OPS-15#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-14
