# OPS.8.1 - Choose Work-Release Rules When Earlier Work Can Return {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

> **Type:** Method pattern
> **Status:** Stable
> **Normativity:** Normative

## OPS.8.1:1 - Problem frame {#problem-frame}

**Use this when** finishing one operation can trigger new work even though the previous result may still need correction, another visit or downstream acceptance. A specialist finishes an analysis and begins a long client session; the analysis then returns for urgent revision. A part leaves a machine but may return after inspection. An admission limit frees a place at local completion while later work still needs the same resources.

Choose what event should permit another start, what remaining and possible work that start must accommodate, and how the decision changes when feedback arrives. The result is a release rule that can be operated: a signal, eligible next work, a load or time condition, treatment of returns and a response when the conditions no longer fit.

Start with the result and resource that the rule must protect. If the existing rule already handles these returns adequately, use it through OPS.5 rather than reconstruct it for every admission. Identifying the resource that limits throughput, when that is uncertain, is a separate contribution from OPS.9.

## OPS.8.1:2 - Problem {#problem}

A completion signal establishes that something finished within its stated boundary. The next start can nevertheless displace work still needed for the previous customer's result. A rule that waits for all possible later claims can create the opposite loss: useful resources remain idle while a completed item awaits a response that uses none of them.

The operator needs to compare these consequences before selecting a signal. The signal, the population limited by a card or count, the resource load and the customer's completion event may have different boundaries.

## OPS.8.1:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| Earlier release and correction capacity | Starting sooner can advance new work but occupy the resource needed when an earlier result returns. |
| Simple counts and unequal demands | One freed place is easy to recognize; the returning and incoming jobs may require very different resources and times. |
| Protection and useful idle time | Holding capacity can preserve a deadline; excessive protection postpones work without improving the required service. |
| Feedback timing and decisions | Waiting can reveal whether a return is needed, but that information may arrive too late to protect the result. |
| Local pace and the receiving result | A constraint's completion can regulate replenishment while another resource or downstream join determines customer delivery. |

## OPS.8.1:4 - Solution {#solution}

**Working sequence:** choose the receiving result → locate the proposed release signal → recover work that remains or can return → compare the next admission with the capacity it would leave → choose the rule and its response to feedback → operate it and reconsider the changed conditions.

The capacity comparison can return to the proposed signal, job selection, resource arrangement or commitment. A signal that works for one product mix may fail for another.

### OPS.8.1:4.1 - Choose the completion and release events separately {#choose-the-completion-and-release-events-separately}

Name the service to be protected, its receiving result and relevant horizon or deadline. Retain the event from which the customer has been waiting. Then identify the event currently proposed to permit another start: an operation completes, the selected constraint consumes its next ready job, a job leaves a controlled loop, acceptance arrives, or the remaining workload falls below a limit.

For a count limit, identify what enters and leaves its population. For a replenishment signal, identify the activity and ready supply it serves. Define readiness for the next operation using OPS.8; future outputs need not already exist.

Ask what obligation or operating work survives the signal. Trace it to the resource that would perform it. A card may be returned when a job leaves one loop even though that job still contributes load to another resource or a later visit. Preserve those contributions in the comparison.

### OPS.8.1:4.2 - Recover known work and possible returns {#recover-known-work-and-possible-returns}

For each resource that can change the release decision, establish the unfinished operations already assigned to it, their remaining occupancy, calendars and required times. Include known later visits by the same job. Count the resource use of each visit, while retaining one customer's result and waiting history.

For work that may return, identify the event that reveals the need, when the resource could be needed and the possible amount and kind of work. A supported bound, a small set of scenarios or a joint probability model can be enough, depending on the receiving question. Preserve shared causes: the same defect may return several jobs together.

Separate work already known to remain from allowance for work that is still contingent. If a return becomes known, replace its contingent allowance with the actual remaining work; do not add both for the same visit. When acceptance or another suitable event excludes that return within the selected horizon, release the corresponding allowance. An acceptance event does not remove separately retained warranty or other later service obligations.

When the possible return cannot yet be quantified, keep the supported comparison and identify which promised service remains unsupported. Further observation is useful when it can change the release choice. The responsible person can choose to release despite the unresolved possibility; distinguish that choice from a claim that the earlier service is protected.

### OPS.8.1:4.3 - Test what capacity the next start leaves {#test-what-capacity-the-next-start-leaves}

Begin with the simplest consequence that can decide the question. In a fixed horizon, the known remaining occupancy, the proposed job's occupancy and a chosen allowance for returns can be compared with usable resource time.

For example, a resource with five usable hours cannot complete two hours of existing work, two hours of a protected return and two hours of new work within that horizon. Passing the total-hours comparison is only a necessary condition: readiness, precedence, joint resources and uninterrupted windows may still prevent placement. OPS.10.2 constructs that schedule or obstruction.

Match the comparison to the promised protection:

- For a stated return scenario, place that return and the new work with their readiness, access and deadlines.
- For protection over a bounded family, show that the selected response can handle every member of that family.
- For a probability requirement, use the joint model and the operating policy through OPS.10.1; a mean return load alone does not determine a service probability.

A policy that reacts to feedback must use information available at the time of its choice. If release is allowed before inspection, the policy needs an executable response when inspection later requires a return. It cannot choose an early start only in retrospect for the outcomes in which no correction was needed.

A workload-control norm can instead be a calibrated congestion-control quantity. Retain its definition and units: a route-position-weighted load is not the same quantity as occupied hours available before a deadline. Use its operating comparison for its intended purpose, and a finite schedule when the deadline question requires one.

### OPS.8.1:4.4 - Compare signals and their return treatment {#compare-signals-and-their-return-treatment}

Compare the existing rule with a material alternative on the same arrivals, resources, receiving result and waiting origin. Keep the rule's actual mechanism visible.

| Candidate rule | What permits new work | What to resolve about returns |
| --- | --- | --- |
| Completion at a selected constrained activity triggers replenishment | That activity consumes the next ready supply and calls for its replacement. | Which later work can revisit this resource or occupy another resource needed for delivery? What ready supply and remaining capacity protect those visits? |
| A job's departure frees a place in a limited loop | The controlled population falls below its limit. | Is a return inside that loop, or admitted through another rule after departure? Retain its load wherever it will be served. |
| Remaining workload fits the selected norms | The candidate's contributions fit the resource-specific load rule. | Include repeated visits under that rule, distinguish known work from uncertain returns, and define what happens when feedback changes the load. |
| Acceptance permits the next start | The selected receiving event closes the exposure being protected. | Does waiting for this event preserve useful capacity, or unnecessarily hold a place while acceptance uses another resource? |

The names Drum-Buffer-Rope, CONWIP and workload control locate families of these methods; they do not settle the particular boundaries or exception rules. A rule can combine a replenishment signal with a return allowance or use a separate return queue. Evaluate that combination rather than assuming that choosing a name determines its behavior.

Compare the delay imposed on new work with the protected earlier result. If holding one job would starve an important resource, consider another ready job with compatible resource use, a smaller independently useful unit, another capable resource or a different start window. Any exception that spends protected capacity changes what the rule can support. OPS.7 and OPS.13 supply priority and commitment decisions when the two services cannot both be retained.

### OPS.8.1:4.5 - Define the actions at release and feedback {#define-the-actions-at-release-and-feedback}

Choose the next eligible work and the condition under which it can start. Make the condition usable in the operation's existing account: for example a freed loop place together with a reserved correction window, or a remaining-load calculation updated at inspection.

At a return, restore the work's readiness and resource demand, replace the corresponding allowance, and apply the selected priority and placement rule. Keep the original customer clock. A repeated service visit may restart a station's own interval without restarting the customer's wait.

At no-return confirmation, remove only the allowance that the event actually resolves, then reconsider held work. At late or ambiguous feedback, update the possible demand and the time left; absence of a message alone does not establish acceptance.

Observe whether the rule changes completion, total waiting, resource starvation, actual correction burden and displaced work. Reopen it when the return route, feedback time, service duration, resource access, product mix or receiving requirement changes. Stop redesigning once the existing inputs support a usable rule or a specific choice requiring changed conditions.

## OPS.8.1:7 - Conformance Checklist {#conformance-checklist}

- The receiving result, its time requirement and the proposed release event are distinguishable.
- Known remaining operations and possible returns retain their resource use, readiness and customer waiting origin.
- Any claimed protection states its scenario, bounded family or probability interpretation; an unresolved risk remains visible in the release choice.
- A total-load screen is followed by placement when calendars, precedence or uninterrupted work can change feasibility.
- Feedback replaces or releases the relevant allowance; it does not count the same return twice.
- The selected rule states what happens to both returning work and the next candidate, including conflicts that need a changed priority or commitment.
- A changed feedback time or return route can reopen the decision.

## OPS.8.1:9 - Consequences {#consequences}

The release rule can exploit available capacity while retaining the demand that may return. Its price is the information and coordination needed to distinguish the relevant events and resource contributions. A small deterministic comparison may suffice; larger operations can need the capacity and scheduling constructions.

Some conflicts remain real. Protecting an earlier correction can delay new work, and waiting for information can itself make the earlier result unattainable. The method exposes those choices for the responsible operating decision.

## OPS.8.1:12 - Relations {#relations}

OPS.8 supplies the queue, readiness and protective-policy context. OPS.5 applies the resulting rule to a particular admission; OPS.6 continues an admitted case; OPS.7 and OPS.13 handle priority and commitment changes.

OPS.11.1 supplies the operating arrangement and resource relationships. OPS.15.1 constructs the visit, occupancy and customer-time quantities. OPS.10.1 compares capacity and uncertain service; OPS.10.2 constructs the finite schedule and revises it after feedback. These contributions let the release rule remain about when to start work rather than redefining the underlying quantities or scheduling method.

MMP.8 and MMP.8.SD supply sequential information and consequence reasoning when the choice depends on what can be learned before acting. C.11 supports choice under the actual alternatives and resources; C.29 retains correspondence between the modeled load and the operating work.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-8#root, spec://ai.lev/fpf-eng-ops/contract/OPS-5#root; conditional spec://ai.lev/fpf-eng-ops/contract/OPS-10-1#root/.2, spec://ai.lev/fpf-eng-ops/contract/OPS-15-1#root, spec://ai.lev/fpf-think-mmp/contract/MMP-8#root/.8.SD @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-8-1
