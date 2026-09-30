# OPS.6 - Continue Cases and Handle Exceptions: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.6:5 - Archetypal Grounding — Three Continuing-Case Replays {#archetypal-grounding-three-continuing-case-replays}

### OPS.6:5.1 - PumpWorks field incident {#pumpworks-field-incident}

`FieldIncident-I73` is an admitted continuing case under the current incident Method. The operation refreshes incident impact, deployed-controller and telemetry correspondence, missing test `T9`, rig access, provider conditions, safety return, release authority, and service commitments. The incident chooser, responsible diagnostic or validation performer, release and safety authorities, candidate Work, records, and case state remain distinct.

If current permission and rig access support a bounded diagnostic replay, OPS.6 states that Work, performer, stop, fallback, and expected telemetry or test evidence. Report case progression only after the Work and evidence support a changed incident claim. If `T9`, rig access, safety return, provider permission, or current telemetry is absent, the result names that unmet condition and returns to its owner. A ticket move, agent run, recommendation, or code change does not by itself establish incident progression or release.

### OPS.6:5.2 - Public-hospital clinical case {#public-hospital-clinical-case}

One admitted clinical case continues from the exact patient and clinical-case subjects, current observations, applicable clinical and operating Methods, authorized practitioners, bed and resource relations, service obligations, and current consent, privacy, safety, and statutory conditions. A qualified clinical System retains medical decisions.

OPS.6 can state the next authorized clinical or operating Work, responsible performer, stop or fallback, and evidence needed before the case-state claim changes. Missing consent, clinical evidence, bed relation, competence, medical-safety return, or statutory permission remains an unmet condition, not an Operations workaround. A record closure, bed-board move, or elapsed wait does not establish treatment, patient change, or clinical resolution.

### OPS.6:5.3 - AI-assisted user issue {#ai-assisted-user-issue}

An admitted user issue encounters a changed trace, tool result, provider condition, model input, candidate change, or harness state. The operation refreshes evidence and applies the software domain Method and current established authority. It distinguishes the human or other deciding System, the responsible performer, agent episode, tool invocation, candidate change, test evidence, issue record, and release decision.

The continuation contract may authorize one bounded diagnostic, test, or repair Work with context and tool limits, stop, fallback, evidence expectation, and human return. Report issue or candidate progression only after performance evidence supports it. A successful episode, green local test, visible trace, automated loop, or generated patch does not by itself establish issue progression, an integrated change, software assurance, a security result, or release permission.

## OPS.6:6 - Bias-Annotation {#bias-annotation}

| Bias or pressure | How it distorts continuation | Countermeasure |
| --- | --- | --- |
| workflow-state bias | A configured transition becomes the case truth. | Recover the exact case subject, performance evidence, and qualified state separately. |
| action bias | Selecting any next step feels better than returning a blocker. | Use direct mandatory and recognition branches first; return when no permissible action exists. |
| automation bias | A successful agent episode or model output is treated as progress. | Separate invocation, Work, artifact, evidence, integration, and case-state claims. |
| plan-completion bias | Updating a plan or checklist appears to satisfy the obligation. | Name the actual Work, responsible performer, result, and evidence expected. |
| stale-permission bias | Earlier permission is reused after conditions changed. | Match matter, conditions, configuration, horizon, and authority before selection. |
| expert-shadowing bias | Operations quietly substitutes for clinical, safety, legal, or engineering judgement. | Return the bounded specialist result and keep the receiving coordination decision local. |
| exception novelty bias | Every surprising event is treated as unprecedented improvisation. | Reuse the applicable domain Method and choose the least elaborate adequate branch. |

## OPS.6:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Failure | Repair |
| --- | --- | --- |
| workflow transition equals progress | A representation substitutes for changed case state. | Require independently supported Work and resulting evidence. |
| selected action equals Work | A choice or instruction becomes a performance claim. | Name performer and admit the dated Work separately. |
| agent ran, therefore case advanced | Invocation and output hide authority, integration, and subject evidence. | Preserve episode, Work, artifact, test, integration, decision, and state distinctions. |
| generic exception handler | One fallback overrides domain Methods and specialist returns. | Recover the applicable Method and exact unmet condition. |
| chooser-performer collapse | Decision authority, assignment, capability, and performance become one relation. | Name and support each relation independently. |
| stale authorization carryover | Permission survives changed conditions by default. | Revalidate exact matter, configuration, horizon, and effective conditions. |
| endless analysis | No responsible performer, stop, evidence expectation, or return is stated. | Produce the executable continuation contract or a blocker return. |

## OPS.6:10 - Rationale {#rationale}

Case continuation sits between permission and evidence. If it collapses into admission, selection appears to perform Work. If it collapses into priority or commitment management, elapsed time or consequence pressure can bypass the applicable domain Method. Keeping the continuation contract and the later state update separate makes exceptions usable without inventing a lifecycle.

The two-result form is deliberate. An exact unmet condition with owner, safe fallback, and retry can be the complete useful Operations result. It prevents administrative state changes from hiding missing permission, capability, evidence, or specialist conclusions.

## OPS.6:11 - SoTA-Echoing {#sota-echoing}

| Practice question | Selected current line and serious alternative | Defect overcome and governed loci | Source roles and limits | Reopen condition |
| --- | --- | --- | --- | --- |
| How should an admitted continuing case choose and evidence its next permissible Work when facts or exceptions change? | The selected line is **situation-responsive steering inside the applicable domain Method, with separate permission, chooser, performer, Work, evidence, state update, stop, and return**. The serious default is a **workflow, case-plan, ticket, or automated loop transition used as the progression result**. | The default confuses representation with subject state and choice with performance. **Adapt:** `OPS.6:4.1`–`OPS.6:4.7` confirm permission, refresh action-changing facts, choose the least elaborate branch, specify performance, and admit state change only from evidence. **Reject:** one universal case lifecycle, record-to-Method inference, or agent output as progress. | Current FPF `A.15.7` supplies the general next-action steering Method and `C.11` bounded choice. CMMN contributes discretionary case planning and state representation; DCR contributes condition, response, inclusion, exclusion, marking, execution, and acceptance distinctions. DEMO contributes bounded commitment, coordination, and responsibility distinctions. DORA, harness, and loop sources contribute short-horizon evidence, bounded concurrency, traceable episodes, stops, integration burden, and human continuation. None supplies the case's domain state, authority, Work, progression evidence, release, or universal Operations Method. | Reopen if a stronger continuation account preserves the same permission, domain-Method, performer, performance, evidence, state, blocker, and return boundaries with less burden, or if a source changes the permissible-action or evidence contract. |

The selected comparison is supported by these bounded source roles.

| Source line | Retained contribution | Use boundary |
| --- | --- | --- |
| Current FPF [`A.15.7`](spec://ai.lev/fpf-spec/contract/A-15-7#root) | Currentness, domain-Method limits, chooser, performer, authority, direct branch, comparison, probe, fallback, stop, and feedback for live next-action selection. | Supplies no case-specific permission, state, obligation, domain evidence, operating commitment, or progression result. |
| Current FPF [`C.11`](spec://ai.lev/fpf-spec/contract/C-11#root) | Choice among several formed admissible alternatives and bounded probe-worthiness. | Does not generate permissible actions, authorize performance, or prove state change. |
| CMMN 1.1 and the DCR source line, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Discretionary planning, condition and response, inclusion and exclusion, marking, execution, and acceptance distinctions. | A notation, case file, model, or transition neither chooses, authorizes, performs, nor proves effective continuation. |
| DEMO, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Production/coordination Work, commitment, responsibility, and transaction distinctions. | Source-local roles do not assign authority or establish performance in another organization. |
| DORA 2025, harness engineering, and loop-engineering sources, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Context and tool capacity, bounded concurrency, traceable episodes, evidence-gated stopping, integration load, and human continuation. | Supply no universal AI operation, agenthood, model capability, release, security, safety, provider authority, or effectiveness result. |


## OPS.6:End {#end}
