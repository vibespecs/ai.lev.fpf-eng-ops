# OPS.5 - Admit Work and Limit Starts: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.5:5 - Archetypal Grounding — Three Admission Replays {#archetypal-grounding-three-admission-replays}

### OPS.5:5.1 - PumpWorks controller service {#pumpworks-controller-service}

`PumpWorks-ControlServiceOps` considers `ReleaseCandidate-R42`, `FieldIncident-I73`, `SafetyQuestion-S19`, `ProviderChange-P8`, and competing test-rig requests while maintaining weekly evidenced-release commitments. The current account exposes missing test `T9`, a safety-return gap, provider-access conflict, release authority, service consequences, and the current rig-access relation.

OPS.5 keeps the items separate. It can admit bounded incident-diagnosis Work for `FieldIncident-I73` when identity, incident authority, evidence, performer, and access conditions obtain. It defers release continuation whose required `T9` evidence or rig access is absent. It returns `SafetyQuestion-S19` to the competent safety authority. A high rank, booked rig request, release candidate, or weekly horizon creates neither capacity, permission, Work, nor release. The first usable result is the item-by-item admission account and visible residual demand; the first honest blocker is the exact missing permission, evidence, access, or specialist return.

### OPS.5:5.2 - Public-hospital emergency-care operation {#public-hospital-emergency-care-operation}

One emergency-care operating function considers operating Work around exact patient and clinical-case subjects, changing observations, waiting, bed relations, service horizons, and current clinical and operating evidence. OPS.5 can return a bounded operating admission disposition only from authorized inputs. It does not turn a patient into a generic Work item or infer clinical priority from waiting age.

If consent, clinical evidence, competence, medical-safety, privacy, statutory permission, or another specialist condition is missing, the result names that blocker and its owner. Operations neither supplies treatment authority nor overrides clinical judgement. The first useful result is an authorized operating admission or an exact returned condition, not a dashboard state or automatic triage result.

### OPS.5:5.3 - AI-assisted software operation {#ai-assisted-software-operation}

One software operation considers user issues, agent episodes, candidate changes, harness and tool access, traces, test results, human decisions, and release commitments. OPS.5 uses current context and tool capacity, bounded concurrency, integration burden, evidence needs, and established human or other authority to decide what may start.

A model score, available agent, free context window, generated patch, or scheduled episode does not by itself establish admission, permission, performed Work, or release. The result admits only the exact bounded Work whose identity, conditions, evidence, access, authority, and start limit obtain; it defers or returns the rest with retry conditions. Security, software assurance, provider capability, agenthood, and release authorization remain direct specialist returns.

## OPS.5:6 - Bias-Annotation {#bias-annotation}

| Bias or pressure | How it distorts admission | Countermeasure |
| --- | --- | --- |
| visibility and rank bias | The top visible item appears authorized and ready. | Test identity, evidence, permission, authority, and start conditions separately. |
| sunk-commitment pressure | Earlier planning or public promise is used to force admission. | Recover the actual commitment parties, conditions, authority, and current status. |
| utilization pressure | Every available person, rig, tool, or model is filled immediately. | State the bounded receiving result and explicit-start limit; preserve deliberate non-start. |
| automation bias | A model recommendation or generated artifact is treated as admission or Work. | Require a separate admission result, authorized starter, performance evidence, and later result evidence. |
| urgency leakage | Age or consequence language becomes automatic admission order. | Leave priority and commitment revision to `OPS.7`; use only the current admission criteria here. |
| silent-rejection pressure | Deferred or rejected demand disappears from the account. | Preserve identity, disposition, reason, retry or return, and residual demand. |
| source-school anchoring | A familiar board, backlog, buffer, or WIP rule supplies the whole Method. | Adopt only the bounded mechanism that changes this decision and keep its limits explicit. |

## OPS.5:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Failure | Repair |
| --- | --- | --- |
| top card means start | Rank substitutes for authority and permission. | Record admission, permission, starter, and start conditions separately. |
| everything is “in progress” | Hidden starts erase residual demand and overload the operation. | Apply an explicit-start limit and give every item a disposition. |
| availability implies capacity | A free slot, worker, rig, tool, or model is treated as a complete capability and access result. | Recover the exact performer, resource relation, capability, permission, and configuration. |
| choose-first option set | An artificial score replaces mandatory conditions or direct rules. | Use the direct branch; compare only genuine admissible alternatives. |
| admission by artifact | Ticket creation, assignment, plan, model output, or code generation becomes “Work started”. | Admit actual Work only from independent performance evidence. |
| rejection without return | Demand silently disappears or repeatedly re-enters. | Keep the reason, residual identity, owner, and retry condition. |
| local rule claims the system | One start limit becomes a universal WIP, queue, capacity, or constraint Method. | Bound the result and return wider policy questions. |

## OPS.5:10 - Rationale {#rationale}

Admission is valuable because it protects the boundary between possible demand and authorized current Work. Combining it with queue design, performed Work, or service assurance would make a locally usable decision depend on much wider results and would hide exactly where permission and evidence are needed.

The four dispositions prevent the false binary “start or lose”. Direct rules remain direct, genuine alternatives can be compared, and residual demand stays available for reconsideration or specialist return. The pattern therefore closes the smallest decision that lets a continuing operation limit starts while leaving unresolved queue, constraint, capacity, interacting-structure, and whole-service questions for their own decisions.

## OPS.5:11 - SoTA-Echoing {#sota-echoing}

| Practice question | Selected current line and serious alternative | Defect overcome and governed loci | Source roles and limits | Reopen condition |
| --- | --- | --- | --- | --- |
| How should an operating System decide what may enter now without confusing priority, permission, commitment, and Work? | The selected line is a **bounded item-by-item admission account with explicit conditions, authority, starter relation, start limit, residual demand, and review**. The serious default is a **ranked backlog or workflow-state transition used as permission to start**. | The default hides mandatory conditions and residual demand and lets visibility or selection stand for authority and Work. **Adapt:** `OPS.5:4.1`–`OPS.5:4.6` reuse current inputs, separate truth states, apply direct rules or genuine comparison, and return four dispositions. **Reject:** universal backlog ontology, fixed WIP number, or local admission as proof of performance or service. | Current FPF `C.11` supplies bounded choice among already formed alternatives, not admission criteria or authority. The Kanban Guide supplies bounded Work-item, active-item, WIP, age, cycle-time, throughput, and explicit-policy concepts. TameFlow supplies the option-versus-committed-Work and hidden-demand concerns. Reinertsen supplies queue, delay, variability, feedback, and economic trade-off mechanisms. None supplies a universal Operations Method, start permission, or complete current capacity result. | Reopen if a stronger admission account preserves all truth states, residual demand, authority, start limits, and specialist returns with less burden, or if a source changes an action-bearing admission condition. |

The selected comparison is supported by these bounded source roles.

| Source line | Retained contribution | Use boundary |
| --- | --- | --- |
| Current FPF [`C.11`](spec://ai.lev/fpf-spec/contract/C-11#root) | Choice, rejection, probe, and reroute among an already formed current OptionSet. | Supplies no domain criteria, permission, commitment, performed Work, or operating result. |
| [The Kanban Guide 2025.5](https://kanbanguides.org/the-kanban-guide/2025.5/) | Bounded Work-item boundary, active-item management, WIP, throughput, Work-item age, cycle time, and explicit workflow policies. | Supplies no universal board, queue discipline, WIP value, service guarantee, or complete admission Method. |
| TameFlow sources, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Distinguish options from committed Work and expose hidden demand, commitment, interaction, financial, and human-condition concerns. | The backlog/buffer prescription and concern set are not universal kinds or comparative proof. |
| Reinertsen, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Queue, delay, batch, WIP, feedback, variability, and multivariable economic trade-offs. | Supplies no universal priority score, permanent optimum, local-utilization rule, authority, or Work evidence. |


## OPS.5:End {#end}
