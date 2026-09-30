# OPS.17 - Compare and Refresh Operations Methods {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.17:1 - Problem frame {#problem-frame}

**Use this when** the current way of running an operation repeatedly misses its purpose, a changed condition defeats one of its assumptions, or a serious alternative could improve a live operating decision. You may need to choose how ready work enters a queue, how an exceptional case continues, or how a service responds to failures.

Start with that decision and one family of Work: the actual work people and other systems perform to produce the operating result. Recover what the present method does, where it fails and what result an alternative must improve. The first useful result is a small repertoire of operating methods with their applicable uses, evidence, costs and reasons to reconsider them. A repertoire is a maintained selection of ways of working, with enough guidance to choose among them.

Operations management is the wider practice. This pattern governs the choice and maintenance of reusable operating methods within it. If an existing method already fits the situation and its conditions still hold, use it for the current decision. Replacing a display, repairing a tool or resolving one unusual case may need only that bounded action. A present comparison or traceable candidate account can be complete while a stronger operating-effect claim remains unsupported. Developing or testing that claim is separate work, selected only when its attainable contribution is worth the whole burden.

A PumpWorks board contains twelve matters, yet only four test packages are ready for the rig. Buying more rig time, restricting work in progress and repairing readiness can all sound like remedies. Their value depends on why work waits. Comparing their operating moves makes that question answerable before the team commits to a school or tool.

## OPS.17:2 - Problem {#problem}

A named approach often bundles useful operations with assumptions about demand, resources, evidence and the purpose of the organization. Adopting the bundle can import an unsuitable objective or omit a condition that made its source example work. A local success also gives weak grounds for general use if the team cannot recover what was actually changed.

A catalogue creates a different difficulty: it preserves names but leaves every practitioner to reconstruct applicability. The needed knowledge is what each method lets the operation do, what it requires, and what observable change would defeat the claim.

## OPS.17:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| reuse and fit | A known method saves invention, while local demand, authority or capability can invalidate its assumptions. |
| improvement and adoption cost | A stronger response can consume training, observation and coordination effort that a simpler adequate response avoids. |
| local gain and operating result | Faster preparation can move unfinished work to acceptance or consume incident cover elsewhere. |
| comparison and preference | Several feasible methods can remain worthwhile for different service, burden and financial consequences. |
| consistency and exception | A stable work policy helps coordination; a justified urgent exception can require explicit displacement and recovery. |

## OPS.17:4 - Solution {#solution}

### OPS.17:4.1 - Frame the choice in operating terms {#frame-the-choice-in-operating-terms}

Name the Work family, the result served, the receiving decision and its horizon. Describe the current method through a recent representative case: what triggered action, what inputs and resources were used, what people did, what result was accepted and where work or information waited. Use existing evidence first.

State the consequential discrepancy. “The board has twelve cards” is an observation. “Four ready packages cannot receive their required two-hour rig visits before Friday” names a service problem. If the mechanism is unresolved, state how that uncertainty affects the current choice. OPS.9 helps with a disputed constraint; OPS.15 helps when the existing account cannot make the distinction.

Keep current practice and the least costly adequate response in the comparison. A corrected readiness check may be enough when a wholesale planning change offers no further decision-relevant benefit.

### OPS.17:4.2 - Recover candidate operations from their sources {#recover-candidate-operations-from-their-sources}

Read each candidate at the level that could actually be reused. Recover its input, sequence or conditional rules, first useful result, required capability and support, evidence for the claimed effect, and conditions for stopping or changing its use. Retain the source and its relevant version or date when that changes the meaning.

For example, an explicit limit on started work requires a start/end definition and a policy for reaching the limit. A rule protecting a scarce resource requires evidence of the resource's limiting role for the named demand and horizon. A case method requires conditions under which a practitioner may choose or change the next action. These are different claims even when one tool presents them together.

The following repertoire supplies starting comparisons. Select only the row needed by the operating question.

| Operating question | Candidate move | Evidence and limit that change its use |
| --- | --- | --- |
| Too much work starts while eligible work waits | Define readiness, control work in progress and pull new work when the stated capacity is available, using the Kanban line. | Recover item boundaries, actual waiting and the start policy. A limit must protect the receiving service; its value is not inferred from the number of board cards. |
| A particular resource or dependency limits the result | Protect its useful time and feed it appropriately, using bounded moves from the Theory of Constraints (TOC) and TameFlow. | Establish the current limiting mechanism. Historical average utilization alone can miss starvation or short peak overloads. |
| New information changes an admitted case | Choose or revise the next action under case conditions, using CMMN case planning or declarative condition/response rules. | Recover prerequisites, pending obligations and practitioner discretion. A recurring subprocedure can remain fixed inside the case. |
| A customer-relevant service objective is missed | Relate eligible service events, observed loss and an authorized response through a service-level objective (SLO) and an error-budget policy that connects permitted loss to action. | Check event coverage and response timing. An aggregate can hide a severe short incident or an affected customer group. |
| Repeated production results change or a lot needs disposition | Use statistical monitoring for variation, or an acceptance plan for the particular lot. | The population, sampling basis and decision differ. A monitoring signal does not supply a lot-disposition decision. |
| More output appears financially worthwhile | Compare contribution per scarce resource under a suitable model, and compare actual incremental payments and receipts over the decision horizon. | Recover demand, variable costs, displacement, acceptance and timing. Coupled constraints and indivisible jobs can defeat a simple ranking. |
| Extra service consumes human recovery or attention | Remove avoidable demand, redesign the work pattern or provide qualified coverage before relying on individual coping. | Recover affected groups and supplied protection conditions. Use OPS.12 to choose the intervention. |

A source's example is evidence for what it demonstrates. Treat a proposed combination as a candidate whose compatibility and fit still need examination. A tool's changed version is a reason to inspect its effect on the method, rather than sufficient evidence of a new Method variant.

### OPS.17:4.3 - Compare feasible ways of working {#compare-feasible-ways-of-working}

First exclude options that violate a supplied protection, authority limit or necessary operating condition. For the remaining options, compare the consequences that could change the decision: accepted service, resource demand, delay, quality, human burden, financial effect and the effort to introduce and sustain the method.

Use the same Work family, horizon and result definition for each option. Carry uncertainty as an interval, scenario or unresolved claim suitable for the use. Separate an observed result from a forecast or causal explanation. A method that worked in one team may still be a useful candidate elsewhere; the evidence for that receiving use must remain visible.

An option is dominated when another feasible option is at least as good on all consequential comparison characteristics and better on at least one, under the stated comparison. Keep non-dominated options when the preference remains unresolved. The authorized decision maker can choose among them by an explicit priority or justified trade-off. For example, earlier service may justify a higher payment; a weighted score cannot make a breached recovery condition acceptable.

Increase comparison effort only where it can change the choice. If every proposed option depends on the same unresolved mandatory staffing condition, obtain that missing result before refining their service scores.

### OPS.17:4.4 - Compose compatible moves and state the usable result {#compose-compatible-moves-and-state-the-usable-result}

Several moves can serve one operation. Readiness-based admission can coexist with case discretion and a reliability stop rule. Check the shared subject and the points at which one rule changes another rule's permission, priority, resource use or stopping condition.

Resolve a consequential conflict before using the combination. An urgent incident may override a WIP policy under an existing service authority. The exception needs the displaced work, remaining protected conditions and recovery action to be clear. A general “urgent” label cannot supply those facts.

Return the selected use and the actual level of support: an applicable established method, a conditional alternative, a traceable candidate account with an unresolved operating claim, or an unsuitable use with its reason. On the available basis, the repertoire can retain current practice, keep or revise a candidate account, or reject a proposed use. Preserve the gap needed by a later stronger use in that same return. Keep any selected first action, its conditions and evidence limits, burden and reason to reopen close to the consequential choice. An existing operating note or method description can hold this result; maintaining a second catalogue adds value only if someone uses it to choose work.

### OPS.17:4.5 - Refresh the affected method claim {#refresh-the-affected-method-claim}

Reconsider a method when a relied-on condition changes, its operating result deteriorates, or a credible alternative changes the comparison. Locate the failed claim before replacing the whole repertoire. A change in customer acceptance can affect a service forecast while leaving readiness checks useful.

Use ME.15 when the reusable semantics change: inputs, operations, applicability or result may define a Method variant. Keep changes to the description, supporting tool and one local departure distinguishable. Preserve evidence only for the claims and conditions it still supports. A combination of previously admitted methods needs its own evidence where their interaction changes the claimed result.

Use the available qualified evidence, estimates and judgement to complete the comparison needed by the decision maker, or to document the proposed method's origins and unresolved claims. Retain the adequate incumbent or bounded candidate account with its actual gap when no further inquiry can make a worthwhile attainable contribution. Use ME.7 for the status of a proposed whole and ME.14 for its practical worth. Maintaining an account or choosing a repertoire supplies no additional Method admission, compatibility, empirical fit or transfer evidence, or permission for operating use.

When an unresolved operating effect could change the decision, compare the attainable contribution of a new trial question or evidence acquisition with its whole burden: design, performance, interpretation, delay and displaced operating Work. Select it only when that contribution is obtainable and worth the burden. For a selected trial, return the effect to observe, protected conditions, authority, stop and comparison basis. When the question concerns competing explanations, include the observation that could distinguish them. ME.11 can guide that trial. The repertoire choice itself establishes neither that the candidate was performed nor that it improved service.

## OPS.17:7 - Conformance Checklist {#conformance-checklist}

| Check | Evidence sufficient for the declared use |
| --- | --- |
| The choice has a working purpose. | The Work family, receiving decision, discrepancy and horizon can be recovered. |
| Candidate content is actionable. | Inputs, operating moves, first result, needed capability/support and source limits are clear. |
| The comparison preserves feasibility and preference. | Protected conditions are checked before trade-offs; consequential differences and unresolved preferences remain visible. |
| Composition is usable. | Shared conditions, exceptions, displacement and stops are compatible for the selected use. |
| The returned claim has appropriate support. | Supported uses, current candidate accounts, actual evidence gaps and any selected worthwhile attainable trial are distinguished. |
| Refresh can be directed. | A changed condition can be traced to the affected method claim and its receiving decision. |

## OPS.17:9 - Consequences {#consequences}

Practitioners can reuse a bounded operating move without importing a whole school's objective or record system. The repertoire also makes changed conditions easier to address: the team can revise one admission rule or acceptance assumption while retaining useful neighboring methods.

The comparison takes effort, and some effect claims remain uncertain until local use. Maintaining only decision-relevant alternatives and finishing the supported comparison limits that cost. Further inquiry is selected for the contribution it can make at its full cost. Broader comparative effectiveness remains an empirical question.

## OPS.17:12 - Relations {#relations}

OPS.5, OPS.6, OPS.8 and OPS.9 supply the concrete admission, continuation, queue and constraint questions for which a repertoire entry can be selected. OPS.12–OPS.15 and OPS.18 supply human-condition, service, financial, account and control results needed by particular comparisons. Their use follows the live question.

ME.15 guides maintenance of Method variants and the evidence they can reuse. ME.11 supplies a trial method for a selected worthwhile and attainable local comparison; ME.13 and ME.14 address fit and worth where those judgments are required. The full operating-Method-change question of OPS.16 and cultural continuation question of OPS.20 remain distinct from maintaining this repertoire.

FPF A.3.1/A.3.2 distinguish performed Work, a Method and its description when the comparison relies on those claims. C.16 and G.5 support meaningful comparison characteristics and selection among alternatives. A.11.OP limits additional collection or apparatus to what contributes to the decision, needed assurance or recovery.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-me/contract/ME-15#root; conditional spec://ai.lev/fpf-eng-ops/contract/OPS-5#root–spec://ai.lev/fpf-eng-ops/contract/OPS-15#root, spec://ai.lev/fpf-eng-ops/contract/OPS-18#root, spec://ai.lev/fpf-eng-me/contract/ME-11#root, spec://ai.lev/fpf-eng-me/contract/ME-13#root, spec://ai.lev/fpf-eng-me/contract/ME-14#root; FPF spec://ai.lev/fpf-spec/contract/A-3-1#root, spec://ai.lev/fpf-spec/contract/A-3-2#root, spec://ai.lev/fpf-spec/contract/C-16#root, spec://ai.lev/fpf-spec/contract/G-5#root, spec://ai.lev/fpf-spec/contract/A-11-OP#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-ops/contract/OPS-18#root, spec://ai.lev/fpf-eng-ops/contract/OPS-19#root, spec://ai.lev/fpf-eng-ops/contract/OPS-20#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-17
