# OPS.4 - Keep Current Operating State Recoverable Across Participants: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.4:5 - Archetypal Grounding — PumpWorks Current Operating Account {#archetypal-grounding-pumpworks-current-operating-account}

The weekly release decision uses a small account rather than one status board:

| Account claim | Evidence, uncertainty, and authority | Next decision or Work |
| --- | --- | --- |
| `FieldIncident-I73` may affect controller behavior at `FieldPumpInstallation-P4`. | Field-engineer report and telemetry record are current to different times; lab reproduction is absent; service-impact extent is disputed. Field service may update observations but cannot accept product safety. | Continue bounded diagnosis, obtain lab evidence, and keep release effect unresolved. |
| `ReleaseCandidate-R42` passed tests `T1–T8`; `T9` remains blocked by rig access. | Signed test results identify candidate and fixture versions; the test-rig booking is current but does not prove a completed test. Release authority remains separate. | Await exact rig access and `T9`; no release from card status. |
| `SafetyQuestion-S19` has no current specialist decision. | The issue record contains a question and evidence request, not a safety verdict. Only the named safety authority can return the needed result. | Hold the affected release use or narrow its scope under the current authority rule. |
| `ProviderChange-P8` changes model-artifact access after the current window. | Contract and technical-access records disagree on effective date. | Resolve the access relation or choose the supported incumbent route. |
| Weekly evidenced-release commitment is at risk. | Incident, test, provider, and release claims have different horizons and authority. The account displays the relation without collapsing them into one status. | Release, hold, rollback, narrow, or renegotiate only through the corresponding authority and evidence. |

The product-side control view separately represents `FieldTelemetryObserver-O4`, `DeployedController-C17`, plant `FieldPumpInstallation-P4`, `FieldModeSupervisor-S1`, and their direct relations where supported. The operating-supervision view separately represents reports from `PumpWorks-ControlServiceOps` and constraints returned by `ReleaseSupervisorTeam-S2`. The separately qualified temporal claims concern sub-second product control, minute-to-hour field observation, daily incident triage, weekly release, and slower provider change.

The OPS.4 account may cite claims about those participants, relations, and rates. The control diagram does not establish their current state, two-sided feedback, stability, safety, release authority, or the account itself. A dashboard can display the release hold and missing `T9`; it does not create either fact.

For a shift or model-session handoff, the next participant must recover the operating question, five subject claims above, evidence versions, unresolved conflicts, permissions, next permissible Work, and stop. If recovery requires private memory or an unrecorded chat, `A.15.8` returns the exact missing carrier, update/use relation, cue, or support condition. OPS.4 then repairs the operation-specific account claim or view.

Reopen only the affected claim when new telemetry arrives, `T9` completes, safety authority returns a decision, provider access changes, a commitment is renegotiated, or a participant view can no longer support its action.

## OPS.4:6 - Bias-Annotation {#bias-annotation}

| Recurring bias | Likely drift | Repair |
| --- | --- | --- |
| single-source-of-truth bias | One database or screen is treated as the world and final authority. | Preserve exact claims, provenance, conflicts, permissions, and receiving decisions. |
| visibility-as-alignment bias | Everyone can see the board, so coordination is assumed. | Test whether each participant can recover the next decision and disagreement. |
| consensus bias | Conflicting qualified claims are forced into one status. | Keep disagreement explicit with evidence reach and resolution condition. |
| freshness bias | The newest timestamp is assumed current for every horizon. | State claim-specific currentness and expiry for the receiving use. |
| access-authority bias | The ability to edit or view is treated as authority to decide. | Recover permission and decision authority separately. |
| representation-as-control bias | A loop or control room is treated as feedback closure or operating Method. | Recover actual relations and keep view, account, rates, and stronger claims distinct. |
| memory-repair bias | People or models are told to remember more after handoff failure. | Use A.15.8 to recover the missing state, carrier, update/use relation, cue, or support condition. |

## OPS.4:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Repair |
| --- | --- |
| “Build one dashboard for everyone.” | Start from participant actions and select claims and views for each, with correspondence and return. |
| “Green means done.” | Recover the subject state, commitment, evidence, acceptance or fulfilment result, and authority. |
| “Latest update wins.” | Apply claim-specific currentness, source reach, conflict, and supersession rules. |
| “Make everyone agree.” | Preserve qualified disagreement and name the evidence or authority needed for resolution. |
| “If it is editable, the team owns it.” | Separate access, permission, responsibility, assignment, and decision authority. |
| “The control room closes the loop.” | Recover the in-life relation sides and rate claims; treat the display as a representation. |
| “The handoff failed because attention was low.” | Identify the missing subject claim, carrier, update/use relation, cue, permission, or stop. |

## OPS.4:10 - Rationale {#rationale}

Shared attention is an operating achievement when participants can coordinate from qualified claims about the same subjects and commitments. That achievement is weaker than universal agreement and stronger than common visibility. A small decision-specific account preserves the distinction, while FPF continues to govern epistemes, evidence, Work-performance recovery, structures, and control claims.

## OPS.4:11 - SoTA-Echoing {#sota-echoing}

| Practice question | Selected current line and serious alternative | Defect overcome and governed loci | Source roles and limits | Reopen condition |
| --- | --- | --- | --- | --- |
| How should participants maintain shared attention to current operating state without treating visibility as truth, agreement, authority, or control? | The selected current line is a **small decision-specific account of qualified claims with provenance, uncertainty, permissions, conflicts, participant views, next action, and refresh**. The serious default is a **single real-time dashboard, latest record, or “single source of truth”** used as the shared state. | The default hides stale or incomparable claims, erases qualified disagreement and authority, and lets a display stand for world state or feedback closure. **Adapt:** `OPS.4:4.1` selects claims from participant actions, `OPS.4:4.2` returns a refreshable account, `OPS.4:4.3` permits honest conflict and local repair, and `OPS.4:5` tests handoff and recovery. **Reject:** common visibility or edit access as sufficient evidence, agreement, permission, or control. | Current FPF supplies the account, evidence, recovery, temporal, and control boundaries. Kanban is the official comparator for bounded workflow visibility; OCEL and object-centric work preserve several histories; DORA, harness, and loop sources supply fast-changing AI-assisted-operation cases; layered-control/LCA sources expose relation and rate distinctions. None establishes a universal shared-state carrier, authority model, or effectiveness result. | Reopen if a stronger current coordination account or repeated handoff case achieves the same provenance, conflict, authority, refresh, and recovery value with lower burden, or if a source changes the minimum claim content or account/control boundary. |

The selected comparison is supported by the following bounded source roles and limits.

| Source line | Retained contribution | Use boundary |
| --- | --- | --- |
| Current FPF `C.2.1`, `A.15.8`, `A.10`, `C.30.LCA`, and `C.27.TA` | Claim-bearing account focus, configuration/recovery testing, evidence use, control-view boundary, and temporal/currentness claims. | FPF supplies no Operations subject selection, service commitment, domain intervention, or release authority. |
| [The Kanban Guide 2025.5](https://kanbanguides.org/the-kanban-guide/2025.5/) | Make workflow definition, Work items, active items, states, and flow measures visible for managing a bounded Kanban workflow. | Board visibility and measures do not establish world state, shared truth, every case, or a complete operating account. |
| [OCEL](https://www.ocel-standard.org/specification/overview/) and [object-centric process management](https://doi.org/10.3390/math11122691) | Preserve several subject histories and event-object relations instead of forcing one case identifier. | Event records remain evidence with source and serialization limits; they do not establish current state or authority by themselves. |
| DORA 2025, harness engineering, and loop engineering, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Make context capacity, bounded concurrency, traceable episodes, evidence-gated stopping, integration burden, and human continuation needs visible in AI-assisted operation. | Fast-changing software/provider cases have short refresh horizons and establish no universal attention, memory, stopping, or effectiveness rule. |
| Layered-control and LCA sources, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Expose unlike observation, actuation, supervision, feedback, and rate relations in selected structures. | The source diagrams and labels are not the operating account, Operations Method, stability proof, safety result, or authority. |


## OPS.4:End {#end}
