# OPS.18 - Control Operating Quality and Reliability {#root}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Working sections of the pattern; its depth sections live in the source document named by the last line. See LICENSE.md for the list of changes.

## OPS.18:1 - Problem frame {#problem-frame}

**Use this when** an operating result may no longer meet its requirement, observed service failures exceed the agreed allowance, a recurring process changes, a lot needs acceptance or an incident raises a containment, recovery or recurrence-prevention question.

Begin with the result at risk, the affected population or configuration, and the action someone is authorized to take. Select the evidence method for that question. The first useful result is a decision about the affected work, service or output, together with the next action and the evidence and conditions needed to support it.

This pattern governs operating decisions about quality and reliability. A monitoring account is one input. A qualified product requirement, clinical decision, statistical method or engineering acceptance result may be another. If the question is only how to define and reconcile observations, use OPS.15. If a current response policy and adequate evidence already settle the action, apply them directly.

For example, twelve nonconforming items in a sample can trigger investigation under a process-monitoring rule. A lot-disposition decision still needs its own acceptance basis. Likewise, exhausting a software service's error budget can pause discretionary changes while urgent restoration continues under the responsible authority.

## OPS.18:2 - Problem {#problem}

Different quality questions are often compressed into one status: the process looks stable, the customer objective was met, the lot passed or the service is restored. Each statement needs different evidence and supports a different action.

A dashboard can therefore look satisfactory while the actual service remains impaired. The opposite failure reacts to every fluctuation as a process change, consuming effort and destabilizing work without a suitable monitoring basis.

## OPS.18:3 - Forces {#forces}

| Force | Practical tension |
| --- | --- |
| prompt response and false signals | Earlier detection can help containment while unsuitable thresholds create unnecessary interventions. |
| stability and acceptability | A stable process can repeatedly produce results that fail the requirement. |
| aggregate service and local consequence | A good average can hide an affected customer group or a short severe incident. |
| restoration and causal understanding | Service may be recoverable before the cause is fully established, while recurrence prevention still needs investigation. |
| continuity and protected conditions | Urgent recovery work requires the capability, authority and protections of its actual operation. |

## OPS.18:4 - Solution {#solution}

### OPS.18:4.1 - Recover the result, requirement and available action {#recover-the-result-requirement-and-available-action}

State the operating result at risk: conforming output, correct responses, timely service, availability or restored operation. Recover the relevant population, configuration, period, requirement and consequence of failure. Name the authority for continuation, containment, acceptance and restart where those decisions differ.

Use the actual requirement. A product specification, an agreed service objective and a statistical control limit answer different questions. A control limit describes variation under its model. A requirement states what the result must satisfy. Recover each from its appropriate basis.

If a known violation already calls for a protective action, take that action under the current authority while obtaining the missing diagnosis or recovery result. A broad data analysis is unnecessary before a response already required by the observed condition.

### OPS.18:4.2 - Select the evidence branch {#select-the-evidence-branch}

| Current question | Evidence method | First operating use |
| --- | --- | --- |
| Has a recurring process changed from its established behavior? | A suitable statistical monitor with a qualified baseline, sampling rule and response policy. | Continue observation or investigate and contain the affected process/result. |
| Is event-based service meeting its objective? | Good/eligible event definitions, observation coverage, window, permitted loss and a response policy. | Adjust continuation or change activity under the service decision. |
| Should a particular lot or result be accepted? | Its qualified acceptance plan, defect definitions, sampling basis and relevant risks. | Accept, reject, segregate, rework or obtain the missing acceptance result. |
| Can an impaired service be restored or restarted? | Evidence of the failure, containment or repair, and the required restart conditions. | Restore service under the appropriate authority and continue any unresolved investigation. |
| What prevention does an incident or near miss need? | Reconstructed events, material explanations and sufficient support for feasible protective measures. | Select and verify prevention under :4.4, retaining the limits on the causal conclusion. |

Branches can be complementary. Select each because its answer changes the current action. A favorable result from one branch cannot supply the evidence required by another.

For recurring variation, recover whether observations are comparable, whether the baseline is appropriate and whether the selected model fits the data. Independence, changing sample size, seasonality, clustering or rare events can change the required monitor. A simple chart should yield to a qualified statistical method when its assumptions or detection performance are inadequate.

For an event-based service, define the good and eligible events from the recipient's experience. Check omitted events, important subgroups and observation delay. A fast failure can require a timely alert before an end-of-window aggregate is available.

For acceptance, recover the lot or item, what counts as a defect, the sampling/inspection method, and the consequences of accepting unacceptable output or rejecting acceptable output. Obtain the qualified plan where it is missing. An operating practitioner can use a supplied plan without deriving its statistical design anew.

### OPS.18:4.3 - Interpret the observation within its evidence limits {#interpret-the-observation-within-its-evidence-limits}

Calculate the selected quantity from its declared population. Use OPS.15 when event identity, coverage, time or missing observations need repair. Preserve any consequential uncertainty in the control decision.

A process-monitoring signal supports the action specified by its policy; it does not identify the cause by itself. An observation within the limits can still violate a product requirement. A capability claim needs the relevant stable-process and specification basis.

An error budget expresses permitted service loss for a stated objective and population. Compare observed loss with that allowance, then apply the authorized policy. Protected safety, human or clinical conditions remain applicable regardless of budget remaining.

A sample acceptance result supports the named lot decision under its plan and risks. It does not establish that every item conforms, that the process is stable or that a known failure mechanism has been corrected.

### OPS.18:4.4 - Carry out containment or recovery and preserve continuing service {#carry-out-containment-or-recovery-and-preserve-continuing}

Select an action within the available authority: continue with observation, segregate affected output, pause a risky change, adjust admission, restore a known workable configuration, rework a lot or request the needed professional decision. State the affected scope and any service that must continue.

Obtain the capability, access and protected human conditions required for the action. Use OPS.12/.13 if recovery competes with existing service or relies on extra cover. An urgent label can identify priority; the actual assignment and authority determine who may act.

Where containment restores service before the cause is known, state what remains unresolved. Enter the following inquiry when prevention still needs an explanation. Extending a correction to new operating conditions requires support for its protective effect there; a stronger causal claim needs evidence for that claim. Reuse sufficient existing results, and apply a qualified correction directly when they settle the action.

1. **Reconstruct the incident.** Recover the failed result and requirement, affected occurrences and configurations, sequence, effects and containment already performed. Obtain the relevant participants' knowledge and permitted records. Distinguish observations from inferred links and identify missing facts that could matter to prevention.
2. **Develop the material explanations.** Follow contributing conditions beyond the immediate symptom, allowing several interacting conditions or rival accounts. Use B.5.2 when plausible explanations still need to be developed. For a disputed link, identify the existing observation, established mechanism or attainable test that could support or challenge it. C.28 helps qualify the causal conclusion; domain knowledge and evidence must supply the links in this incident.
3. **Choose supported prevention.** Compare retaining adequate protection, a narrow configuration or access correction, a change to the reusable way of working and a larger redesign where these are credible alternatives. Assess future exposure and avoidable consequences together with the full effort, delay, displaced service and other burden of each change. C.11 governs the choice; use C.11.CRC when the contribution of a finite change to the present arrangement needs that comparison. Zero loss in a near miss does not remove the exposed future consequence.
4. **Assign and verify the chosen change.** Name who will deliver it, the required result and its completion conditions. A recurring operating Method change belongs to OPS.16; choosing among ways to retain in an operating repertoire belongs to OPS.17. A local configuration, access or maintenance correction can finish as that correction. Verify completion separately from the restart conditions and later recurrence observations in :4.5.

Require sufficient support for the proposed protection under the relevant explanations that remain plausible. If they all support the same available correction, choosing a final causal account is unnecessary for that prevention decision. Retain the unresolved explanation wherever it limits a claim or later use. Obtain another observation when it can change the prevention, its permissibility or burden, or what the evidence warrants saying. If the worth or feasibility of that inquiry is itself unsettled, use C.11.DUA. Applicable protection and evidence requirements continue to govern the action.

### OPS.18:4.5 - Verify restart and choose the next observation {#verify-restart-and-choose-the-next-observation}

Recover the condition under which service, normal production or discretionary change may resume. Obtain the observation that actually establishes it: applicable test evidence, a confirmed working configuration, restored service behavior, qualified acceptance or another required result.

Check the observation's scope and time. A restarted process, a new reporting period or an empty incident queue is not itself evidence that the defect was corrected. Preserve residual uncertainty and a response if the condition fails again.

Choose follow-up from the consequence and detection need. Large isolated departures, small persistent drift and rapid incidents may need different observation rules. Retain enough evidence for the continuing decision, and end collection that no longer contributes to a decision, required assurance or recovery.

Return the action, its evidence, affected population/configuration, authority and restart or next-observation conditions in the existing operating account. The selected control decision is the result; the chart or dashboard makes its basis inspectable.

## OPS.18:7 - Conformance Checklist {#conformance-checklist}

| Check | Evidence sufficient for the declared use |
| --- | --- |
| The result and possible action are clear. | Requirement, affected population/configuration, consequence and response authority are recoverable. |
| The evidence method answers that question. | Monitoring, service-objective, acceptance, recovery and prevention uses retain their distinct bases. |
| The observation is interpretable. | Baseline, sample or event population, coverage, time, model and uncertainty fit the claim. |
| The action follows the applicable rule. | Continuation, containment, acceptance, restoration or Method change uses the actual policy and protected conditions. |
| Restart has real evidence. | The required result is established at the relevant scope and time; a reporting reset does not stand in for it. |
| Remaining work is directed. | Unresolved cause, recurrence risk, missing professional result or changed method assumption has a concrete receiving use. |
| Prevention has sufficient support. | Further discrimination changes prevention, permissibility, burden or a supported claim; a common adequately supported correction can proceed with the remaining explanation explicit. |

## OPS.18:9 - Consequences {#consequences}

The practitioner can connect quality and reliability evidence to a concrete operating response. The action remains scoped to the affected output, service or configuration, while necessary service can continue under its own conditions.

Monitoring and acceptance can incur false alarms, missed failures, inspection cost or delayed service. Recovery can restore operation while leaving a cause unresolved. Selecting the method and evidence by consequence makes these trade-offs visible instead of hiding them in a single green status.

## OPS.18:12 - Relations {#relations}

OPS.15 helps construct the observation account when its subjects, coverage or definitions are unresolved. OPS.4 guides shared attention to qualified operating state. OPS.5–OPS.7 guide admission, continuation and attention to aging work when the control decision changes those actions.

Use OPS.12 for human conditions and OPS.13 for service commitments and resource choices affected by containment or recovery. OPS.14 helps compare consequential operating and financial alternatives. OPS.16 evaluates a change to an operating Method; OPS.17 compares and refreshes the repertoire of ways available for operating work.

B.5.2 helps develop rival explanations of the incident; C.28 qualifies their causal support. C.11 and C.11.CRC support the choice and whole-burden comparison of preventive changes. C.11.DUA enters only when the contribution or feasibility of a requested inquiry remains in question.

FPF C.16 governs the measures and statistical assumptions relied on, and A.10 preserves evidence reach. A.11.OP limits additional monitoring or records to their decision, assurance or recovery contribution. Engineering, clinical and other qualified practitioners supply the specific acceptance, protection or restoration results their domains require.


## Dependencies {#dependencies}

- @fact:DEPENDS-ON Dependencies (as published): conditional spec://ai.lev/fpf-eng-ops/contract/OPS-12#root–spec://ai.lev/fpf-eng-ops/contract/OPS-15#root, spec://ai.lev/fpf-eng-ops/contract/OPS-17#root; FPF spec://ai.lev/fpf-spec/contract/C-16#root, spec://ai.lev/fpf-spec/contract/A-10#root, spec://ai.lev/fpf-spec/contract/A-11-OP#root @status:spec/done
- @fact:REFERENCED-BY Referenced by (computed from the Tables of Contents): spec://ai.lev/fpf-eng-cgov/contract/CGOV-9#root, spec://ai.lev/fpf-eng-chk/contract/CHK-4#root, spec://ai.lev/fpf-eng-eam/contract/EAM-5#root, spec://ai.lev/fpf-eng-ops/contract/OPS-13#root, spec://ai.lev/fpf-eng-ops/contract/OPS-15#root, spec://ai.lev/fpf-eng-ops/contract/OPS-17#root @status:spec/done

#source spec://ai.lev/fpf-eng-ops/source/OPS-18
