# OPS.3 - Distinguish Operating Subjects, Cases, Queues, Resources, and Records: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.3:5 - Archetypal Grounding — PumpWorks Subject Account {#archetypal-grounding-pumpworks-subject-account}

The weekly release decision initially sees four cards and a rig calendar. OPS.3 expands only the distinctions that change action:

| Visible item | Recovered subject or relation | Record boundary |
| --- | --- | --- |
| `ReleaseCandidate-R42` card | A release-candidate subject and its candidate contents, required evidence results, release Work items, and receiving release decision. | The card and commit identifiers are records; moving the card does not change deployed field state or satisfy the release commitment. |
| `FieldIncident-I73` ticket | A case organized around `FieldPumpInstallation-P4`, reported symptoms, service commitments, evidence, authority, permissible next Work, and closure conditions. | Ticket closure does not establish restored field condition or fulfilled service. |
| `SafetyQuestion-S19` issue | A question episteme, related evidence needs, specialist safety decision, and any Work items created to obtain that result. | A red label is neither a safety state nor authority to accept risk. |
| `ProviderChange-P8` epic | A time-bounded change subject with provider relations, access conditions, project WorkPlan content, affected release cases, and decisions. | The epic does not make the provider part of PumpWorks or prove performed migration Work. |
| test-rig booking row | Queue membership of an exact eligible request for resource relation to `TestRig-2`, with interval, order/policy, access condition, and status evidence. | The booking row records planned access. Establish request eligibility, allocation authority, performed test Work, and test completion separately. |

Records remain distinct: ticket, trace, source commit, build result, test result, service log, field-engineer report, telemetry record, and release decision each support bounded claims. A multi-object event record may relate one event to several subjects, but it does not identify those subjects with one case or prove the represented Work.

For the product-side control view, `FieldPumpInstallation-P4`, `FieldTelemetryObserver-O4`, `DeployedController-C17`, and `FieldModeSupervisor-S1` retain their relation-specific meanings. For operating supervision, `ReleaseSupervisorTeam-S2` is an admitted acting System only where supported and the two-sided report/constraint relation to `PumpWorks-ControlServiceOps` is recorded only if both sides obtain. The diagram, participants, relations, state claims, and operating account remain distinct.

The result supplies OPS.4 with exact subjects, records, current claims, conflicts, permissions and refresh needs. Reopen only the affected identity or relation when a release candidate is superseded, an incident splits or merges under an explicit rule, a queue membership changes, a record source becomes stale, or a claimed control relation loses one side.

## OPS.3:6 - Bias-Annotation {#bias-annotation}

| Recurring bias | Likely drift | Repair |
| --- | --- | --- |
| card-identity bias | Card, case, Work item, and subject become one thing. | State separate identities and direct relations. |
| case-file bias | The file becomes the continuing case. | Name the subject, commitments, current facts, permissible Work, and closure conditions. |
| queue-container bias | A column or list is treated as an obtaining queue. | Recover membership, order/service relation, policy, interval, and evidence. |
| resource-scalar bias | A person, machine, or capability is reduced to available hours. | Preserve the subject and exact access, support, allocation, or use relation. |
| event-log realism | A log is treated as complete performed Work. | Preserve source limits and admit Work independently. |
| object-centric collapse | Multi-object linkage is read as one universal case or process. | Keep subjects, event relations, records, views, and receiving uses distinct. |
| control-role reification | Observer, controller, plant, or supervisor labels become permanent kinds. | Recover participant meanings in exact obtaining relations. |

## OPS.3:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Repair |
| --- | --- |
| “One issue equals one unit of value.” | Name the represented subject, Work item, result relation, identity rule, and receiving decision. |
| “The customer is in the queue.” | State whether the queued participant is a request, case, Work item, physical subject, or another exact entity. |
| “The resource is 80% utilized.” | Identify the resource subject, availability/allocation/use relation, time window, Work, and decision. |
| “The event log shows the process.” | State the logged events, object relations, source coverage, reconstruction rule, and missing Work evidence. |
| “Status Done means fulfilled.” | Recover the commitment, supplied result, acceptance or fulfilment evidence, and authority separately. |
| “The dashboard closes the feedback loop.” | Recover both in-life relation sides and keep the display, claims, rates, and proof separate. |

## OPS.3:10 - Rationale {#rationale}

Operations decisions act on subjects and obtaining relations, while coordination normally uses records and representations. Keeping those layers distinct preserves practical speed without allowing tool schemas to decide ontology. A minimal relation-specific account is enough when it names what can change the decision and what remains unsupported.

## OPS.3:11 - SoTA-Echoing {#sota-echoing}

| Practice question | Selected current line and serious alternative | Defect overcome and governed loci | Source roles and limits | Reopen condition |
| --- | --- | --- | --- | --- |
| What is the smallest operating account that preserves decision-bearing subjects and relations across cases, queues, resources, events, and records? | The selected current line is **subject- and relation-first, multi-object where needed, with records and events retained as qualified evidence**. The serious default is **case-ID, ticket, schema, or event-log first**, where one recorded identifier or serialization becomes the operating subject. | The default creates false identities, denominators, completion claims, and causal or state inferences. **Adapt:** `OPS.3:4.1` recovers exact subjects and direct relations, `OPS.3:4.2` records representation and evidence limits, `OPS.3:4.3` localizes repair, and `OPS.3:5` tests several unlike subjects. **Reject:** record closure, event order, shared fields, or one case identifier as sufficient world-side state. | OCEL and object-centric process management are the best-known-line candidates for escaping one-case convergence in event data. CMMN and DCR are serious bounded case/constraint alternatives; DEMO contributes commitment and coordination distinctions; current FPF governs obtaining relations and claim-bearing accounts. These sources do not prove performed Work, current world state, causal effect, or one universal operating ontology. | Reopen if a stronger current account or repeated use preserves the same identities, direct relations, provenance, uncertainty, and local repair at lower effort, or if a source changes the minimum multi-object or record-use distinction. |

The selected comparison is supported by the following bounded source roles and limits.

| Source line | Retained contribution | Use boundary |
| --- | --- | --- |
| Current FPF `A.6.REL`, `C.2.1`, `B.2.5`, and direct subject patterns | Recover obtaining relation occurrences, claim-bearing epistemes, two-sided supervision relations, and subject-specific identity. | FPF does not choose Operations subjects, domain queues, records, service commitments, or intervention consequences. |
| [CMMN 1.1](https://www.omg.org/spec/CMMN/1.1/PDF) and [DCR](https://doi.org/10.4204/EPTCS.69.5) | Preserve changing case facts, discretionary planning, milestones, and declarative condition/response relations. | A case plan or constraint model is not the case subject, performed Work, or complete Operations Method. |
| [OCEL](https://www.ocel-standard.org/specification/overview/) and [object-centric process management](https://doi.org/10.3390/math11122691) | Relate events to several objects and retain object histories instead of forcing one case identifier. | OCEL 2.1 adds serializations to the OCEL 2.0 model; neither an event log nor an object link establishes the world-side operation, complete Work, or one universal case. |
| DEMO 2020/2024, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Distinguish production and coordination Work, transaction roles, commitments, responsibility, and result relations. | Source-local transaction constructs do not become general FPF relation kinds or a complete operating ontology. |
| Integrated material, transaction, information, financial, and relation-specific network sources, see the [source account](spec://ai.lev/fpf-eng-ops/pub/framework-boundary-and-refresh#source-use-and-currentness) | Preserve several connected, non-isomorphic structures for one decision. | Shared nodes or proximity do not create one universal flow or network identity. |


## OPS.3:End {#end}
