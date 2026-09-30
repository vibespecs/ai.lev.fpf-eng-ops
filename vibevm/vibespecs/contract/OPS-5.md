# OPS.5 - Admit Work and Limit Starts {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.5:0 - Use This When {#use-this-when}

Use this pattern when exact eligible operating demand may be explicitly started or committed now, but the operating System cannot honestly start everything that appears ready. Typical cues are “pull the next item”, “approve this case”, “the card is top priority”, “the agent is free”, “the rig has an opening”, or “we already selected it” without a current admission decision, start permission, or explicit start limit.

The first useful result is one bounded admission account:

> For eligible demand `D` serving operating result or commitment `R`, under criteria and non-negotiable conditions `K`, explicit-start limit `L`, deciding authority `A`, configuration and horizon `H`, each considered item is `admitted`, `deferred`, `rejected`, or `returned`; an admitted item has effective start conditions and an authorized starter where one exists; residual demand and the next review or return remain visible.

Recognition is cheap: enter when one exact demand item needs a truthful “may enter now?” answer. Assurance is stronger: eligibility, admission, priority, permission, commitment, actual Work, result, safety, release, and service fulfilment each retain their own evidence and authority.

Do not use OPS.5 to design a queue or buffer policy, identify or exploit the current constraint, size capacity under variability, coordinate interacting structures, or make a whole-service commitment credible. Return those questions to `OPS.8`–`OPS.13` when their results are available, or to a qualified direct source. If the current problem is continuing an already admitted case after facts changed, use `OPS.6`. If age, dependency, risk, or consequence may revise priority or an existing commitment, use `OPS.7`.

## OPS.5:0.1 - Working Distinctions {#working-distinctions}

| Name used here | Meaning |
| --- | --- |
| eligible demand | An exact demand item, such as a request, need, condition, case, or candidate Work item, that may be considered for current admission. Identify the demand claim and the subject it concerns separately. Eligibility is not admission, priority, permission, commitment, or Work. |
| option or request | A possible demand item presented for consideration. Its presence in a list or account creates no right to admission. |
| admission decision | A bounded decision about whether exact demand may enter the selected current coordination account under stated criteria, limits, horizon, and authority. |
| admitted item | Eligible demand whose admission conditions obtain for the stated configuration and horizon. Admission permits a further start decision under its conditions; it does not establish start or result. |
| deferred item | Demand not admitted now, with the observation, condition, horizon, or changed fact that would make reconsideration useful. |
| rejected item | Demand declined for this operating use, with its reason and any receiving return that another owner can answer. |
| returned item | Demand for which a named missing, stale, unsupported, or externally owned condition prevents this admission decision. |
| start permission | An obtaining permission or authorization for the admitted matter under effective conditions. A comparison or selected answer is not permission unless the deciding System also has and exercises the required authority. |
| explicit-start limit | A stated bound on what may be started now for this operating use. It is not a universal WIP number, capacity model, queue policy, or constraint-buffer design. |
| commitment | A promise or obligation with parties, content, conditions, horizon, authority, and status. Admission can rely on or create a bounded commitment only where the relevant authority is present. |
| authorized starter | The System permitted to initiate the admitted Work under the effective conditions. Responsibility, capability, availability, and permission remain separate. |
| Work occurrence | Dated Work whose occurrence is established from performance evidence, independently of the demand-admission decision. A card move, approval, selected item, plan, agent invocation, or generated artifact does not establish that Work occurred. |
| residual demand | Every considered or still-relevant demand item not in the admitted set, with enough identity and disposition to avoid hidden starts or silent loss. |
| admission result | The dispositions, reasons, conditions, authority, horizon, starter relations, residual demand, and next review or return that make the admission decision usable. |

## OPS.5:1 - Problem Frame {#problem-frame}

Continuing operation usually receives more apparent demand than it can honestly start. Requests arrive through customers, incidents, clinical cases, release candidates, providers, planned changes, automated agents, and internal commitments. Each item may be valuable, urgent, visible, or technically ready while still lacking the identity, evidence, permission, access, authority, or explicit-start condition required now.

The practical problem is not merely choosing the highest-ranked item. It is deciding which exact demand may cross into current operating coordination without hiding residual demand or treating selection alone as evidence that Work occurred.

## OPS.5:2 - Problem {#problem}

Boards and intake systems compress unlike truth states. “Ready”, “selected”, “approved”, “assigned”, and “in progress” become interchangeable labels. A high priority is treated as permission; an available performer as authority; a scheduled slot as capacity; a generated change as started Work; and an admission decision as a fulfilled commitment.

The opposite failure keeps every item nominally open. Nothing is explicitly rejected, deferred, or returned, so the operation accumulates hidden commitments and starts. Practitioners cannot recover which demand was considered, why it did not enter, or what would justify another look.

## OPS.5:3 - Forces {#forces}

| Force | Tension |
| --- | --- |
| responsiveness versus truthful starts | Delay can harm service, but premature starts create hidden Work, interruption, or unsafe continuation. |
| common intake versus unlike subjects | A shared account aids coordination, but incidents, patients, release candidates, provider changes, and rig requests retain different identities and conditions. |
| comparison versus direct rule | Several live alternatives may need choice, while mandatory or recognition-based conditions should not be converted into an artificial option contest. |
| local limit versus wider policy | One explicit-start bound can close the current decision without claiming a complete queue, capacity, or constraint Method. |
| visibility versus authority | Making demand and evidence visible helps, but neither visibility nor rank grants permission or commitment authority. |
| fast admission versus adequate evidence | A short-horizon answer is useful only if evidence currentness, conditions, and reopen triggers remain explicit. |
| focus versus residual demand | A bounded admitted set reduces active burden, but deferred, rejected, and returned demand must not disappear. |

## OPS.5:4 - Solution {#solution}

### OPS.5:4.1 - Recover only the action-changing operating inputs {#recover-only-the-action-changing-operating-inputs}

Name the deciding operating System, receiving result or commitment, configuration, and horizon. Reuse matching current `OPS.2`, `OPS.3`, and `OPS.4` results only where the selected coordination form, exact subjects and relations, current claims, uncertainty, permissions, commitments, or gaps can change admission. If an input is stale, mismatched, or absent, repair or return that exact blocker; do not reconstruct the whole operation by default.

### OPS.5:4.2 - Name each exact demand item and its proposed use {#name-each-exact-demand-item-and-its-proposed-use}

For every item under consideration, state the demand subject, claimant or source, proposed operating result, relevant commitment, and why admission is current. Keep a request, option, candidate Work item, admitted item, commitment, start permission, and performed Work separate even when one record represents several of them.

### OPS.5:4.3 - State criteria, non-negotiable conditions, and the explicit-start limit {#state-criteria-non-negotiable-conditions-and-the-explicit-start}

Record the conditions that can change the admission decision. Test exact identity; relevant readiness and evidence; required authority or permission; intended receiving use; safety, legal, clinical, security, or other specialist returns; performer and access conditions; current commitments; and the capacity, resource access, bounded concurrency, or explicit-start limit that matters now.

Do not translate these into a universal score. Some conditions are mandatory, some admit qualified comparison, and some require a return to another owner.

### OPS.5:4.4 - Choose only where a real choice exists {#choose-only-where-a-real-choice-exists}

When a direct domain rule, mandatory condition, or recognition branch gives the answer, apply it and record the basis. When several live admissible alternatives genuinely require comparison, form a stable current OptionSet and comparison basis and use `C.11`. If the options or comparison facts are insufficient, choose a bounded probe only when it can change the decision, or return the missing condition. Do not manufacture an OptionSet merely to make admission look analytical.

### OPS.5:4.5 - Give every item a usable disposition {#give-every-item-a-usable-disposition}

Return each considered item as:

- **admitted**, with reason, effective conditions and horizon, governing authority, authorized starter where established, and next review;
- **deferred**, with the condition, observation, horizon, or changed fact that makes reconsideration useful;
- **rejected**, with the reason and receiving return where another owner can answer the need; or
- **returned**, with the exact missing or externally owned result, what it blocks, safe stop, and retry condition.

Keep the residual demand visible. Record no start merely because the item is admitted.

### OPS.5:4.6 - Close the local decision and expose wider returns {#close-the-local-decision-and-expose-wider-returns}

State the admitted set, current explicit-start limit, unresolved or residual demand, next review, and the facts that reopen this admission. If the answer now depends on queue ordering, buffer design, a current constraint, capacity under variability, interacting structures, credible whole-service commitments, clinical triage, safety acceptance, release, law, finance, or another specialist result, return to that owner without filling the gap locally.

## OPS.5:7 - Conformance Checklist {#conformance-checklist}

- [ ] The exact operating System, receiving result or commitment, configuration, and horizon are named.
- [ ] Every considered demand item has an identity and proposed receiving use.
- [ ] Eligibility, admission, priority, permission, commitment, Work, and result remain distinct.
- [ ] Matching `OPS.2`, `OPS.3`, and `OPS.4` inputs are reused only where action-changing and current.
- [ ] Admission criteria and non-negotiable conditions include relevant evidence, authority, permissions, access, specialist returns, and currentness.
- [ ] The explicit-start limit is bounded to this use and is not presented as a universal queue, capacity, or constraint policy.
- [ ] `C.11` is used only for several real live alternatives on a stable comparison basis.
- [ ] Every item is admitted, deferred, rejected, or returned with reason, conditions, horizon, and next review or return.
- [ ] The authorized starter is named only where that relation is established.
- [ ] Residual demand remains visible.
- [ ] Admission is not claimed as started or completed Work.
- [ ] Wider Operations and specialist questions return to their direct owners.

## OPS.5:9 - Consequences {#consequences}

The operation gains a truthful boundary between demand and current starts. Participants can see what entered, what did not, why, under whose authority, for which horizon, and what should be reviewed. Hidden starts and silent residual demand become easier to challenge.

The cost is explicit identity, evidence, conditions, authority, and disposition work. Some demand remains visibly deferred or returned rather than cosmetically “active”. This pattern does not promise optimal throughput, maximum utilization, service fulfilment, or a complete queue, capacity, or constraint design.

## OPS.5:12 - Relations {#relations}

- `OPS.2` supplies a selected coordination-form decision where that form changes admission. `OPS.3` supplies exact operating subjects and direct relations. `OPS.4` supplies current claims, evidence, permissions, commitments, uncertainty, and gaps. None of those results admits demand by itself.
- `C.11` governs comparison only when several live admissible alternatives require choice. `A.10` governs evidence reliance; `A.15.8` governs performance-configuration and recovery questions when they become the actual blocker.
- `OPS.6` may consume the applicable admission and independently supported current permission for the same matter and conditions. An admission result may carry both; admission alone establishes neither permission, Work nor progression.
- `OPS.7` separately governs current priority or bounded commitment revision. `OPS.8`–`OPS.13` retain queue, buffer, constraint, capacity, interacting-structure, and wider commitment questions.
- Clinical, safety, legal, privacy, security, finance, product release, capability, and other specialist practices retain their subjects, evidence, permission, authority, and conclusions.
- Pattern order is not Work order. Practitioners may enter OPS.5 directly when matching current inputs already exist, repeat it as demand changes, or stop after its result.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): spec://ai.lev/fpf-eng-ops/contract/OPS-2#root, spec://ai.lev/fpf-eng-ops/contract/OPS-3#root, spec://ai.lev/fpf-eng-ops/contract/OPS-4#root; FPF spec://ai.lev/fpf-spec/contract/C-11#root, spec://ai.lev/fpf-spec/contract/A-10#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-adm/contract/ADM-5#root, spec://ai.lev/fpf-eng-ops/contract/OPS-17#root, spec://ai.lev/fpf-eng-ops/contract/OPS-6#root, spec://ai.lev/fpf-eng-ops/contract/OPS-8-1#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-5
