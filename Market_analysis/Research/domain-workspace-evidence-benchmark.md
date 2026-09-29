# Spacialize: evidence benchmark for a workspace organized by responsibility

Research date: 29 September 2026. Secondary research; no new participants, outreach, product installations, or performance tests.

## Decision

**There is enough existing evidence to justify a small prototype without making interviews the next dependency. There is not enough evidence to claim that a zoomable spatial browser is the winning solution.**

The strongest supported direction is preserving the context of an activity across applications: its working materials, relevant views, and reminders. Spatial navigation is a separate hypothesis with encouraging precedents and meaningful counterexamples. An operational overview is another separate hypothesis; its usefulness depends on the information it contains and its accuracy.

For Spacialize, the recommended first job is:

> When I move between support management and project management, help me recover the right working context and next action without reconstructing them across scattered tools.

This is an evidence-informed problem statement, not a measured market-size or revenue claim. It is narrower than replacing the browser, building a complete digital workplace, or solving information overload generally.

This report updates the direction in the [initial market analysis](browser-navigation-market-analysis.md) and the sequence in the [validation plan](../../Product_discovery/validation-plan.md).

## 1. Scope and method

This is a targeted scoping review, not a systematic review or meta-analysis. Searches covered browser overload, application switching, task resumption, activity-based computing, virtual desktops, spatial document retrieval, zoomable interfaces, and first-person accounts from IT managers, project managers, and consultants. Product searches covered existing workspace browsers and canvas tools. Both supportive and adverse findings were retained.

The retained evidence comprises nine research papers, six public discussion threads, two practitioner/research essays, five product capability pages, and three additional sources covering a usability issue, a discontinued feature, and industry telemetry. Older studies explain mechanisms and historical attempts; current documentation establishes available alternatives. The existing market analysis contains additional browser-specific research.

Evidence was treated differently by source:

- **Research:** methods, findings, and limitations from accessible paper sections or primary institutional abstracts. Abstract-only access is identified below.
- **Public accounts:** volunteered experiences that help identify triggers and workarounds. Identities, outcomes, and representativeness were not independently verified. Comments in one thread are not independent studies.
- **Product documentation:** evidence of advertised capabilities, not proof of effectiveness, adoption, or commercial success. No comparative product scores were invented.
- **Our synthesis:** product implications and proposed experiments, explicitly separated from reported results.

Searches are biased toward English-language, publicly indexed material. Complaint forums overrepresent dissatisfied users and may contain promotion. No counts of posts, votes, or search hits are used to estimate prevalence. Four discussion sources below were examined through indexed excerpts rather than full-page retrieval. Their summaries are limited to that visible material. Research samples do not directly represent Portuguese enterprise IT management; their participant counts must not be added into a market survey.

## 2. Research that already performs part of the discovery work

| Study | Method and population | Finding relevant to Spacialize | What it does not establish |
| --- | --- | --- | --- |
| [R1. Managing Multiple Working Spheres, CHI 2004][r1] | Observation and interviews with 14 information workers, including managers, analysts, and developers; three formal observation days per person after acclimatization. Full-text methods and findings reviewed. | Work is organized around several broader responsibilities and recurring activities, with frequent movement among them. Workers maintain representations of their work outside individual applications. | Frequency in today's target market, or the amount of switching that an interface could eliminate. A change of event or tool is not necessarily a change of responsibility. |
| [R2. Task-Centric Application Switching, GI 2023][r2] | Interviews with 15 knowledge workers and five product teams. Primary institutional abstract reviewed. | People deliberately use several applications even within one task. Collaboration, tools, and workflow constraints help explain switching. | That switching is inherently wasteful, or that placing apps together removes data conversion, permissions, or coordination costs. |
| [R3. Dedicated Workspaces, 2016][r3] | Experiment with 16 participants: a Windows 7 desktop versus dedicated virtual desktops for independent tasks. Institutional abstract reviewed; full text was not accessible through the research browser. | Task resumption averaged 10 seconds faster with dedicated workspaces; cognitive load was lower. In that experiment, most users recovered setup cost after three returns to suspended tasks. | An expected saving for Spacialize, superiority over today's saved workspaces, or any benefit specifically caused by a spatial map. |
| [R4. Giornata, CHI 2009][r4] | Five Mac users from an academic/HCI network; average use 54 days, range 22–82. Logs and interviews. Full-text methods and findings reviewed. | Activity-specific storage was valued. People used activities as working places and temporary holding areas. Resources and running apps also needed to cross activity boundaries. | Population-level productivity gains. Small, selected sample, no randomized comparison, and one missing final interview. |
| [R5. Lotus Activities, CHI 2010][r5] | Workplace-tools survey and interviews with 22 users; system had been deployed for over two years in one large company. IBM abstract reviewed. | An activity-centric system could ease fragmentation for a particular kind of activity while working alongside other tools. | That one organizer can replace the whole tool ecosystem, or a general causal estimate of time saved. |
| [R6. Tabs.do, UIST 2021][r6] | One-week field deployment with 10 participants using their own computers. Full-text methods and findings reviewed. | Saving tabs as task bundles helped participants describe and resume their work. Different people favored reopening bundles versus individual tabs. | Self-reported time savings are not measured productivity. The difference in counts of tabs reopened via bundles versus individually was not statistically significant; that is not a test of resumption speed. |
| [R7. Data Mountain, UIST 1998][r7] | 32 experienced IE4 users stored and retrieved 100 pages; spatial thumbnail interfaces compared with Favorites. Full-text methods and findings reviewed. | The spatial interface showed retrieval advantages, supporting the plausibility of stable visual locations as retrieval cues. | A clean isolation of spatial layout from thumbnails, screen area, and other design differences. The viewpoint was fixed: users did not travel through an infinite canvas. |
| [R8. Scalable Fabric, AVI 2004][r8] | Spatial task groups with live windows; comparison against the Windows XP taskbar, plus a later 13-person field trial. Full-text evaluation reviewed. | Participants valued the approach, but the comparison found no significant task-time difference. The field trial exposed practical usability and performance problems. | That positive reactions to a spatial interface translate into faster work. The later field-trial sample should not be presented as the comparison sample. |
| [R9. Zoomable Interfaces With and Without an Overview, TOCHI 2002][r9] | 32 participants performed navigation and browsing tasks on two maps. Full-text study reviewed. | 80% preferred an overview, yet there was no correctness advantage and one map was faster without it. Preference and performance diverged. | That an overview is generally harmful, or that map navigation outperforms a list of workspaces. Both tested interfaces were zoomable maps. |

These studies already supply observations, interviews, field deployments, and controlled comparisons. We do not need to repeat basic discovery merely to establish that fragmented work and resumption difficulties exist. We still need local evidence before transferring their measured effects to this product.

### A quantitative benchmark with usable limits

The most directly relevant numerical reference is R3's **10-second resumption difference**. Treat it as a demonstration that the mechanism can matter, not as an estimate or minimum target for our product. R8's lack of a significant task-time difference and R9's preference/performance split are equally important benchmarks.

Do not turn industry headlines into a savings model. Microsoft's 2025 report is often summarized as 275 daily interruptions per worker. Its methodology specifies the **top 20% by received ping volume**, counts across a **24-hour day**, and excludes EU and education tenants. Pings are not observed cognitive task switches. This is context about communication intensity, not a baseline for this founder or a recoverable productivity budget. [Microsoft methodology][i1]

There is no defensible pooled effect size across these sources: they measure different tasks, interfaces, populations, and outcomes.

## 3. Public accounts resembling interview findings

The following are paraphrased evidence extracts, not fictional interview transcripts. The last column is our interpretation.

| Account and access | Trigger / reported difficulty | Current workaround or counterexample | Implication to examine |
| --- | --- | --- | --- |
| [F1. IT manager responsible for Network and Data Center][f1]. Original post and comments read. | Team operations work adequately in Jira, but the manager's own tasks arrive through email, chat, phone, and meetings. | Tried Obsidian, Microsoft To Do, and paper. Another commenter reports To Do plus regular triage works; a different commenter uses an XMind grid for projects, blockers, deadlines, and goals. | The gap can be personal coordination across systems even when the team already has a task tool. Both simple lists and spatial overviews are credible alternatives. |
| [F2. Project-related browsing and forgotten bookmarks][f2]. Indexed post and reply read; direct retrieval failed. | Research URLs lose visibility when filed in bookmarks; the author wants open tabs attached to a task or project. | A reply suggests pasting URLs into an existing task's comments. | Preserving the relationship between a resource and intended action may matter more than its screen coordinates. |
| [F3. Consultant juggling four or more clients][f3]. Indexed original post read; direct retrieval failed. | Overlapping timelines, administrative work, and follow-ups are difficult to track; the author describes overload and stress. | Writes things down and seeks task-management/process advice. | This is a relevant responsibility-management problem, but the account does not identify browser navigation as its cause. |
| [F4. Consultants' organization practices][f4]. Indexed thread read. | Changing priorities require managing what to do and where work can be performed. | Calendars, per-project sticky-note lists, and batching work requiring a client machine. Advice also includes delegation and reprioritization. | Existing tools and work practices may be sufficient. Some friction is caused by capacity and access constraints. |
| [F5. Agency with multiple clients and projects][f5]. Original post read. | The author wants visibility across all tasks without an overwhelming number of sheets, while retaining fast task entry. | Evaluating Smartsheet; the thread does not establish a successful resolution. | Global overview and local execution are distinct needs. A map is one possible presentation, not the requested outcome itself. |
| [F6. Wavebox work/personal link routing][f6]. Indexed user complaint and support reply read; direct retrieval failed. | A work document opened in the last-used personal group/space. The relationship between groups and spaces was confusing to the author. | Support describes link-routing rules. | Correct account/context routing and understandable grouping rules can matter as much as navigation speed. |

The closest match is F1: more than one recurring responsibility, an established organizational tool, and residual coordination work across channels. But it is one thread. It does not establish how many managers have this problem or how much they would pay to solve it.

The accounts support at least four distinct jobs: capture incoming commitments; recover working context; locate resources by activity; and assess priorities across activities. A browser workspace may address some more directly than others. Combining all four into a single promise would obscure what we need to test.

## 4. What blogs and design accounts add

[Tiago Forte's PARA essay][b1] distinguishes ongoing areas of responsibility from projects with an end state. This supplies useful design vocabulary: Support Management is an area; resolving a particular service issue is a task or project within it. It is a practitioner's method and commercial essay, not a controlled validation of the proposed UI.

[Ink & Switch's Capstone report][b2] is particularly close to the map metaphor. It describes research with creative professionals and a prototype combining mixed media, nested zoomable boards, and a persistent collection shelf. Its authors explicitly discuss spatial memory and Maps-like gestures. It demonstrates a relevant design exploration, while reporting interaction and implementation difficulties. Its creative research workflow differs from recurring IT operations, and the report supplies no comparable estimate of operational productivity.

Our inference: use domains as stable entry points, but allow temporary work, unfinished classification, and resources shared across domains. An empty inbox or temporary area should be usable before someone designs a complete map of their job.

## 5. Existing alternatives set a higher bar than ordinary tabs

Capabilities below were checked in public documentation on the research date. These are a **feature baseline**, not results from hands-on testing. Undocumented features are unknown, not assumed absent. Subscription, platform, and organization-policy restrictions still require checking for an actual pilot.

| Alternative | Documented approach | Benchmark it supplies |
| --- | --- | --- |
| [Workona][p1] | Named project spaces, saving/restoring tab sets, switching visible tabs, and related resources, notes, and tasks. | Can Spacialize improve on an already organized project context, including the cost of keeping it organized? |
| [Wavebox][p2] | Spaces for account isolation, groups for related apps/tabs, and persistent apps in each group's tab strip. | A particularly relevant comparator for someone operating several web apps across clients or responsibilities. “All my work apps together” is already available. |
| [Rambox][p3] | Brings apps and accounts into a managed work environment with workspaces. | App consolidation and account handling need to work reliably before a new navigation model matters. |
| [Vivaldi Workspaces][p4] | Named collections of tabs, with tab stacks and tiling usable within workspaces. | Compare against grouping and simultaneous visibility available in a conventional browser. |
| [Kosmik][p5] | Advertises a browser on an infinite canvas alongside notes, images, PDFs, and captured web material. | A canvas containing browsing and notes is not, by itself, differentiation. Its documented emphasis is creative/research work. |
| Existing browser + project note | A deliberately configured baseline: grouped links, a next-action note, search, and shortcuts. This is our proposed comparison setup, not an evaluated product claim. | Any advantage must exceed the benefit of simply spending time organizing today's tools. |

There is also a history of unsuccessful or limited adoption. Mozilla [removed Firefox Tab Groups/Panorama in 2016][p7], citing low use and a desire to focus its development resources. That establishes one adoption failure, not the cause of failure of every spatial interface. Historical products should not be listed as currently available competitors.

Spatial tools create their own retrieval problems. The [Concepts help center documents recovery after losing a drawing on an infinite canvas][p6]. This establishes a real supported failure mode, not its frequency. Spacialize should offer reliable home, search, and direct-jump controls from the beginning.

## 6. What can we consider established?

These confidence labels are qualitative judgments about the retained evidence, not statistical probabilities.

| Claim | Assessment today | Consequence |
| --- | --- | --- |
| Some knowledge workers struggle to manage fragmented resources and unfinished work across activities | Strong evidence of existence across studies and volunteered accounts | Stop treating the general problem's existence as the main uncertainty. Its prevalence and severity in our chosen segment remain unknown. |
| Keeping activity resources together can improve resumption | Moderate support, including a small controlled experiment and field accounts | A justified basis for a narrow prototype. |
| Recurring responsibilities are a useful organizing unit | Plausible and supported qualitatively, but work also follows projects, people, and temporary tasks | Offer flexible organization rather than impose a complete hierarchy. |
| Stable spatial locations improve retrieval | Some controlled support in constrained document tasks | Worth testing against equally informative conventional navigation. |
| Semantic zoom through countries and cities improves everyday IT management | Unestablished in the reviewed evidence | Treat as a specific experiment, not a validated feature requirement. |
| Domain counters improve operational decisions | Public demand for visibility, but no directly matching validation here | Test summary content and freshness separately from layout. |
| A new browser is necessary | Unestablished; existing products and simpler configurations cover substantial ground | Start with the smallest delivery mechanism that can preserve the needed context. |
| Users will adopt, obtain permission for, or pay for Spacialize | Unknown | Do not infer demand from complaints, competitor existence, or prototype enthusiasm. |

### Revised value proposition

> A persistent workspace for people managing several responsibilities, keeping each area's tools, working materials, and next steps ready to resume.

Potential additional value: understanding which areas need attention. The spatial map is a candidate way to access and understand that workspace. Neither that presentation nor shared collaboration needs to be included in the first product promise.

The likely initial audience is defined by behavior: repeatedly returning to two or more responsibilities that require several applications and unfinished context. An IT service/project manager is a concrete starting case. A job title or large tab count alone is insufficient evidence of need.

### Design implications to carry forward

1. **Save more than links.** Preserve the reason for a resource, the relevant view where possible, and the next action. Explicitly distinguish stored URLs from restored application state.
2. **Allow shared resources.** The same service, document, chat, or app may belong to several domains. Avoid forcing duplicate copies and competing versions of notes. R4 provides direct motivation.
3. **Make organization cheap.** Support temporary capture and later classification. Count setup and maintenance as product costs.
4. **Keep direct access available.** Search, keyboard navigation, recent work, and a home view must remain usable even if a map is present.
5. **Separate summaries from navigation.** A useful counter can help a dashboard just as much as a map. Credit its benefit to the correct component.
6. **Use task success as the outcome.** Opening the right window is only a step toward resuming the right work; fewer tabs or more zooming is not a productivity measure.

These are proposed requirements derived from the synthesis, not claims that a tested Spacialize implementation already meets them.

## 7. Next evidence without recruiting anyone

The desk research is sufficient for a bounded founder experiment. External interviews are deferred; they are not a gate for this next step. The experiment below is proposed, not performed.

### A. Define one realistic two-domain scenario

Use Support Management and Project Management, with a small representative set of actual resource types: service dashboard, ticket queue, project sheet, relevant conversation, working note, and next action. Include one resource shared across domains, one temporary item, and a return after a break or the following day. Use redacted or representative content wherever needed.

Record several ordinary switches before reorganizing anything. Separate time spent finding resources, reconstructing the next action, waiting for apps, and actually doing the work. A founder log measures this founder's situation; it does not estimate the market.

### B. Establish the best simple baseline

Configure the same materials as named workspaces with a compact note and direct links. Choose the existing browser setup or one of the documented workspace tools. Include time spent setting it up and maintaining it. If this removes the meaningful friction, that is a useful result: the problem may need configuration rather than a new product.

### C. Compare two matched representations

Only if friction remains, make a small conventional list/tree and a spatial map backed by the **same** domain/resource data. Give both the same labels, previews, search, next-action notes, and information freshness. Compare:

- Current setup versus conventional workspace: the value of organizing and preserving context.
- Conventional workspace versus map: the additional value or cost of spatial navigation.
- Same interface with versus without summaries: the separate value of operational overview, if pursued.

Do not give the map richer information and attribute the difference to location. Alternate order and use comparable task variants to reduce practice effects. Include keyboard use, a laptop-sized viewport, delayed return, and an unexpected shared resource. A founder comparison can expose bad designs and personal utility, but familiarity and preference prevent it from establishing a population effect.

### D. Keep a small result log

| Measure | Definition |
| --- | --- |
| Resumption time | From deciding to return to an activity to the first correct substantive action; include external navigation and loading. |
| Correctness / failures | Wrong account, wrong resource, missed next action, inability to complete, and fallbacks to the old workflow. Keep failed attempts in the report. |
| Orientation cost | Wrong region visits, unnecessary zoom/pan, and use of search or home to recover. |
| Organization cost | Setup minutes plus daily minutes capturing, sorting, moving, and repairing the workspace. |
| Reported effort | A consistent short effort rating after each comparable episode, reported separately from timed performance. |
| Repeat usefulness | Whether the workspace still helps after several returns and after its contents change. |

For a first pass, use a one-week time box and aim for several comparable returns under each usable condition; extend only if too few genuine opportunities occur. This is a proposed practical limit, not a scientifically powered study. Do not build a browser engine or broad integration platform to conduct it.

### E. Decide using net value

For time savings, use the following planning model:

`net minutes/day = qualifying returns/day × seconds saved/return ÷ 60 − upkeep minutes/day − setup minutes ÷ expected days of use`

Illustration only: 20 returns saving 10 seconds each yield 3 minutes 20 seconds before upkeep. Five minutes of daily organizing would outweigh that benefit even before setup. These inputs are hypothetical; the study's result is not a prediction for Spacialize. Other benefits, such as fewer errors, must be measured separately rather than invented to rescue a negative time result.

| Founder experiment result | Next decision |
| --- | --- |
| Existing workspace configuration solves the problem adequately | Document the working setup; reconsider the standalone product premise. |
| Preserved context helps, but the map adds cost or no worthwhile advantage | Continue only the context/workspace proposition; retain conventional navigation. |
| Map repeatedly improves the chosen outcome after upkeep, without worse correctness | Continue a narrow spatial prototype; broader adoption remains an open question. |
| Summaries help, but location does not | Explore an operational overview with direct access to work. |
| Neither representation reduces meaningful friction | Revisit whether workload, task capture, integration, or prioritization is the actual problem. |

Agree what constitutes a personally worthwhile saving before collecting results, and report absolute seconds and maintenance time rather than only percentages. This experiment can justify another small investment or stop an unhelpful direction. Claims about other users, retention, purchasing, and enterprise deployment remain deferred until there is evidence about those people and settings.

## Source register

All sources below were checked on 29 September 2026. Publication dates belong to the source, not the access date. Reddit relative timestamps and indexed dates can disagree; dates are not used to support trend claims. R1, R4, and R6–R9 were examined through full-text sections. R2, R3, and R5 rely on primary institutional abstracts. F2, F3, F4, and F6 rely on indexed public excerpts; the other retained web sources were directly accessible.

[r1]: https://www.ics.uci.edu/~gmark/CHI2004.pdf "Gonzalez and Mark: Managing Multiple Working Spheres, CHI 2004"
[r2]: https://www.research.autodesk.com/publications/task-centric-application-switching/ "Jahanlou et al.: Task-Centric Application Switching, GI 2023"
[r3]: https://pure.itu.dk/da/publications/dedicated-workspaces-faster-resumption-times-and-reduced-cognitiv/ "Jeuris and Bardram: Dedicated Workspaces, 2016"
[r4]: https://stephen.voida.com/uploads/Publications/Publications/voida-chi09a.pdf "Voida and Mynatt: Giornata field study, CHI 2009"
[r5]: https://research.ibm.com/publications/fitting-an-activity-centric-system-into-an-ecology-of-workplace-tools "Balakrishnan, Matthews, and Moran: Lotus Activities, CHI 2010"
[r6]: https://lxieyang.github.io/assets/files/pubs/tabsdo-uist-2021/tabsdo-uist-2021.pdf "Tabs.do: Task-Centric Browser Tab Management, UIST 2021"
[r7]: https://www.microsoft.com/en-us/research/wp-content/uploads/1998/01/p153-robertson.pdf "Robertson et al.: Data Mountain, UIST 1998"
[r8]: https://www.microsoft.com/en-us/research/wp-content/uploads/2004/01/avi2004-scalablefabric.pdf "Robertson et al.: Scalable Fabric, AVI 2004"
[r9]: https://hjemmesider.diku.dk/~kash/papers/TOCHI2002_hornbaek.pdf "Hornbaek, Bederson, and Plaisant: Zoomable Interfaces, TOCHI 2002"
[f1]: https://www.reddit.com/r/ITManagers/comments/1pozc48/toolsprocedures_for_your_own_tasks/ "ITManagers: tools and procedures for a manager's own tasks"
[f2]: https://www.reddit.com/r/projectmanagement/comments/16g0kcp "Projectmanagement: collecting open tabs into a project task"
[f3]: https://www.reddit.com/r/consulting/comments/r23c87 "Consulting: productivity advice for juggling clients"
[f4]: https://www.reddit.com/r/consulting/comments/10xuih8 "Consulting: practices for changing priorities"
[f5]: https://community.smartsheet.com/en/discussion/42061/managing-multiple-clients-tasks "Smartsheet Community: managing multiple clients and tasks"
[f6]: https://www.reddit.com/r/waveboxapp/comments/1nr8mta "Wavebox: enforce spaces and groups"
[b1]: https://fortelabs.com/blog/para/ "Tiago Forte: The PARA Method"
[b2]: https://www.inkandswitch.com/capstone/ "Ink and Switch: Capstone, a tablet for thinking"
[p1]: https://workona.com/help/tab-manager/ "Workona: Tab Manager documentation"
[p2]: https://wavebox.io/platform "Wavebox: platform, spaces, groups, and apps"
[p3]: https://rambox.app/how-it-works/ "Rambox: how it works"
[p4]: https://vivaldi.com/features/workspaces/ "Vivaldi: Workspaces"
[p5]: https://www.kosmik.app/blog/kosmik-browser "Kosmik: built-in canvas browser"
[p6]: https://tophatch.helpshift.com/hc/en/3-concepts/faq/133-i-lost-my-drawing-on-the-infinite-canvas-how-do-i-find-it-again/?p=android "Concepts: recovering a drawing lost on the infinite canvas"
[p7]: https://blog.mozilla.org/futurereleases/2016/03/08/discontinuing-rarely-used-firefox-features/ "Mozilla: discontinuing rarely used Firefox features, 2016"
[i1]: https://www.microsoft.com/en-us/worklab/work-trend-index/breaking-down-infinite-workday "Microsoft WorkLab: infinite workday report and methodology, 2025"
