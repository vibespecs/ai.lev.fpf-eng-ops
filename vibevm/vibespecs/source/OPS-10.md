# OPS.10 - Qualify Operating Capacity Under Variability: depth {#depth}

<status stage="spec" state="done"/>

> Source: Anatoly Levenchuk, *Operations Management Principles Framework* (20 September 2026), `Engineering DPF Suite/OPERATIONS-MANAGEMENT-PRINCIPLES-FRAMEWORK.md` at https://github.com/ailev/FPF commit d131d30a44e7, licensed CC BY 4.0. Depth sections of the pattern; the working sections are in the contract document of the same id. See LICENSE.md for the list of changes.

## OPS.10:5 - Archetypal Grounding {#archetypal-grounding}

### OPS.10:5.1 - PumpWorks: fit, reserve and a deferred package {#pumpworks-fit-reserve-and-a-deferred-package}

In this constructed extension, four eligible test packages each require two consecutive rig-hours, including their normal setup, under the current estimate. In the next eight-hour horizon, this operation has access during hours 0–6; hours 6–8 are currently reserved for another use. This gives six continuous usable rig-hours. Permission and required configuration for the tests are current; release authority and SafetyQuestion-S19 remain separate.

The initial load is eight rig-hours, so all four packages cannot fit the six usable hours even before uncertain recovery. More ready packages or a larger buffer cannot remove that deficit.

For comparison, assume one adverse scenario: one of the planned packages needs a single consecutive two-hour repeat, after which it passes. The failed attempt is identified on completion and its repeat can run next under the current test conditions. This is a supplied scenario, not an estimated failure probability. The resource owner can offer hours 6–8 to this operation through a separate access and cost decision that accounts for the displaced use.

| Option | Usable rig-hours | Planned packages | Explicit reserve | Accepted test packages without repeat | Accepted packages in the one-repeat scenario |
| --- | ---: | ---: | ---: | ---: | ---: |
| current access, plan three | 6 | 3 | 0 | 3 | 2, with unfinished load returned |
| extra access, plan three | 8 | 3 | 2 | 3 | 3 |
| extra access, plan four | 8 | 4 | 0 | 4 | 3, with unfinished load returned |

If the operating decision requires three completed packages in both stated scenarios, the second option supports that comparison; the first does not. If the decision instead values four nominal completions and can accept the stated adverse shortfall, the third is a different choice. Cost, permission and affected commitments remain explicit rather than being hidden in “maximum utilization.”

The first useful return can therefore be: obtain the authorized extra access, admit three packages for this plan, reserve two hours for the named repeat scenario, and return the fourth package to OPS.5 and any affected existing commitment to OPS.7. If the extra access is not obtained, use the six-hour result instead.

No probability or release guarantee is claimed. More than one repeat, a longer repeat, changed configuration or another loss reopens the comparison. A passed test package still does not settle the release decision for R42.

### OPS.10:5.2 - Equal total load, different waiting {#equal-total-load-different-waiting}

One continuously available server processes four one-hour jobs. There is no setup, failure, other resource or initial backlog.

| Scenario | Arrival times in hours | Start times | Waiting times |
| --- | --- | --- | --- |
| one burst | 0, 0, 0, 0 | 0, 1, 2, 3 | 0, 1, 2, 3 |
| one job per hour | 0, 1, 2, 3 | 0, 1, 2, 3 | 0, 0, 0, 0 |

Both consume four server-hours and finish the last job at hour 4. If the criterion is completion within two hours of arrival, two of four jobs meet it in the burst scenario and all four in the second. The difference follows from the stated arrival scenarios, not from shifting the measurement origin or claiming a forward probability.

This result tells the practitioner why total hours alone cannot settle service. It does not authorize delaying already arrived demand and then starting its clock later.

### OPS.10:5.3 - Nominal beds and qualified capacity {#nominal-beds-and-qualified-capacity}

A hospital's bed count is not the capacity for every care requirement. The receiving question may depend on the supplied clinical class, staffing qualification, equipment, cleaning readiness, access and synchronized availability.

OPS.10 can compare operating arrangements from those qualified inputs and state a resource-time or scenario result. If the clinical eligibility or staffing Method is missing, it returns that exact input. It does not invent a clinical staffing ratio or treat every empty bed as usable service capacity.

## OPS.10:6 - Bias-Annotation {#bias-annotation}

| Bias | Consequence | Countermeasure |
| --- | --- | --- |
| nominal-capacity bias | Calendar presence substitutes for usable capability and access. | Recover the relevant service and resource conditions. |
| average sufficiency | Equal totals are treated as equal service. | Inspect arrival timing, variation and the actual service criterion. |
| double-counted loss | A failure is included in service time and again deducted from capacity. | State each estimate's contents and count the effect once. |
| precise-number confidence | A sophisticated model hides poor premises. | Match model scope to the question and qualify the result kind. |
| reserve-as-waste bias | Recovery capacity is removed to increase utilization. | Compare the named disturbance and service consequence. |

## OPS.10:8 - Common Anti-Patterns and How to Avoid Them {#common-anti-patterns-and-how-to-avoid-them}

| Anti-pattern | Failure | Repair |
| --- | --- | --- |
| Total demand is below total hours, so the deadline is safe. | Timing, precedence or incompatible capability can prevent a schedule. | Recover the actual resource windows and a feasible witness. |
| Use mean utilization as a service guarantee. | The wait distribution and relevant tail remain unknown. | State the intended service criterion and select a suitable analysis. |
| Treat a scenario as a probability. | No occurrence model or calibrated data supplies that probability. | Label the conditional result and return the missing probabilistic basis. |
| Treat every person or machine-hour as interchangeable. | Capability, configuration and access differ. | Compare usable service capacity by the relevant class. |
| Count repeats as additional delivered results. | Attempts and accepted outputs have different identities. | Keep load and result populations separate. |
| Buy capacity before establishing the limiting mechanism. | The added resource may not change completion. | Use OPS.9 where the treatment basis is unresolved. |

## OPS.10:10 - Rationale {#rationale}

Usable capacity, workload and service are related but different. A load bound answers whether enough required resource time exists. A schedule answers whether that time can be used as needed. A service forecast adds a claim about uncertain outcomes. Keeping these questions separate prevents a cheap answer to one from being mistaken for an answer to all three.

## OPS.10:11 - SoTA-Echoing {#sota-echoing}

| Practice question and selected line | Serious alternative, trade-off and pattern change | Source roles, limits and reopen condition |
| --- | --- | --- |
| Can average population and flow data establish timely service? **Adopt** compatible population accounting; **reject** using a mean identity as a tail guarantee. | Mean utilization cannot distinguish the two arrival scenarios in 5.2. A mean-flow identity can recover different mean times from compatible population data, but does not establish their two-hour completion fractions. Sections 4.1, 4.3 and 4.5 retain the service criterion and result kind. | [Little (2011)](https://doi.org/10.1287/opre.1110.0940) supplies the mature mean-relation basis, not a deadline model. The finite example provides the decision-changing contrast at comparable calculation effort. Reopen when the population, boundary, returns or required service claim changes. |
| What model should handle dependent arrivals and feedback? **Adapt** model selection to the actual temporal and network dependence. | A simple independent-input mean approximation is easier but can omit consequential burst structure. Sections 4.3–4.5 call for a suitable specialist model only when that omission can reverse the decision. | [Whitt and You (2022)](https://doi.org/10.1002/nav.22010) is a bounded model candidate: a single-class open single-server network with Markovian routing, nonrenewal arrivals and feedback, estimating mean steady-state performance through dispersion functions. It does not supply every service tail or transient solution. Reopen for nonmatching routing, classes, regime or service criterion. |
| Should the response be more capacity, pooling, or a different batch policy? **Adapt** finite comparison of setup, waiting, reliability and service effects. | Capacity additions can be lumpy; smaller batches and pooling can have different protected consequences. Sections 4.2–4.4 and 5.1 retain those costs and scenarios rather than selecting a universal utilization or pooling rule. | Reinertsen (2009), batch-size trade-offs, supplies a mechanism candidate. [Andradóttir et al. (2017)](https://doi.org/10.1016/j.ejor.2016.05.009) and [Cao et al. (2021)](https://doi.org/10.1287/opre.2019.1976) supply conditional pooling counterexamples. Their studied conditions are not transferable staffing or rig prescriptions. Reopen when capability, failures, batching or the service criterion changes. |


## OPS.10:End {#end}
