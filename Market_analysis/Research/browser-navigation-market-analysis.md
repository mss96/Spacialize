# Browser navigation: user problems and attempted solutions

Research date: 29 September 2026. Initial desk research for Spacialize.

## Decision in brief

There is credible evidence of difficulty managing web-based work, especially research spread across sources and sessions. There is not yet sufficient evidence here that an infinite canvas improves productivity or that users will pay to replace their browser.

The promising proposition is **a persistent research workspace that helps people recover sources, reasoning, and next steps**. Spatial layout is one candidate mechanism. It must outperform tab groups, search, saved workspaces, and split views after accounting for time spent arranging the canvas.

The concept already has direct competitors. Differentiation cannot rest on movable live web pages, an infinite canvas, or adjacent notes alone.

## Scope and evidence quality

Focus: desktop knowledge work, navigation across pages, task switching, retrieval, and synthesis. This is a problem-and-competition assessment, not a market-size estimate or exhaustive product audit. Products were checked through public documentation; none was installed or benchmarked. Feature documentation demonstrates an attempted solution, not demonstrated productivity gains, adoption, or commercial success.

Evidence classes used below:

- **Research:** published studies with described methods. Samples remain limited and do not represent all browser users.
- **User report:** an individual account or feature request. Useful for discovering mechanisms, not estimating prevalence.
- **Vendor documentation:** evidence of advertised capabilities, subject to platform and version differences.
- **Hypothesis:** our interpretation or proposal requiring validation.

Repository inputs: `reddit-analyses.pdf` is a two-page screenshot of an AI-generated Reddit answer, explicitly marked as potentially inaccurate. Its themes are useful interview prompts, but its unattributed quotations and feature claims are not treated as verified evidence. Parts of its second page are obscured. `../Competitors_features/comp-features.png` shows Stack advertising multiplayer as “Coming soon”; this is not proof of a released feature. Both originals were preserved.

## 1. What problems do users report?

| Problem | Evidence and mechanism | Implication for Spacialize |
| --- | --- | --- |
| Difficulty closing tabs | The 2021 *When the Tab Comes Due* study found competing reasons to keep and close tabs, including reminders, anticipated retrieval effort, attention, and resource costs. Tabs carry unfinished work, not merely URLs. [1] | Saving must feel trustworthy and make work easy to rediscover. Moving clutter elsewhere is insufficient. |
| Losing context between tasks | Tabs.do explored task bundles and resumption rather than individual-tab management. Participants valued structures matching their work. [2] | Preserve a task's sources and next action together. Test resumption after an interruption. |
| Uncertainty about future relevance | Gstell's 2026 field experiment studied 29 knowledge workers. Its shelf and evolving groups helped participants move between active and stored pages; reported benefits included improved focus. [3] | Offer a low-effort inbox or “maybe later” state before demanding a category or canvas position. |
| Losing the browsing trail | Marble's creator describes losing the original travel search after following related topics across dozens of tabs. This is a maker's self-report, not independent demand validation. [4] | Explore automatic parent-child trails and collapsible branches. Location alone may not preserve reasoning. |
| Repeated switching during comparison | Vivaldi provides tiling to keep pages visible together. This establishes an existing competitive response; its availability alone does not quantify the user problem. [5] | Compare against split view before attributing benefits to an infinite canvas. |
| Separating evidence from interpretation | A Miro community user asks to interact with web pages inside a board. This is a concrete integration request, but just one report. [6] | Keep notes and source references adjacent; investigate whether users need live pages, captures, or both. |
| Resource pressure | Chrome deactivates inactive tabs through Memory Saver and reloads them when needed. This mitigates memory use rather than the meaning or organization of tabs. [7] | Distinguish a saved canvas object from a running web page. Benchmark many-page workloads. |
| Organization itself becomes work | Tabs.do discusses shortcomings of existing storage and grouping approaches; its small field study does not establish universal superiority. [2] | Measure organizing effort. Avoid making users label, place, or connect every page before receiving value. |

The strongest underlying distinction is between **accessing a page** and **managing an activity involving many pages**. Our inference: a browser can be good at the former while leaving users to reconstruct the latter themselves.

### How strong is the research?

- **When the Tab Comes Due (CHI 2021):** ten information workers interviewed repeatedly over two weeks, followed by a survey of 103 participants. Strong evidence for mechanisms and competing pressures; insufficient for a population-wide market percentage. [1]
- **Tabs.do (UIST 2021):** ten participants recruited for having experienced tab overwhelm, approximately one week of deployment. Seven continued daily use beyond ten weeks at reporting. Encouraging for task-centered management, but a small, self-selected sample and not a trial of spatial browsing. [2]
- **Gstell (CHI 2026):** a multi-week field experiment with 29 knowledge workers, with comparative usage data for 28 after one baseline failure. Supports further testing of storage and emerging organization, not a conclusion that canvases are necessary. [3]

Do not translate these samples into claims such as “most users need a spatial browser.” We also lack a representative estimate of willingness to switch or pay.

## 2. What has been tried?

The last column is our assessment of the remaining opportunity, not a claim that a product fails for every user.

| Approach | Examples and documented capabilities | What it addresses | Remaining question |
| --- | --- | --- | --- |
| Improve the tab list | Chrome documents tab search, saved groups, and vertical tabs. [8] | Findability, readable titles, temporary grouping, reopening work | Can a canvas beat this familiar, built-in baseline? |
| Preserve hierarchy | Tree Style Tab represents tabs in a collapsible tree. [9] | Branching navigation and visible relationships | Does free placement add enough beyond a tree? |
| Save and restore collections | OneTab converts tabs into restorable lists; Workona manages tabs in named spaces. [10][11] | Clutter, persistence, context separation | Do saved collections remain discoverable and meaningful weeks later? |
| Separate contexts | Arc Spaces separates browsing areas; Vivaldi Workspaces combines contexts with tab stacks and tiling. [12][5] | Switching projects without mixing everything | Is task restoration sufficient without a canvas? |
| Show several pages simultaneously | Vivaldi Tab Tiling. [5] | Comparison and reference while working | Does panning/zooming improve on a few readable panes? |
| Put captures and notes beside browsing | Arc Easels supports visual collections; creation/editing is documented for macOS, with viewing elsewhere. [13] | Research collection and visual composition | How often is a live page needed instead of a capture? |
| Combine browsing and a canvas | Kosmik documents a browser beside notes, images, PDFs, and extracted material. [14] | A combined browsing and synthesis workflow | This directly overlaps the proposed concept; workflow advantage must be demonstrated. |
| Spatial browser/workspace | Stack promotes a spatial and multiplayer browsing experience. The repository capture marks multiplayer as forthcoming. [15] | Spatial organization and shared work | Verify released capabilities and reliability; avoid scoring roadmap items as shipped. |
| Emerging canvas browsers | Marble describes connected live pages and local saving; Sowser's repository describes draggable WebView2 cards, pan/zoom, and workspaces. [4][16] | Spatial trails and persistent research | Public projects show supply and experimentation, not established retention or revenue. |
| Visual collaboration | Mural documents notes, frameworks, and canvas options; Miro supports embeds, subject to the source site's restrictions. [17][6] | Shared synthesis and facilitation | Can browsing be integrated without adding collaboration complexity too early? |
| AI-assisted research | Deta Surf currently positions itself as an intelligent notebook combining the web, files, and AI. [18] | Retrieval and sensemaking through a different interaction model | The alternative may be asking for information rather than navigating a visual layout. |

Additional watchlist: Web Canvas's App Store listing advertises browsing, notes, connections, and saved sessions on iPhone/iPad; Drift markets spatial browsing on Mac. These reinforce concept overlap but were not tested. [19][20]

### What earlier attempts teach us

Mozilla removed its earlier Tab Groups/Panorama feature in 2016, describing it as rarely used. That is evidence of limited adoption of a particular implementation, not proof that all visual organization fails. Still, it cautions against equating enthusiastic niche feedback with broad demand. [21]

Arc also phased out Notes. This confirms that browser-integrated productivity features can be withdrawn; the documentation alone does not establish why. Export and portability should therefore be part of the proposed value, particularly for users investing effort in long-lived research. [22]

Research on SAGE3 describes orientation problems on infinite canvases and “window inflation,” where newer content becomes larger and more prominent. Its use of viewports and navigation aids suggests that infinite space needs boundaries and landmarks. This is adjacent collaboration research, not a controlled browser comparison. [23]

## 3. Where might there be a market opportunity?

These are proposed segments to validate, not established market rankings.

| Candidate segment | Repeated job | Likely value to test | Main uncertainty |
| --- | --- | --- | --- |
| Researchers, analysts, consultants | Gather sources, compare evidence, resume a brief | Recover reasoning and produce a traceable synthesis | Existing reference and note tools may already be sufficient |
| Product and UX practitioners | Compare competitors, assemble findings, explain decisions | Keep evidence connected to notes and themes | Miro/Mural plus a browser may be good enough |
| Students and independent writers | Research across sessions and build an outline | Preserve source context while drafting | Willingness to pay and sustained organization effort |
| People comparing purchases or travel | Compare options across many sites | Side-by-side evaluation and revisitability | Episodic use may not support a subscription |
| General everyday browsing | Messaging, search, entertainment, transactions | Unclear incremental value | Navigation overhead may exceed benefits |

**Recommended initial segment:** people who repeatedly research a question across multiple sources and return to it on another day. Recruit by observed behavior rather than job title or number of tabs alone.

Potential positioning: “Return to your research with its sources, relationships, and next steps intact.” This is a hypothesis, not a validated product promise.

The meaningful competitive baseline is a modern browser with saved groups and search, plus an existing notes/whiteboard tool. A deliberately disorganized browser would exaggerate the advantage.

Commercial evidence is still missing: active users, cohort retention, conversion, acquisition costs, switching barriers, and willingness to pay. A product list is not a market-size calculation. After identifying a segment, estimate opportunity bottom-up from eligible users, observed problem frequency, reachable distribution, and tested conversion/pricing assumptions.

## 4. What should the spatial premise be tested against?

The hypothesis is that stable positions and visible relationships reduce the effort of recovering and using context. Competing explanations include better persistence, simultaneous visibility, or better notes. Those could work without free spatial navigation.

### Proposed research sequence

1. **Observe 12-15 target users.** Ask them to show a real unfinished research task, retrieve an older source, switch projects, and explain why tabs remain open. Include users satisfied with existing tools and people who abandoned tab managers. Record incidents, workarounds, and consequences; do not ask only whether they like the concept.
2. **Compare three conditions.** A: familiar browser with search/groups and normal notes. B: saved task workspace with the same sources, notes, and persistence as C, but a list or tiled view. C: spatial canvas. Comparing B and C helps isolate spatial layout from the rest of the feature bundle.
3. **Use realistic tasks across sessions.** Have users compare alternatives, support a recommendation with sources, then resume after a delay. Counterbalance condition order, match task difficulty, and give comparable training. Measure setup time as part of the cost.
4. **Run a two-to-four-week field pilot.** Look for voluntary reuse across real projects, accumulation of clutter, retrieval after days away, and export or migration needs. A short demo cannot reveal whether the canvas becomes another storage graveyard.

### Measures and decision rules

| Measure | Why it matters |
| --- | --- |
| Time to resume meaningful work | Tests the central context-restoration promise |
| Correct source retrieval after a delay | Tests durable findability rather than visual appeal |
| Quality and completeness of the final decision | Prevents speed gains from hiding weaker reasoning |
| Total time, including arrangement and maintenance | Detects productivity losses from canvas housekeeping |
| Navigation mistakes and lost-location incidents | Detects spatial disorientation |
| Perceived workload, followed by observed repeat use | Separates pleasant first impressions from ongoing value |
| Reliability and memory use at realistic page counts | Checks whether usable performance survives scale |

Before testing, choose a minimum worthwhile improvement with prospective users. For example, a 20% reduction in median resumption time with no material loss of task quality could be a provisional product threshold; this number is a proposed criterion, not a research finding. Report participant variability and uncertainty. If the task workspace performs as well as the canvas with less effort, prioritize the workspace. If benefits disappear after novelty wears off, reconsider the spatial premise.

## 5. Implications for an initial prototype

Prioritize persistent task workspaces, safe restore, source-linked notes, search, optional relationships, and rapid switching between overview and readable page views. Provide automatic initial placement, undo, a home/overview action, and keyboard navigation. Treat canvas arrangement as optional until evidence says otherwise.

Use a hybrid of saved representations and active pages to investigate performance. Make it explicit whether an object is a URL, saved capture, or live page. Miro's documented embed limitations also mean that a whiteboard containing arbitrary website embeds should not be assumed equivalent to a browser. [6]

Defer a full Miro/Mural feature set and multiplayer until solo research value is established. Collaboration should be a separate hypothesis: shared source organization and notes do not automatically require sharing authenticated browsing sessions.

The next decision should be **which recurring research workflow to test**, followed by whether spatial layout improves it enough to justify switching costs.

## Sources

All web sources accessed 29 September 2026. Dates below are publication dates where established, not search-engine crawl dates.

1. [When the Tab Comes Due, CHI 2021](https://josephcc.com/static/papers/233987809/paper.pdf) — empirical research.
2. [Tabs.do: Task-Centric Browser Tab Management, UIST 2021](https://lxieyang.github.io/assets/files/pubs/tabsdo-uist-2021/tabsdo-uist-2021.pdf) — prototype field study.
3. [From Tabs to Structures: Understanding and Supporting Web Page Management, CHI 2026](https://doi.org/10.1145/3772318.3791979) — Gstell field experiment.
4. [Marble creator's account, September 2026](https://www.reddit.com/r/SideProject/comments/1wi4iwd/i_built_a_spatial_browser_because_i_kept_losing/) — maker self-report; promotional context.
5. [Vivaldi Workspaces](https://vivaldi.com/features/workspaces/) and [Tab Tiling help](https://help.vivaldi.com/desktop/tabs/tab-tiling/) — vendor documentation.
6. [Browser page within Miro](https://community.miro.com/ask-the-community-45/browser-page-within-miro-3181) — user request and support discussion.
7. [Chrome performance settings](https://support.google.com/chrome/answer/12929150?hl=en) — vendor documentation.
8. [Manage tabs in Chrome](https://support.google.com/chrome/answer/2391819?hl=en-GB) — vendor documentation; availability can vary by version/platform.
9. [Tree Style Tab](https://addons.mozilla.org/en-GB/firefox/addon/tree-style-tab/) — extension listing.
10. [OneTab Help](https://www.one-tab.com/help) — vendor documentation.
11. [Workona Tab Manager](https://workona.com/help/tab-manager/) — vendor documentation.
12. [Arc Spaces](https://resources.arc.net/hc/en-us/articles/19228064149143-Spaces-Distinct-Browsing-Areas) — vendor documentation.
13. [Arc Easels](https://resources.arc.net/hc/en-us/articles/19231142050071-Easels-Capture-Create) — vendor documentation.
14. [Kosmik Browser](https://www.kosmik.app/blog/kosmik-browser) — vendor description.
15. [Stack](https://stackbrowser.com/) — vendor site; release status of individual claims not verified.
16. [Sowser / TREE-TABS repository](https://github.com/noisyboy08/TREE-TABS) — creator documentation, not a code audit.
17. [Mural features](https://www.mural.co/features) — vendor documentation.
18. [Deta Surf](https://deta.surf/) — current vendor positioning.
19. [Web Canvas App Store listing](https://apps.apple.com/us/app/web-canvas-spatial-browser/id6755220973) — developer-provided listing.
20. [Drift](https://driftwebbrowser.com/) — vendor site.
21. [Mozilla: Discontinuing Rarely Used Firefox Features, March 2016](https://blog.mozilla.org/futurereleases/2016/03/08/discontinuing-rarely-used-firefox-features/) — historical product decision.
22. [Phasing Out Arc Notes](https://resources.arc.net/hc/en-us/articles/19233788518039-Phasing-Out-Arc-Notes) — vendor documentation.
23. [Building Collaborative Intelligence: The Translational Journey of SAGE, 2026](https://link.springer.com/article/10.1007/s42979-026-04861-5) — adjacent spatial collaboration research.
