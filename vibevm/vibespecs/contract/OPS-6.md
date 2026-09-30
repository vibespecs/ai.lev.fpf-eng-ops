# OPS.6 - Continue Cases and Handle Exceptions {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.6:0 - Use This When {#use-this-when}

Use this pattern during one admitted continuing case when current facts, an exception, or a changed condition makes the standard next action uncertain. Typical cues are “the normal route no longer fits”, “the ticket moved but nothing changed”, “the model recommends a fix”, “we are waiting for one more result”, or “who may act now?” while the case subject, permission, performer, evidence, and next permissible Work are unclear.

The first useful result has one of two forms:

> **Progression:** for case subject `S` in qualified state `Q` at configuration and horizon `H`, matching permission `P` and domain Method `M` support next Work `W` by responsible performer `R`, with stop or fallback `F` and expected evidence `E`; after independently supported performance, report the progressed state `Q'` and its evidence to the participant responsible for the next operating decision under return conditions `N`.
>
> **Blocker:** condition `K` is missing, stale, contradicted, unauthorized, unsafe, unsupported, or unavailable; owner or source `O` must supply the bounded result; safe fallback or stop is `F`; retry when `T` obtains.

Recognition is cheap: enter when participants cannot choose or execute the next permissible Work in an admitted case from the current facts. Assurance is stronger: selected action, permission, responsible performer, actual Work, resulting evidence, and progressed case state each require separate support.

Do not use OPS.6 to design one universal workflow or case lifecycle, reconstruct a reusable Method from event data, infer progress from a ticket, plan, model, trace, or record update, or revise priority merely because the case is old. Use `A.15.7` for the general situation-responsive next-action Method, `A.3.1.MR` when reusable Method recovery from several performances is the actual question, and `OPS.7` when temporal or consequence evidence can change priority or an existing commitment.

## OPS.6:0.1 - Working Distinctions {#working-distinctions}

| Name used here | Meaning |
| --- | --- |
| case | One bounded continuing Work situation organized around an exact subject, state, commitments, evidence, authority, and permissible next Work. It is not its file, ticket, queue position, or every Work item within it. |
| case subject | The patient, incident, user issue, release candidate, service relation, request, physical item, or other exact subject around which continuation is being coordinated. |
| case-state claim | A qualified claim about the case subject and relevant relations at a stated time or horizon. It changes only from adequate evidence. |
| exception | A fact or condition for which the standard continuation branch is absent, contradicted, no longer adequate, or requires bounded choice or return. It is not automatically an error or rare event. |
| matching admission and permission | The applicable case admission and independently supported current permission for the same matter, effective conditions, configuration, and horizon. A valid `OPS.5` result may carry both; admission alone is not permission. |
| deciding System | The System authorized to select or confirm the next permissible Work. It may differ from the responsible performer. |
| responsible performer | The System assigned and capable for the selected Work under its conditions. Assignment, capability, permission, authority, and performance remain distinct. |
| next permissible Work | The exact Work that may occur next under the applicable domain Method, permission, obligations, evidence, and stop conditions. A task description or tool call alone does not show that this Work was performed. |
| action choice | A selected next Work, probe, fallback, stop, or return. Choice does not perform the Work or progress the case. |
| Work occurrence | Dated performance admitted from direct evidence under the relevant configuration. Intention, assignment, invocation, trace presence, or artifact creation does not establish it alone. |
| evidence expected from performance | The observations, produced results, or records needed to judge what occurred. State the claim each supports, including any claim of a changed subject state or a failure. |
| record update | A change to a ticket, case file, plan, model, trace, database, or dashboard. It may carry evidence but is not the case-state change by itself. |
| unmet condition | The exact missing, stale, contradicted, unauthorized, unsafe, unsupported, or unavailable condition that prevents a truthful next action or progressed state, together with its return or stop. |
| progression result | Either an evidenced progressed case state with its next return, or an unmet-condition return with owner, fallback or stop, and retry condition. |

## OPS.6:1 - Problem Frame {#problem-frame}

Continuing cases do not simply advance because a standard sequence exists. New observations, dependency failures, changed permissions, resource relations, specialist decisions, or unexpected outcomes can make yesterday's next action unsafe, impossible, or irrelevant. The operation still needs a bounded way to continue without replacing the applicable clinical, engineering, legal, safety, security, or other domain Method.

The practical problem is to select the next permissible Work from the current situation and then admit progression only after performance and evidence, while returning exact blockers rather than fabricating a state transition.

## OPS.6:2 - Problem {#problem}

Workflow systems encourage a false equation: transition selected equals Work performed equals case progressed. A case-file state, agent loop, plan update, model recommendation, or “done” ticket appears to settle the case even when no authorized performer acted or the resulting subject state is unknown.

The opposite failure treats every exception as improvisation. Practitioners bypass mandatory domain branches, create an ungoverned OptionSet, or keep analyzing without a responsible performer, stop, evidence expectation, or return. Cases then drift between records while obligations and commitments remain unresolved.

## OPS.6:3 - Forces {#forces}

| Force | Tension |
| --- | --- |
| responsiveness versus currentness | Cases need timely continuation, but stale facts or permission can make the selected action inapplicable or harmful. |
| domain Method versus local exception | The applicable Method constrains permissible Work, yet current facts may require recognition, adaptation, comparison, probe, or return. |
| chooser versus performer | The System that decides may not perform; collapsing them hides assignment, capability, permission, and responsibility. |
| action versus evidence | Selecting a good action is useful, but it does not show that Work occurred or the case changed. |
| recordability versus subject truth | Files and transitions support coordination, but they represent rather than constitute the case subject and state. |
| automation speed versus authority | Automated episodes can run quickly, but tool access and output do not establish permission, software assurance, release, or accountable continuation. |
| progress pressure versus honest blocker | A visible “next state” is attractive, while naming an unmet condition may be the only truthful result. |

## OPS.6:4 - Solution {#solution}

### OPS.6:4.1 - Confirm the case and matching permission {#confirm-the-case-and-matching-permission}

Name the exact case subject, current configuration and horizon, and the demand or commitment being served. Recover the applicable admission and the required current permission for the same matter and conditions. A valid `OPS.5` result may carry both; admission by itself does not establish permission. If the required permission is absent, expired, or contradicted, return that blocker to the authority or source that can resolve it; do not select Work or claim progression under a merely similar item, earlier approval, queue rank, or general mandate.

### OPS.6:4.2 - Refresh the action-changing situation {#refresh-the-action-changing-situation}

Recover the current qualified case state, applicable domain Method, obligations and operating commitments, action-changing evidence and its currentness, relevant permissions and authority, and the condition that made continuation uncertain. Follow only the reach that can change the next action; unaffected case claims remain reusable under their conditions.

### OPS.6:4.3 - Separate decision, performance, records, and state {#separate-decision-performance-records-and-state}

Name the deciding System, responsible performer, required permission or authority, available actions, actual Work to be performed, records used or changed, and the state claims the result may support. Do not infer one relation from another. If performer capability, assignment, access, permission, or authority is missing, return that exact condition.

### OPS.6:4.4 - Use the least elaborate adequate steering branch {#use-the-least-elaborate-adequate-steering-branch}

Apply the direct mandatory branch when a current rule and facts determine the next permissible Work. Use recognition when one current situation clearly matches a governed action. Adapt within the applicable domain Method when a bounded variation is authorized. Use `C.11` only when several admissible live actions genuinely require comparison. Select a bounded probe only when its expected information can change the decision. If no permissible action exists, generate candidates through the owning practice or return the missing result instead of improvising an ungoverned action.

### OPS.6:4.5 - Specify the executable continuation contract {#specify-the-executable-continuation-contract}

State the selected next Work, responsible performer, permission and effective conditions, stop or fallback, expected evidence, and the return to continuing operation. Name the observable change that would invalidate the action and require refresh. An existing plan, instruction, prompt, ticket-transition record, or model recommendation can carry this contract if it states these terms and identifies the required authorization.

### OPS.6:4.6 - Admit performance and update state separately {#admit-performance-and-update-state-separately}

After the Work, recover direct performance evidence, the changed subject or result, failures and limits, and the claim each observation supports. Update the case-state claim only when the relevant Work and resulting evidence are independently adequate. If Work did not occur or evidence is insufficient, retain the earlier state claim under its stated limits and return the unmet condition. Never use a record update, successful invocation, generated artifact, or selected action as automatic progression evidence.

### OPS.6:4.7 - Return one usable result {#return-one-usable-result}

Return either:

- an evidenced progressed case state, its evidence and limits, fulfilled or still-open obligations, and next return; or
- the unmet condition, direct owner or source of the needed result, safe fallback or stop, and exact retry condition.

State what remains outside: priority or commitment revision, queue and capacity policy, specialist judgement, release, safety, security, clinical outcome, legal permission, and other direct results.

## OPS.6:7 - Conformance Checklist {#conformance-checklist}

- [ ] The exact case subject, configuration, horizon, and served demand or commitment are named.
- [ ] The required current permission is supported for the same matter and conditions; admission alone is not treated as that permission.
- [ ] Current case state, domain Method, obligations, commitments, evidence, and exception are recovered.
- [ ] The deciding System, responsible performer, permission, capability, assignment, and authority remain distinct.
- [ ] Available actions, selected action, actual Work, records, evidence, and state claims remain distinct.
- [ ] Direct mandatory or recognition branches are used when adequate.
- [ ] `C.11` is used only when several admissible live actions genuinely require comparison.
- [ ] The continuation contract names Work, performer, conditions, stop or fallback, expected evidence, refresh, and return.
- [ ] Case progression is reported only after independently supported Work and adequate resulting evidence.
- [ ] A plan, ticket, model output, episode, trace, or record update is not treated as progress by itself.
- [ ] The result is either evidenced progression or an exact unmet-condition return with owner, fallback or stop, and retry.
- [ ] Specialist and wider Operations results remain with their owners.

## OPS.6:9 - Consequences {#consequences}

The operation gains a defensible continuation move for exceptional and changing cases. Practitioners can tell what may happen next, who should perform it, what evidence will count, when to stop, and whether the case truly progressed or remains blocked.

The cost is that visible motion no longer counts as progress by default. In some cases, the account cannot yet report progression while an unmet condition is returned. The pattern does not promise a universal workflow, automated resolution, clinical or engineering correctness, release, service fulfilment, or evidence that the selected Method is generally effective.

## OPS.6:12 - Relations {#relations}

- `OPS.5` supplies admission and may record independently grounded start permission for the same matter and effective conditions. Admission alone establishes neither permission, Work nor case progression.
- `A.15.7` governs the general situation-responsive steering Method. `A.3.1.MR` separately governs candidate reusable Method recovery from several performances or other direct evidence.
- `C.11` governs comparison only where several admissible live actions require choice. `A.10` governs evidence reliance; `A.15.8` governs the performance configuration or recovery dependency when that is current.
- `OPS.7` may consume an evidenced progressed state or unmet condition only as evidence where it changes priority or an existing commitment. It does not inherit revision authority.
- `OPS.8`–`OPS.13` retain wider queue, capacity, interacting-structure, and commitment-account questions.
- Clinical, medical-safety, consent, privacy, legal, software assurance, security, release, provider, capability, and other specialist practices retain their decisions and evidence.
- Pattern order is not a case lifecycle. Practitioners may enter OPS.6 directly with matching valid permission for an admitted case, repeat it as facts change, stop at a blocker, or return to another current pattern.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-5#root; FPF spec://ai.lev/fpf-spec/contract/A-15-7#root, spec://ai.lev/fpf-spec/contract/C-11#root, spec://ai.lev/fpf-spec/contract/A-10#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-adm/contract/ADM-6#root, spec://ai.lev/fpf-eng-chk/contract/CHK-4#root, spec://ai.lev/fpf-eng-mkt/contract/MKT-11#root, spec://ai.lev/fpf-eng-mkt/contract/MKT-7#root, spec://ai.lev/fpf-eng-ops/contract/OPS-7#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-6
