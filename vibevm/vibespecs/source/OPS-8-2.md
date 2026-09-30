# OPS.8.2 - Use Protective Capacity While Keeping It Available: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.8.2:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.8.2:5.1 - Practice during an operator's reserve interval {#practice-during-an-operator-s-reserve-interval}

An already-qualified operator has a 45-minute interval during which a call can require a return to protected service within five minutes. Once back, the operator and required equipment can sustain that service. A proposed practice exercise uses an independent training setup and can be stopped at short points.

The constructed timing assumptions are maximum durations under this arrangement:

| Return operation | Minutes |
| --- | ---: |
| Detect the call | 1 |
| Reach a stopping point and leave the needed resumption note | 1 |
| Move to the protected workstation | 1 |
| Recover its current situation and prepare the next action | 2 |
| Total, with these operations serial and no additional waiting | 5 |

This exercise fits the stated response requirement. The calculation does not establish its learning value; its practice and feedback still need to serve the selected development question.

A live lesson with a 25-minute segment that cannot be left can exceed the entire five-minute allowance before transfer or restoration begins. Its fit within the 45-minute interval does not make it suitable for this anytime-call protection.

Now change the workstation's restoration to five minutes. The former exercise gives 1 + 1 + 1 + 5 = 8 minutes and no longer preserves the response. Preparing a usable handover in advance might reduce restoration, but that is a changed arrangement whose time and burden must be included. Otherwise choose another activity or preserve readiness.

### OPS.8.2:5.2 - A free machine but an unavailable setter {#a-free-machine-but-an-unavailable-setter}

A machine must be ready for its protected job at 09:30. There is no earlier-call requirement in this case. An auxiliary trial needs five minutes of setup by a setter, twenty minutes of unattended machine time and five minutes of restoration by that setter. The setter is available from 09:00 to 09:20 and then from 09:40. The protected job's operator is available at 09:30.

The duration sum is thirty minutes. But setup at 09:00–09:05 and running at 09:05–09:25 leave restoration waiting until 09:40–09:45. The trial does not fit the protected start.

If a separately useful ten-minute trial is available, setup at 09:00–09:05, running at 09:05–09:15 and restoration at 09:15–09:20 fit both calendars. The machine is ready before 09:30. Alternatively, prepare a different unit or obtain another qualified setter; merely labeling the trial low priority changes none of these times.

This arrangement protects the named start. It has not established immediate recall during the trial's indivisible machine cycle.

### OPS.8.2:5.3 - Suspending a background AI job leaves its accelerator occupied {#suspending-a-background-ai-job-leaves-its-accelerator-occupied}

A protected computation needs an accelerator and its memory. A background job uses that allocation while the protected queue is empty. The scheduler can suspend the job's execution, but under this configuration suspension retains the accelerator allocation. Starting the protected job requires that allocation to be released.

A “suspend on arrival” rule therefore fails to provide the needed resource even if the suspension command is immediate. For example, Slurm's generic-resource documentation states that resources allocated to a suspended job remain unavailable to other jobs. Use a release mechanism supported by the actual application and scheduler, such as checkpointing followed by termination and later restart.

For a constructed alternative, allow one minute to receive the call, checkpoint and terminate; one minute to release and clean up the allocation; and one minute to load the protected computation. With those serial bounds and resources available, the three-minute return fits a three-minute start requirement. The protected computation's subsequent capacity needs are also assumed to fit.

An extra cleanup wait breaks that bound. Keeping the allocation free may then be the usable choice. Separately retain the cost of restarting the auxiliary computation and any external actions that its earlier execution already caused.

## OPS.8.2:6 - Bias-Annotation {#bias-annotation}

A utilization display makes idle time conspicuous while the protection it supplies may be invisible. Conversely, a label such as “reserve” can discourage useful work even when its full return fits the service requirement.

A successful short return can hide later costs. Repeated interruption may waste auxiliary progress, exhaust a person or occupy supporting resources. Judge the arrangement at the receiving service and the intended auxiliary result, rather than by occupied minutes alone.

The numerical cases are constructed timing comparisons. They establish conditional consequences, not measured interruption times for people, machines or AI systems.

## OPS.8.2:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Mistake | What fails | Repair |
| --- | --- | --- |
| Filling every idle interval | Protection disappears when the call arrives. | Recover the protected service and fit the whole return before promising the interval. |
| Treating priority as interruptibility | An indivisible operation or retained allocation prevents recall. | Identify the actual stopping and resource-release mechanism. |
| Ending the calculation at “paused” | Travel, cleanup or restoration delays readiness. | Calculate through the first ready protected action. |
| Fitting duration without fitting calendars | A needed setter or handover participant is unavailable. | Place return operations with their required resources. |
| Treating an easy-to-stop lesson as capability gained | An operating fit substitutes for practice and transfer. | Retain HCD's learning and capability question separately. |
| Counting only the first successful return | Repeated transitions damage auxiliary progress or sustained service. | Compare the whole relevant operating interval and its actual burden. |

## OPS.8.2:10 - Architectural Rationale {#architectural-rationale}

Protective capacity is useful through the work it can perform when needed. Its availability depends on capability, timing, location, access and state. The same idle machine or person can therefore be available for one protected service and unavailable for another.

The auxiliary unit, its interruption and the restoration form one operating construction. Keeping them together prevents an attractive auxiliary result from hiding the work needed to resume service. Preserving the auxiliary state and restoring the protected state remain separate contributions.

The method uses ordinary scheduling and capacity comparisons for the return. Its particular contribution is selecting and operating auxiliary work around that return, including the effects that remain after interruption. The comparison retains both the encompassing service and the smaller actions through which availability is restored.

## OPS.8.2:11 - SoTA-Echoing {#sota-echoing}

The selected approach compares a complete return with the protected service, then evaluates the auxiliary contribution and its burden. Simpler alternatives remain useful: keep the resource ready, or use only capacity established as excess to protection. Temporarily occupying protective capacity needs the additional construction in sections 4.2–4.5.

Steve Tendon, *The Book of TameFlow* (2022), printed pp. 226–229, distinguishes productive, protective and excess capacity and uses excess capacity for preparation and development. Adopt that distinction. Applying it to temporary use of the reserve adds an explicit interruption and restoration construction; the source's use of excess capacity does not itself establish that permission. Its fixed-expense argument also leaves transition burden, consumables, lost alternatives and changed service consequences to the receiving comparison.

Hopp and Spearman, *Factory Physics*, third edition, §4.4.3 and §§7.4.2–7.4.3, supplies two useful constructions: move eligible preparation outside machine downtime, and use already-capable workers where work needs them. The simple worker-transfer equivalence assumes no handoff delay. Adapt preparation and transfer to the actual return calendars in 4.2–4.3; training and zero-time handover cannot silently replace present operating capability.

[Van Zoonen and Scharp, *Managing Daily Work Intrusions* (2025)](https://doi.org/10.1037/str0000362), describes a ready-to-resume planning intervention. Adopt the small state-and-continuation aid when it reduces reconstruction. Their field study reports reduced attention residue alongside increased general exhaustion, so include the intervention's burden and do not infer a universal response-time benefit. Sections 4.2 and 4.4 keep those two effects in the choice.

The Slurm documentation makes computational resource release concrete: [suspension](https://slurm.schedmd.com/preempt.html) can retain memory and licenses, and [generic resources](https://slurm.schedmd.com/gres.html) remain allocated to suspended jobs. [Requeueing](https://slurm.schedmd.com/sbatch.html) restarts the batch script, so application recovery must be supplied separately. [Backfill scheduling](https://slurm.schedmd.com/sched_config.html) protects expected starts using runtime limits; that is a different timing requirement from an unknown call. [Prolog and epilog behavior](https://slurm.schedmd.com/prolog_epilog.html) adds real preparation, cleanup and failure conditions. Adapt these mechanisms to the selected configuration rather than inferring released capacity from a generic pause command.

Reopen the arrangement when a different auxiliary unit or return mechanism improves useful service at acceptable cost, or when call timing, allocations, interruption behavior or restoration changes.


## OPS.8.2:End {#end}
