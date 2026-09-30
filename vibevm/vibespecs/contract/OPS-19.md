# OPS.19 - Reconcile Simultaneous Operating Work Across Cases and Scales {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.19:0 - Use This When {#use-this-when}

Use this Method when several kinds of operating Work are present together and a locally sensible choice can harm another case or service, worsen an operating result, or move a result into a horizon where its consequence changes. Typical moments include keeping a busy resource utilized while incident coverage is thinning, completing one case sooner by moving delay to a shared acceptance queue, or starting improvement Work while current commitments and human recovery still need protection.

The first useful result is a short cross-scale operating account and decision. It names the local choice, the simultaneous Work and structures that can reverse it, the conflicting results and measures on their own subjects, feasible alternatives, authority and protection conditions, the selected reconfiguration or bounded continuation, and the condition that reopens the decision. It may instead return one exact unresolved conflict when a necessary result or authority is missing.

Start here only when the decision genuinely crosses subjects, operating scopes, or time horizons. Use `OPS.8` for one queue-policy question, `OPS.9` for one current-constraint question, `OPS.10` for one capacity-and-service comparison, and `OPS.11` for one interacting-structure coordination question that those patterns can settle directly. Use current `ME.6` when the primary question is comparison of Method or candidate-account co-use rather than reconfiguration of continuing operating Work. Use `OPS.16` when the current object is one operating Method change, and `OPS.20` when the current claim concerns continuation or change of enacted practice in a practitioner population.

## OPS.19:1 - Problem frame {#problem-frame}

Continuing operation brings several Work wholes and decision structures together. Customer or patient cases progress while shifts provide service, queues and constraints are coordinated, incidents or recovery Work consume margin, financial-control Work changes the feasible horizon, and Method-improvement Work may be planned or performed. These wholes can overlap without becoming parts of one master process.

A local measure sees only its own subject and scale. Rig utilization can rise while case completion, cash timing, incident resilience, or participant recovery worsens. Faster case admission can overload inspection or release. A change programme can meet its milestone while the continuing service loses a protected condition.

Here *scale* means the subject, operating scope, or time horizon on which a result is claimed. It does not imply a universal hierarchy of team, department, organization, or enterprise levels. The Method selects only the scales and relations that can change the current operating choice.

## OPS.19:2 - Problem {#problem}

Operations teams often receive several correct local accounts that recommend incompatible actions. A queue report says start now, a capacity account retains a recovery reserve, a service account says hold, a financial comparison favors deferral, and an improvement plan needs the same specialist. Combining the numbers into one dashboard does not reconcile their subjects, horizons, evidence, or authority.

The opposite failure is an exhaustive enterprise model. It can describe many structures while leaving the practitioner unable to decide what to start, hold, reconfigure, or return. The practical need is a bounded decision that preserves each material result, exposes moved burden, and stops when an indispensable premise is missing.

## OPS.19:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| local action and wider consequence | A narrow choice is easy to execute, while its delay, risk, cash need, or burden may appear elsewhere. |
| immediate completion and retained resilience | More Work can start now only by consuming recovery, incident, or acceptance margin needed later. |
| unlike results and one decision | Service, cash, quality, human recovery, throughput, and evidence can all matter without one defensible common score. |
| simultaneous Work and sequence | Some Work has real order; other Work overlaps or remains a separate whole. One sequence can hide the conflict. |
| coordination and distributed authority | One operating decision needs several inputs, while clinical, safety, financial, service, and employment authority do not merge. |
| enough structure and timely action | Omitting a material relation makes the choice unsafe; mapping every relation delays the useful result. |
| current evidence and changing conditions | A sound decision can become false when access, demand, commitments, support, or the evidence window changes. |

## OPS.19:4 - Solution {#solution}

Build the smallest truthful account that lets the authorized operating decision preserve simultaneous Work and its material consequences. Begin with the exposed local choice, recover only decision-changing structures and results, construct materially different alternatives, and return a reconfiguration, bounded continuation, or exact unresolved conflict.

### OPS.19:4.1 - Fix the operating question and exposed local choice {#fix-the-operating-question-and-exposed-local-choice}

Name the operating System, the useful result or service that must continue, the receiving decision, the current horizon, and the exact local choice that exposed the conflict. State the local measure or reason supporting that choice and the consequence that could defeat it.

Examples are: start a third package to keep a rig utilized; release more cases into a diagnostic queue; extend a shift to clear backlog; defer inspection to protect a shipping date; or open a Method trial while incident coverage is reduced.

Reuse a current `OPS.1` operating focus and `OPS.3` subject account when they are available. If the subject, commitment, or decision cannot be identified, return that missing basis before comparing alternatives. If no result outside the local choice can reverse it, use the direct local pattern and stop.

### OPS.19:4.2 - Recover the simultaneous Work without forcing one whole {#recover-the-simultaneous-work-without-forcing-one-whole}

Identify the actual or intended Work whose relations matter to the decision. Check case Work, shift or continuing-service Work, queue or constraint coordination, incident and recovery Work, financial-control Work, and Method-improvement Work only when each can change the choice.

For actual Work, preserve each independently supported Work whole and identify any supported parts or episodes separately. Record precedence, succession, or overlap only as relations among the identified Work. For intended Work, keep the `WorkPlan` and its conditions distinct from performed Work. Shared performers, timestamps, resources, labels, or diagrams do not establish parthood.

An admission–processing–inspection–delivery order can be real for one case while service coordination and improvement Work overlap it as separate wholes. Record both facts. Do not turn all concurrent activity into one process or all ordered activity into organization levels.

### OPS.19:4.3 - Select the structures that can reverse the choice {#select-the-structures-that-can-reverse-the-choice}

Select only the subjects, Work, Methods, resources, commitments, accounts, authority relations, and descriptions that can change the decision. Recover the exact obtaining relation or supported claim used from each structure.

Keep every process diagram, board, event log, financial model, and dashboard separate from what it represents. State what the representation preserves, what it omits, and which current decision uses it. Use `C.32.MWA` when a general synthesis across non-isomorphic practice structures is needed; its result is architecture evidence, not the operating decision returned here.

A compact working account can use these positions:

| Position | What to record |
| --- | --- |
| local choice | the proposed start, hold, sequence, allocation, or policy and the local reason for it |
| simultaneous Work | the independently identified Work wholes and only the part, order, episode, or overlap relations used by the choice |
| decision-changing structures | the cases, queues, constraints, resources, commitments, accounts, authority, and descriptions whose relations can reverse the choice |
| conflicting results | each result or measure with its subject, scale, horizon, evidence, and protected condition |
| alternatives | materially different feasible arrangements, including bounded continuation and a truthful stop |
| return | authorized decision or exact unresolved conflict, together with its conditions and reopen trigger |

This table is a writing aid, not a new operating record type.

### OPS.19:4.4 - Keep results and measures on their own subjects {#keep-results-and-measures-on-their-own-subjects}

State each decision-relevant result on the subject and scale it actually concerns. Case completion, total flow, service, current-constraint protection, resilience, cash, participant recovery, quality, and improvement evidence do not become one result because they appear on the same dashboard.

For every relied-on measure or claim, name its subject, scheme or interpretation, time window, evidence basis, and receiving use. Distinguish a direct observation from an association, contribution claim, forecast, or causal claim. Keep an unavailable result as a gap rather than filling it with a nearby proxy.

Use `OPS.12` for human-condition evidence, `OPS.14` for operating and financial consequences, `OPS.15` for a decision-specific account, and `OPS.18` for a quality or reliability control decision when their questions are current. Their results constrain this choice; they retain their own subjects and authority.

### OPS.19:4.5 - Construct materially different operating alternatives {#construct-materially-different-operating-alternatives}

Compare the current arrangement with at least one alternative that changes the decision. Include bounded continuation, reconfiguration, defer or hold, and stop only where each is feasible and materially different. Do not rename the same arrangement or vary only its presentation.

For every alternative, expose where it moves delay, burden, evidence risk, cash need, service exposure, quality risk, or recovery cost. Ask which participant or operating scope receives that moved consequence and whether the required condition or authority is current there.

Preserve protected conditions before seeking a local gain. An alternative that requires unavailable access, unsupported overtime, missing clinical authority, consumed incident margin, or evidence from the wrong configuration is not yet feasible. Return the exact missing result instead of treating the alternative as available.

### OPS.19:4.6 - Apply authority, commitment, evidence, and currentness conditions {#apply-authority-commitment-evidence-and-currentness-conditions}

Identify which operating policies can change within current authority and which decisions belong to another holder. Recover commitments, permissions, protection conditions, evidence windows, and stop rules that the selected alternative relies on.

Use `C.11` for the bounded choice when the chooser, option set, rule, evidence, and authority are present. A coordination proposal, model optimum, or majority preference does not supply missing authority. A clinical, safety, legal, financial, employment, or release result remains with its professional owner.

When a required result is unavailable, decide only what can proceed without it and return the blocked remainder. A partial operating decision plus one exact missing input is preferable to a complete-looking but unauthorized reconfiguration.

### OPS.19:4.7 - Return the cross-scale operating decision {#return-the-cross-scale-operating-decision}

Return one of three useful results:

1. **Cross-scale reconfiguration.** Change which Work starts or is held, or change allocation, sequence, support, or another operating relation so the material results can coexist under current authority and conditions.
2. **Bounded continuation.** Keep the current arrangement for a named scope and interval because changing it would consume a protected condition or lacks a better supported alternative.
3. **Exact unresolved conflict.** Name the incompatible results, missing evidence or authority, what can still proceed, and the result that must return before the decision can close.

Record the decision, conditions, protected consequences, deferred demand, responsible return, and reopen trigger. Do not infer implementation, later effectiveness, a changed Method, or cultural continuation from the decision.

Send the result to `OPS.16` only when it changes a feasible Method trial or protected trial condition. Send it to `OPS.20` only as a candidate practice variation or consequence; that Method independently supports its population, predicate and continuation decision. Any selected intervention, needed authority or claimed later observation keeps its own basis.

### OPS.19:4.8 - Keep the result short enough to use {#keep-the-result-short-enough-to-use}

The practitioner should be able to state the conflict, alternatives, decision, and reopen condition in a brief account. Add structural detail only when it changes feasibility, consequence, authority, or evidence reach.

Recognition is the ability to spot when a local operating choice is exporting harm or consuming another scope's protected condition. Assurance requires supported Work and relation claims, qualified consequences, current authority, and explicit evidence limits. A larger model, more measures, or a cleaner diagram supplies none of those by itself.

What changes in practice: the operator stops asking which local measure should win and instead records which simultaneous results can reverse the choice, compares feasible arrangements, protects current conditions, and returns one authorized action or exact unresolved conflict.

## OPS.19:7 - Conformance Checklist {#conformance-checklist}

1. Is the operating System, useful result, receiving decision, horizon, and exposed local choice clear?
2. Are the simultaneous Work wholes and only their supported part, episode, order, or overlap relations identified?
3. Are actual Work, intended Work, Methods, subjects, structures, descriptions, and records kept distinct?
4. Does every selected structure or relation have a decision-changing use?
5. Are results and measures stated on their own subjects, scales, horizons, schemes, and evidence bases?
6. Do the alternatives differ materially and expose moved delay, burden, evidence risk, cash, service exposure, quality risk, or recovery cost?
7. Are protected conditions, commitments, authority, and currentness checked before an alternative is called feasible?
8. Does the return clearly state reconfiguration, bounded continuation, or exact unresolved conflict?
9. Are downstream Method-trial and cultural questions left to `OPS.16` and `OPS.20` under their own entry conditions?
10. Can a cold practitioner state what changes now and what reopens the decision without reconstructing an enterprise model?

Recognition passes when the practitioner can produce the short cross-scale account and distinguish the material conflict. Assurance requires the obtaining relations, evidence reach, protection conditions, and authority used by the selected decision.

## OPS.19:9 - Consequences {#consequences}

The operation gains a decision that can preserve current cases, service, resilience, cash, human recovery, quality, and improvement conditions without pretending they are one measure. A bounded hold or exact missing return becomes an actionable result rather than evidence of weak coordination.

The cost is explicit recovery of several subjects, relations, evidence windows, and authority conditions. Some decisions remain partial. This cost is proportionate when the selected structures can reverse the choice; detail that cannot do so stays with its direct owner.

## OPS.19:12 - Relations {#relations}

- **Receives from:** `OPS.1` and `OPS.3` for the operating System, commitments, subjects, cases, resources, records, and relation candidates; reidentify any subject or boundary whose current facts no longer support the earlier result.
- **Receives from:** `OPS.11`, `OPS.12`, `OPS.15`, and `OPS.17` for interacting-structure evidence, human-condition consequences, a decision-specific account, and applicable status-preserved Method or repertoire claims. An absent or stale result stays an exact gap.
- **Coordinates with:** `OPS.8`–`OPS.10`, `OPS.13`, `OPS.14`, and `OPS.18` when queue, constraint, capacity, commitment, operating-financial, quality, or reliability results can reverse the choice; each pattern retains its own subject and result.
- **Uses:** current `C.32.MWA` for general several-structure architecture evidence, `C.11` for a bounded choice when its conditions obtain, and the current FPF Work, structure, evidence, measurement, temporal, causal-use, and representation owners for the exact claims relied on here. None supplies the Operations reconfiguration or its domain authority.
- **Provides to:** `OPS.16` only where the cross-scale decision changes the feasible Method trial or protected conditions. The receiving trial independently establishes its subject status, evidence, alternatives, authority, and available return.
- **Provides to:** `OPS.20` only as a candidate practice variation or operating consequence. The cultural Method independently supports its bounded population, predicate and continuation decision; an intervention, needed authority or claimed later observation has its own basis.
- **Does not replace:** clinical, safety, legal, financial, employment, software-assurance, release, product, organization, capability, or cultural decisions owned by their direct practices.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-1#root, spec://ai.lev/fpf-eng-ops/contract/OPS-3#root; conditional spec://ai.lev/fpf-eng-ops/contract/OPS-11#root, spec://ai.lev/fpf-eng-ops/contract/OPS-12#root, spec://ai.lev/fpf-eng-ops/contract/OPS-15#root, spec://ai.lev/fpf-eng-ops/contract/OPS-17#root; FPF spec://ai.lev/fpf-spec/contract/C-32-MWA#root, spec://ai.lev/fpf-spec/contract/C-11#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-oce/contract/OCE-11#root, spec://ai.lev/fpf-eng-ops/contract/OPS-11-1#root, spec://ai.lev/fpf-eng-ops/contract/OPS-16#root, spec://ai.lev/fpf-eng-ops/contract/OPS-20#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-19
