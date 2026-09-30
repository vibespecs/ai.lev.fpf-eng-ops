# OPS.4 - Keep Current Operating State Recoverable Across Participants {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.4:0 - Use This When {#use-this-when}

Use this pattern when people must coordinate continuing Work but act from stale, partial, conflicting, differently authorized, or differently grained accounts of the same operating subjects. Typical cues are “we need one source of truth”, a control room with no claim provenance, a board that hides field state, a case handoff that loses the next decision, or a dashboard whose users cannot tell what they may change.

The first useful move is to create or repair one participant-usable account for one decision:

> For subjects `S` and commitments `C`, current claims are `Q` at horizons `T`, supported by `E` with provenance and uncertainty `P`; participants may read or change `...`; disagreements and gaps are `G`; next decisions or permissible Work are `N`; refresh or expiry occurs under `R`.

Aligned attention does not require identical screens or consensus. It requires that participants can recover the subjects, qualified claims, evidence, permissions, disagreements, and next decision relevant to their Work.

Recognition is cheap: enter when a participant cannot resume, decide, or explain a material disagreement from the maintained account. Assurance is claim-specific: world state, evidence, authority, permission, Work, safety, stability, causal effect, and release or acceptance decisions keep their own governing patterns.

Do not use OPS.4 to build a generic dashboard, mandate transparency, create one shared mental model, replace specialist records, or declare state true because it is visible. If the current problem is a Work-performance configuration or recovery dependency after interruption or support loss, use `A.15.8` for that general question and keep the operation-specific state and commitments here.

## OPS.4:0.1 - Working Distinctions {#working-distinctions}

| Name used here | Meaning |
| --- | --- |
| current operating account | A participant-usable set of qualified claims tied to exact operating subjects, commitments, evidence, permissions, decisions, and refresh conditions. It is neither the operating System nor a universal database. |
| subject-state claim | A claim about one exact subject or relation at a stated time or horizon, with scheme, conditions, provenance, uncertainty, and authority. |
| currentness | The condition under which a claim remains usable for a named decision and horizon. Recent timestamps alone do not establish it. |
| provenance | The source, observation, transformation, record, and responsibility facts needed to judge the claim's receiving use. Provenance does not make the claim true by itself. |
| uncertainty | Missing, estimated, conflicting, stale, or bounded information whose reach can change action. |
| disagreement | Two or more recoverable claims, interpretations, or decisions that cannot yet be used as one result. Visibility of disagreement is compatible with aligned attention. |
| permission and change authority | Separately supported relations governing who may read, write, approve, hold, release, or otherwise use account content. Visibility, responsibility, assignment, and capability imply none of one another. |
| next decision or permissible Work | The decision or Work option currently enabled, blocked, or awaiting a named condition. The account does not perform or authorize it by display. |
| participant view | A use-bounded representation of selected account claims for one participant action. Several views may coexist when subject and claim correspondence remain recoverable. |
| control representation | A view, loop diagram, dashboard, or control-room display representing selected control structures, relations, rates, or account claims. It establishes none of those facts by appearance. |
| attention-maintenance result | The smallest repaired current account, participant views, gaps, refresh rules, and next-decision returns that let the named participants coordinate. |

## OPS.4:1 - Problem Frame {#problem-frame}

Continuing operation needs a present account because the operation outlives one meeting, screen, shift, or model session. Claims arrive at different rates from field observations, cases, tests, providers, plans, queues, and specialist decisions. Different participants need different slices and hold different authority.

The aim is therefore not one display or total agreement. It is recoverable correspondence between exact subjects, qualified claims, evidence, permissions, disagreements, and the next decisions each participant must make.

## OPS.4:2 - Problem {#problem}

Visibility without claim discipline amplifies error. A fresh dashboard can repeat stale field state, a green board can hide an unresolved service commitment, and an integrated twin can merge observations with predictions and planned states. Participants appear aligned until a decision exposes different referents, time horizons, or authority.

The opposite failure stores every record and overwhelms users. Important gaps, conflicts, and expiry conditions disappear in detail, so people reconstruct state from memory or private channels.

## OPS.4:3 - Forces {#forces}

| Force | Tension |
| --- | --- |
| Speed | Participants need a quick current view, while rushed aggregation can erase provenance and uncertainty. |
| Several horizons | Field control, incident response, release, provider change, and finance update at unlike rates. |
| Several participants | People need different views and permissions, while divergence can hide conflicting claims. |
| Continuing Work | Handoffs and interruptions require recoverability, while an account cannot guarantee capability or performance. |
| Disagreement | Teams want one answer, while preserving a qualified conflict can be safer than premature consensus. |
| Representation | Dashboards and control rooms improve attention, while appearance can be mistaken for state, authority, or proof. |

## OPS.4:4 - Solution {#solution}

Maintain the smallest decision-specific account that lets named participants recover exact subjects, current qualified claims, commitments, evidence, uncertainty, permissions, disagreements, next decisions, and refresh conditions. Present several views when needed, but keep claim and subject correspondence explicit.

### OPS.4:4.1 - Pattern-Use Unfolding {#pattern-use-unfolding}

1. **Name participants and decisions.** State who must resume, coordinate, hold, release, escalate, or perform next Work; name the horizon and useful stop for each action.
2. **Import exact subjects and relations.** Use the OPS.3 operating-subject account. Do not let a dashboard row, case file, queue position, or control diagram replace the subject or obtaining relation.
3. **Select only decision-changing claims.** For each subject or commitment, state the current claim, effective scheme, conditions, time or horizon, and action it can change.
4. **Attach evidence and provenance.** Name source, observation or result, carrier, transformation, version, evidence reach, and uncertainty needed for reliance. Keep prediction, plan, observation, and decision claims distinct.
5. **Expose conflict and absence.** Preserve incompatible claims, missing observations, stale evidence, unknown authority, and unresolved specialist returns. Do not average them into false agreement.
6. **Recover permissions and authority.** State who may read, write, annotate, accept, hold, release, or change each relied-on claim or decision. Keep assignment, capability, responsibility, permission, and authority separate.
7. **State next decisions and permissible Work.** Name what is enabled, blocked, awaiting evidence, or returned to a specialist; include the condition and participant that can advance it.
8. **Construct participant views.** Select the smallest representation for each action. Preserve subject identity and claim correspondence; show what the view omits and where claims conflict, and provide a return to the owning account. Do not require one screen.
9. **Keep control views separate.** A selected FPF control view may expose observer, controller, plant, supervisor, observation, actuation, feedback, and rates. The account carries qualified operating claims about those subjects and relations; the view or loop picture establishes neither current state, feedback closure, rate adequacy, stability, safety, authority, nor an Operations Method.
10. **Test interruption and handoff when current.** Use `A.15.8` for the general Work or WorkPlan performance-configuration question. Ask a representative next participant to recover the bounded question, current claims, evidence, disagreements, permissions, next Work, and stop without private memory.
11. **Refresh, expire, and reopen.** State update sources, expected cadence or event, expiry rule, supersession and conflict handling, and the observation that reopens only the affected claim, view, or decision.

### OPS.4:4.2 - Record the Result {#record-the-result}

| Result position | Required content |
| --- | --- |
| use boundary | Participants, actions or decisions, horizons, first useful result, and truthful stops. |
| subjects and commitments | Exact OPS.3 subjects and direct relations; commitment parties, content, conditions, status, and authority. |
| current claims | Claim content, effective scheme, time/horizon, conditions, uncertainty, and receiving action. |
| evidence and provenance | Sources, observations/results, carriers, transformations, versions, reach, and missing evidence. |
| permissions and authority | Read, write, annotate, accept, hold, release, and change relations with their scope and basis. |
| disagreement and gaps | Conflicting or missing claims, affected decisions, specialist returns, and non-admissible compression. |
| next decisions and Work | Enabled, blocked, awaiting, or returned actions; required condition and responsible participant. |
| participant views | Selected claims, subject correspondence, explicit scope of omitted material, conflict cues, return route, and access limits. |
| refresh and recovery | Update or expiry conditions, handoff/recovery observation when current, and smallest reopen rule. |

### OPS.4:4.3 - What Changes in Practice {#what-changes-in-practice}

Participants stop asking whether everyone sees the same dashboard. They ask whether each participant can recover the exact subjects, claims, evidence, permissions, disagreements, and next action needed for that participant's decision. A visible conflict or honest unknown becomes a usable coordination result. A record update no longer masquerades as changed world state.

## OPS.4:7 - Conformance Checklist {#conformance-checklist}

- [ ] The account begins from named participants, decisions/actions, horizons, and useful stops.
- [ ] Exact OPS.3 subjects, commitments, and direct relations remain recoverable in every relied-on view.
- [ ] Each current claim states content, scheme, time/horizon, conditions, evidence/provenance, uncertainty, and receiving action.
- [ ] Observation, prediction, plan, record, decision, and world-state claims remain distinct.
- [ ] Disagreements, missing observations, stale evidence, and specialist returns remain visible with their decision reach.
- [ ] Read, write, annotate, accept, hold, release, responsibility, capability, and authority relations are not inferred from one another.
- [ ] Next decisions and permissible Work name their enabling or blocking conditions.
- [ ] Participant views preserve subject and claim correspondence, make omitted scope and claim conflicts visible, and provide a return to the owning account.
- [ ] A control representation establishes none of current state, feedback closure, rate adequacy, stability, safety, authority, or Method.
- [ ] Refresh, expiry, supersession, handoff/recovery observation when current, and smallest reopen rules are explicit.

## OPS.4:9 - Consequences {#consequences}

The pattern improves continuation across shifts, tools, teams, and interruptions without requiring one representation or consensus. It makes uncertainty and disagreement actionable and lets views change without losing subject identity.

The cost is explicit provenance, permission, conflict, and refresh maintenance. Some attractive dashboards become secondary because they cannot preserve the claim and authority distinctions needed by the decision.

## OPS.4:12 - Relations {#relations}

- `OPS.3` supplies exact subjects, direct relations, records, state claims, provenance, conflicts, permissions, and gaps. `OPS.2` supplies selected participant and control views plus correspondence obligations.
- `C.2.1` governs the claim-bearing account episteme; `A.10` governs evidence reliance; `A.15.8` governs the general Work/WorkPlan performance-configuration and recovery question.
- `C.30.LCA`, `B.2.5`, `C.27.TA`, `C.27`, and `A.3.3` govern the conditional control structure, relation, and rate/dynamics claims. OPS.4 retains operation-specific commitments, state, intervention, authority/evidence, and consequences.
- `OPS.5` later consumes current eligible demand, commitments, and uncertainty for admission. `OPS.6` consumes case state and permissible next Work. `OPS.15` and `OPS.18` remain separate inspectability and operating quality/reliability decisions.
- Security, privacy, law, safety, medicine, product engineering, finance, governance, and other specialists retain their evidence, permission, authority, and decision results.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-2#root, spec://ai.lev/fpf-eng-ops/contract/OPS-3#root; FPF spec://ai.lev/fpf-spec/contract/C-2-1#root, spec://ai.lev/fpf-spec/contract/A-10#root, spec://ai.lev/fpf-spec/contract/A-15-8#root; conditional spec://ai.lev/fpf-spec/contract/C-30-LCA#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-chk/contract/CHK-5#root, spec://ai.lev/fpf-eng-ops/contract/OPS-10#root, spec://ai.lev/fpf-eng-ops/contract/OPS-11#root, spec://ai.lev/fpf-eng-ops/contract/OPS-15#root, spec://ai.lev/fpf-eng-ops/contract/OPS-5#root, spec://ai.lev/fpf-eng-ops/contract/OPS-8#root, spec://ai.lev/fpf-eng-ops/contract/OPS-9#root, spec://ai.lev/fpf-eng-syse/contract/SYSE-38#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-4
