# Spacialize: problem and value validation plan

Date: 29 September 2026. Status: proposed research, not completed validation.

## 1. The decision we need to make

Determine whether people with multiple recurring work responsibilities experience a costly, frequent problem that a persistent domain workspace can solve, and whether a spatial map adds enough value to justify its complexity.

The founder's experience supplies a concrete starting case: an IT professional responsible for project management, consulting, service management, and support, working across many browser tabs, notes, sheets, Gmail, and Google Chat. The proposed environment groups these resources by responsibility. Support Management and Project Management are large regions; Observability is a subregion containing tools and related notes. Zooming changes the level of detail, from domain summaries to working resources.

This changes the initial emphasis from exploratory research to recurring operational work. The [earlier market analysis](../Market_analysis/Research/browser-navigation-market-analysis.md) offers adjacent evidence, but does not validate this more specific problem or audience.

Known today: one detailed founder account, supporting browser-management research, and competing approaches. Unknown: how broadly the same problem occurs, its actual cost, the best alternative, sustained use, and willingness or ability to pay. No interviews, experiments, or commercial commitments described below have yet occurred.

## 2. Value proposition and hypotheses

Provisional proposition:

> For people managing several recurring responsibilities, Spacialize keeps the tools, working materials, and next steps for each responsibility together, so they can enter a work area ready to act and return without rebuilding context.

An operational overview may become a second promise: see which areas need attention and why. Shared workspaces and handover may become further benefits. Each requires separate evidence. The map is a proposed interaction mechanism; it is not yet a demonstrated reason to buy.

| Candidate value | Observable problem | Hypothesis | Test |
| --- | --- | --- | --- |
| Enter a responsibility ready to work | Repeatedly locating the right project, filtered app view, document, and conversation | A persistent workspace reduces preparation and search | Observe current work; compare current setup with domain workspace |
| Resume after an interruption | Re-reading notes and messages to reconstruct the last decision and next action | Preserving working context reduces resumption cost | Delayed resumption tasks and field diary |
| Know what requires attention | Visiting several tools merely to establish current state | Useful summaries improve prioritization accuracy and speed | Same task with and without summaries in the same layout |
| Navigate through stable locations | Losing track of where resources belong across responsibilities | Spatial arrangement improves retrieval and orientation beyond a list/tree | Matched conventional and map interfaces |
| Hand over a work area | Explaining scattered resources and rationale to another person | Sharing context reduces handover effort | Later research only if interview evidence supports it |

Keep competing explanations open. The dominant problem may be excessive workload, unclear ownership, missing access, unreliable source data, or notification volume. Rearranging applications may have little effect on those causes.

## 3. Target participants and a narrow first workflow

Initial audience: IT professionals who personally operate across at least two recurring responsibilities and use several applications in each. Job titles can include service managers, project managers, consultants, and operations leads, but recruitment should establish actual activities.

Start with 12 discovery participants across at least three teams or organizations if accessible. Include people satisfied with their current setup, people using saved groups or dashboards, and people who abandoned an organizer. Seek at least four participants with an established organizational method. Do not screen only for complaints, high tab counts, enthusiasm for maps, or similarity to the founder.

The founder participates in a rehearsal and diary, excluded from the external participant counts. If everyone comes from one employer, label the findings organization-specific until replicated elsewhere. Accommodate keyboard users and different display sizes; do not recruit only large-monitor or whiteboard enthusiasts.

Initial test workflow, subject to discovery:

> Move from a project review into support work, locate the relevant service context, determine the next action, then return to the interrupted project with its context intact.

This requires two domains. A single-domain demo can test navigation, but cannot test the central domain-switching claim. Use only enough subdomains and resources to reproduce observed complexity.

## 4. Sequence, effort, and gates

Indicative schedule: six weeks if recruitment is available and prototypes stay small. Timing is a planning assumption, not a delivery commitment. Recruit in parallel with preparation. Budget roughly 8-12 researcher-days across preparation, sessions, and analysis, plus participant incentives and a separately capped prototype effort. A second observer is useful but optional. Additional integration development is a separate decision.

The numeric gates below are proposed investment rules for a small exploratory sample, not scientific standards or estimates of market prevalence. Agree them before seeing results. Report every participant and exception; crossing a gate permits the next experiment, not a claim of product-market fit.

| Stage | Timing | Work | Decision enabled |
| --- | --- | --- | --- |
| Understand the problem | Weeks 1-2 | 12 interviews with demonstrations; five-day diaries from six participants | Which recurring problem, for whom, is worth addressing? |
| Test organizing by responsibility | Week 3 | Six participants try a conventional domain workspace for five working days | Does keeping work context together help enough to continue? |
| Test the spatial contribution | Week 4 | 12 participants compare matched conventional and map interfaces, including delayed return | Does spatial interaction improve the selected outcome? |
| Test sustained value and adoption | Weeks 5-6 | Six participants use the strongest version for ten working days; discuss buying and deployment | Is there enough repeated value and feasible adoption to justify an MVP? |

Advance only when the previous stage supports the hypothesis. If conventional organization helps but the map does not, continue with the useful workspace and reconsider the map. If discovery identifies a different problem, rewrite subsequent tasks and gates before testing.

## 5. Stage one: establish the problem before showing the idea

### Recruitment screener

1. What recurring responsibilities did you personally handle in the last working week?
2. Which applications or materials did you use for each?
3. How often did you move between those responsibilities?
4. How do you currently keep that work organized? How well does it work?
5. Can you demonstrate a recent task using a redacted example or representative materials?

Recruitment message, ready for the founder to use:

> I am researching how IT professionals organize work across several responsibilities and applications. I would like to observe how you switch between two areas of work in a 45-minute session. People who are happy with their current setup are just as useful as those experiencing difficulties. You can use redacted examples; this is research, not a product demo.

No invitations have been sent as part of preparing this plan.

### A 45-minute interview and observation

| Minutes | Activity | Prompts |
| --- | --- | --- |
| 0-5 | Establish the work context | Which responsibilities did you handle yesterday? Which needed most coordination? |
| 5-20 | Reconstruct a recent switch | Show me the last time you stopped one responsibility to handle another. What triggered it? What did you open, search for, or reread? |
| 20-30 | Observe return to unfinished work | Show me something you left unfinished. How do you find the right materials and decide what to do next? |
| 30-38 | Investigate consequences and alternatives | What was delayed, repeated, missed, or frustrating? What have you tried? Why did it work or fail? When is this easy? |
| 38-45 | Test importance and adoption constraints | Which part would you most want improved? What would you give up or change to fix it? Who controls whether you can use another tool? |

Ask for recent examples and demonstrations. Record whether each claim was observed, recalled, or inferred. Do not introduce countries, maps, zooming, or the product until the problem session is complete. Avoid questions such as “Would an organized canvas help?” or “Would you use this?”

For each incident, distinguish finding a tool, finding the correct state within a tool, reconstructing reasoning, checking status, and waiting on people or access. Count only costs the proposed product could plausibly affect.

### Five-day diary for six participants

Capture the first three qualifying switches each day plus consequential failures, including successful switches with no friction. Log the number of other switches or mark it unknown; do not extrapolate sampled time to the whole day without a denominator.

Fields: participant ID; date; from/to responsibility; trigger; goal; materials needed; steps taken; approximate preparation time; observed versus estimated timing; difficulty 1-7; consequence; workaround; whether the same issue has occurred before. Include a short daily entry for maintenance time and “no qualifying activity” days.

Keep actual customer records, message contents, credentials, and raw recordings outside this Git repository. The study needs workflow evidence, not copies of company data. Obtain participant agreement for any recording.

### Gate one

Provisional proceed signal: at least 8 of 12 participants provide a recent concrete example of the same addressable problem, and at least 4 of 6 diarists show recurrence on three or more days with either roughly five minutes of addressable friction per sampled day or a specific material consequence. Record time and consequence routes separately; never convert a consequential error into invented minutes.

Also require an identifiable segment and evidence that current workarounds leave a meaningful gap. Complaints about having many tabs do not meet this gate by themselves. If needs split into unrelated problems, narrow recruitment and investigate again. If preparation is already quick and reliable, deprioritize this promise.

Output: a one-paragraph problem statement, an evidence table, baseline measurements, and a ranked list of jobs to improve. Proposed form: “When [trigger], [specific users] struggle to [job], causing [observed consequence], despite using [current workaround].”

## 6. Stage two: test a domain workspace with familiar navigation

Build the cheapest useful version: a page or lightweight shell with named domains, nested sections, links to the correct app views, notes, and a place for the next action. Use a tool the participant already knows where practical. Preserve their existing applications and normal sign-in. Do not depend on full in-canvas browsing to test organization.

Six participants use it for five working days. Let participants choose their own labels. Measure and record researcher-assisted setup separately; then observe a participant adding or changing a resource without help. Permit the same document or tool to appear in multiple domains: real work may not fit a strict tree.

Compare their repeated workflows with the stage-one baseline. Track qualifying opportunities, preparation/resumption time, successful completion, upkeep, and whether the participant chooses to use the workspace. Before/after results are directional: learning, workload, and project changes can also explain differences.

Gate two: at least 4 of 6 participants voluntarily reuse the workspace on at least three eligible days, demonstrate a repeated useful outcome, and maintain it without the researcher doing the ongoing organization. As a provisional economic check, setup should plausibly be repaid within ten working days and observed ongoing time saved should exceed upkeep. Report the assumptions behind that estimate; include failed and abandoned setups.

If it works, we have preliminary evidence for responsibility-based organization. It does not establish a need for a new browser or map. If only manual status summaries help, focus the next experiment on summaries.

## 7. Stage three: isolate spatial navigation

### Conditions

- **A: current practice.** The participant's existing browser, groups, search, shortcuts, notes, and dashboards, used as competently as they normally use them.
- **B: conventional domain workspace.** A sidebar or tree with domains and subdomains, a detail panel, persistent resources, notes, and next actions.
- **C: map workspace.** The same domains, resources, notes, and next actions with stable regions and semantic zoom.

A supplies a realistic baseline from prior stages. The controlled comparison is B versus C. Match content, data freshness, search, links, persistence, screen size, task complexity, and available summaries. B must expose the same levels of detail by clicking/drilling down that C exposes through zooming. Neither gets exclusive features or cleaner data.

This comparison tests the combined spatial interaction design. It does not isolate the effects of animation, spatial memory, and zoom separately; follow-up experiments can do that if needed.

### Sessions and tasks

Use 12 target users for a directional study, preferably including some who were not in earlier rounds. Balance B-first and C-first order, six each. Provide equal training to a basic competence check. Use equivalent but different datasets, and balance dataset assignment across interfaces so one task is not always easier. Avoid reusing the exact answers across conditions.

Conduct a 45-60-minute first session and a 20-30-minute return session 24-48 hours later. Use think-aloud in exploratory practice, then quiet timed trials followed by retrospective questions, so narration does not distort the timing comparison.

| Task | Participant goal | Successful outcome |
| --- | --- | --- |
| Enter support work | An issue arrives for a particular service; prepare to assess it | Correct service view, relevant runbook, and related discussion located |
| Switch to project work | A sponsor asks about a milestone while support work is unfinished | Correct milestone material and next step identified |
| Return after a delay | Continue the interrupted support task | Correct context recovered and the correct next action begun |
| Find a shared resource | Locate a contact or document relevant to both domains | Resource found without duplicate conflicting information |
| Maintain the workspace | Add a new service and move an outdated resource | Working organization updated without facilitator help |

Choose one primary task outcome before running the study, using discovery evidence. If resumption is primary, time from the task cue to the first correct work action, not the first click or app opening. Define the correct action and timeout in advance. Record unfinished trials as failures rather than discarding them from the timing results.

Measure correctness, completion, wrong-region visits, facilitator interventions, setup/upkeep, and reported effort alongside speed. Ask users what they relied on: location, text search, labels, remembered content, or shortcuts. Include a keyboard path and test realistic laptop use. Do not force panning if search is their natural choice.

### Gate three

Provisional spatial proceed signal: a median within-person improvement of at least 20% in the preselected timed outcome for C versus B, at least 8 of 12 participants improving, and no material loss in completion, correctness, or maintenance effort. Compare relative improvements per participant; report absolute seconds as well. Tiny absolute savings may not justify new interaction costs.

At this sample size, this is a decision signal, not a statistically established population effect. Show the individual paired results, ranges, errors, and negative cases. If results are mixed, iterate or expand the sample based on observed variability before asserting superiority. If B matches C, prefer the simpler design unless another preselected outcome shows a worthwhile benefit.

### Separate test for operational summaries

If overview and prioritization emerge as a major job, compare the same layout with and without summaries using matched scenarios. Require participants to identify what needs attention and explain the evidence. Measure correct priorities, missed urgent items, and time, including a stale-data scenario.

Use clearly labeled simulated data in early sessions. A useful fictional counter does not establish that live data can be obtained reliably. If summaries are essential, later pilot at least one real source and record freshness and failed updates. Keep this value separate from the map result.

## 8. Stage four: test repeated use, economics, and feasibility

Six participants use the strongest version for ten working days. The first week can include onboarding support; the second should not depend on reminders to use the product. Log assistance and distinguish organized test tasks from voluntary work. Compensate research participation consistently, not positive feedback or frequent usage.

Count use per opportunity: someone handling support only twice a week should not fail a daily-usage target. Track resources added or changed, actual resumed tasks, maintenance, fallback to the old setup, failures, and requests to continue. Include time spent opening external apps or restoring state; do not time only navigation within the prototype.

Gate four: at least 4 of 6 participants choose the product for at least half their qualifying opportunities in the second week and can demonstrate a repeated outcome whose benefit exceeds upkeep. At least three choose to continue with a concrete next step, such as bringing another real domain into the workspace. Interview dropouts; do not replace them silently with enthusiasts.

Validate buying separately. Identify whether the user pays personally or an employer buys it. Discuss the existing budget and purchasing path with at least three relevant budget holders or self-paying users. Present an explicit offer with scope and price chosen after learning the alternatives and value; do not invent a willingness-to-pay estimate from compliments. Seek a paid trial or a specific documented budget-holder commitment. Unpaid pilot interest is weaker evidence and leaves revenue validation open. No offers, payments, or outreach are executed by this document.

Check the smallest necessary technical path against the actual apps participants use: launch links, saved filtered views, persistence after restart, authenticated session behavior, and data access for essential summaries. Investigate embedding only if working within the map is necessary for the benefit. Confirm whether installation and required permissions are feasible for the intended users. A click-through prototype cannot settle these questions.

A ten-day pilot is an early adoption signal. Require a longer paid pilot before claiming durable retention or scaling the product.

## 9. Evidence and decision records

Use this record for each finding. Keep participant names and company-sensitive materials outside the repository; aggregate summaries can live here.

| ID | Hypothesis | Participant/cohort | Trigger and job | Observed / recalled / inferred | Evidence and consequence | Counterexample | Next decision |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Example structure only | Resumption is costly | P01 | Return to an interrupted incident | To be recorded | To be recorded | To be recorded | To be recorded |

At each gate, write: what was tested; sample and recruitment limitations; what happened; evidence against the hypothesis; threshold result; unresolved questions; and the next investment authorized by the findings. Date any changes to the hypothesis or threshold and explain why before running the next round.

| Result | Product direction |
| --- | --- |
| No recurring consequential problem | Stop this proposition or investigate a different segment |
| Pain is real, existing setup solves it cheaply | Offer configuration or workflow help; reassess need for a standalone product |
| Domain workspace helps; map adds little | Develop the domain workspace with conventional navigation |
| Map adds value; summaries add little | Focus on context and navigation; defer integrations |
| Summaries help; map adds little | Explore an operational overview with direct access to work |
| Short tests succeed; field use fades | Investigate upkeep, novelty, and switching costs before adding features |
| Value is sustained; buying or deployment is blocked | Reconsider delivery model or target customer before scaling |
| Repeated value, feasible delivery, credible buying commitment | Specify a narrow MVP and a longer paid pilot |

## 10. First actions

1. Use the founder's own two-domain workday to rehearse the observation and diary. List actual tools, recurring switches, and what must remain in context. Do not treat this as independent validation.
2. Recruit the first four external participants with different existing organizational habits. Complete their problem sessions before showing the map.
3. Review those findings, adjust prompts without retroactively changing recorded evidence, and recruit the remaining eight plus diary participants.
4. Decide whether gate one supports a specific problem statement before investing in either interface prototype.

Immediate deliverables from this plan are the recruitment text, screener, interview guide, diary fields, experiment design, and gate criteria. The next evidence must come from observed work.

## Method references

The sequencing follows a standard separation between discovering user needs and evaluating a proposed solution. GOV.UK's [discovery research guidance](https://www.gov.uk/service-manual/user-research/user-research-in-discovery) emphasizes current activities, tools, observations, and frustrations. Its [moderated testing guidance](https://www.gov.uk/service-manual/user-research/using-moderated-usability-testing) supports realistic tasks with clear goals that do not reveal the intended navigation. Its [discovery-phase guidance](https://www.gov.uk/service-manual/agile-delivery/how-the-discovery-phase-works) treats a decision to stop as a valid result.

These references support the approach, not the proposed sample sizes, schedule, numerical gates, or a claim that Spacialize works. Those are explicit planning choices to revise before data collection as access, baseline costs, and task variability become known. Sources checked 29 September 2026.
