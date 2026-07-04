# L.I.N.K. Master Blueprint
**Version:** 0.2. Complete inventory per full system walkthrough, 04 JUL 2026.
**Role:** Primary source document for the L.I.N.K. Portfolio Project. Seeds three deliverables: (1) public portfolio site, (2) G6 handoff system map, (3) resume and interview prep alignment.
**Convention:** Items tagged [HANDOFF] matter to the G6 handoff rendering. Items tagged [ROADMAP] are under construction and do not render on the public system map. Items tagged [OPEN] need a decision from Drizzy.

---

## 1. Mission and End State

Build a live, public, interactive portfolio website hosted on GitHub Pages and linked from the resume. A hiring manager clicks the URL and gets a full tour of L.I.N.K.: the problem, the program authored, the system built, an explorable architecture map, screenshots, measured adoption numbers, and honestly labeled projections.

The site proves three claims:
1. Comprehensive solution to a big organizational problem. The builder thought of everything. Show, do not tell.
2. The builder has performed the Power Platform Functional Consultant role at division scale for eighteen months: every task the role demands maps to a named artifact (the tasks), and every artifact demonstrates governance, auditability, documentation, ownership, and lifecycle discipline — the exact instincts that prevent the sprawl and technical debt the low-code industry names as its top risk (the mind).
3. The builder is a cleared, GCC High-native, federal-fluent modernizer — the profile federal low-code contractors cannot hire off the street (the moat).

Two viewing modes drive all design decisions:
- **Skim mode (60 seconds):** landing page alone tells the whole story. Numbers up front.
- **Dig mode (5+ minutes):** system map and detail panels prove depth to technical screeners.

---

## 2. Story Arc (Landing Page Narrative)

Seven beats (0–6), top to bottom:

0. **WHO.** This is a portfolio. Identity first: Justin Drake, Power Platform Functional Consultant. Active Secret clearance. U.S. Army veteran, 20 years. Value line: self-taught the platform and single-handedly built and fielded the system of record for recruiter onboarding and certification across a 10,000-person organization — solo, in federal GCC High, at zero licensing cost. L.I.N.K. is presented as THE FEATURED PROJECT, not the site's identity.

1. **PROBLEM.** New recruiter training was inconsistent by unit, tracked in spreadsheets and memory, validated by informal checkboxes, pencil whipped under time pressure. Result: 13% ATP certification completion over the prior 12 months. No audit trail, no chain of command visibility, no protection for the soldier who never received real training. Frame as legacy-process modernization: a mission-critical process running on spreadsheets, memory, and informal checkboxes — the classic legacy state federal modernization work targets.

2. **CONSTRAINT AS CREDENTIAL.** Federal GCC High — the sovereign, compliance-bound government cloud. No budget, no dev team, no premium licensing. One cleared builder, standard connectors, SharePoint data layer. Two-sided framing rule: these are constraints overcome AND a credential moat — hands-on delivery inside the hardest, most compliance-bound version of the platform, an environment accessible only to screened U.S. persons. Copy must carry both meanings.

3. **THE PROGRAM.** Before the platform existed, the doctrine did. Authored the modern ATP itself: 4 domains, 23 capabilities, 34 tasks, 6-checkpoint feedback framework, UR 350-1 Appendix J rewrite, OPORD 26-0016, SOP, 34 Interactive Trainer's Guides, ATP Recruiter's Guide, orientation videos, 21-minute private-proof video SOP covering every role from station commander up, facilitator scripts, checkpoint email packages, Dead Reckoning podcast series. Program architect first, platform builder second.

4. **THE SYSTEM.** L.I.N.K. (Leader's Integration and Navigation Kit). The better mousetrap that makes training a matter of objective, forensic truth. 3 canvas apps, ~19 Power Automate flows, SharePoint data layer, 4 Power BI reports, Palantir/Vantage integration. System of record under general officer signed OPORD 26-0016, launched division wide 01 JUN 2026.

5. **SCALE.** 2,000+ registered users four weeks after launch. Nearly 5,000 soldiers enrolled in the ATP. 10,000-person organization. 1,800 command teams trained — every station, company, and battalion in the division, in person. (The ~14,000 / ~28,000 figures are internal ATP Monitor identity-resolution mechanics ONLY — never in hero or scale copy. The "10/10 sessions, all brigades" claim is retired: factually misleading.)

6. **RESULTS.** Two tiers, honestly framed:
   - **Measured:** Approved public phrasing: "ATP certification completion has achieved and maintained above 90% since launch, against a 13% baseline." "Maintained since launch" is the ONLY permitted time framing — never "month one," never "in one month," anywhere it appears. The 2,000+ users / four weeks adoption-velocity claim stays (registration metric, honestly time-stamped).
   - **Projected (labeled as projection, causal chain shown):** two-sided attack drives a targeted 10% increase in recruiter first-year production, an estimated 4% overall bottom line impact. The causal chain: structured curriculum arms trainers from the top, frictionless access pulls recruiters in from the bottom, and even the least engaged station commander now delivers decent training.
   - Copy rule: never present the projection as a result. The honesty is a credibility asset.

---

## 3. Site Structure

Single page site with anchored sections plus the interactive map view.

| # | Section | Content | Mode |
|---|---------|---------|------|
| 1 | Hero | Identity strip: JUSTIN DRAKE — POWER PLATFORM FUNCTIONAL CONSULTANT · PORTFOLIO · Active Secret clearance. Compass mark + L.I.N.K. framed as FEATURED PROJECT. Value-prop line (Beat 0). One-line problem→outcome frame in civilian language. Stat cards: 2,000+ users/four weeks · 13% baseline → 90%+ certification completion, maintained since launch · 3 apps · nearly 20 flows · 4 BI reports, solo build, standard licenses · 1,800 command teams trained, every echelon, division-wide. CTAs: Explore the System / Contact | Skim |
| 2 | The Problem | Beats 1 and 2 | Skim |
| 3 | The Program | Beat 3. The authorship stack, itemized by name | Skim/Dig |
| 4 | The System | Beat 4. Component cards; click opens detail panel | Dig |
| 5 | System Map | Interactive architecture diagram (Section 7) | Dig |
| 6 | Scale and Rollout | Beat 5, rollout timeline | Skim |
| 7 | Results | Beat 6 | Skim |
| 8 | How It Was Built | Origin story (battle rhythm tool → discovered the broken ATP → nearly alpha-ready when command came asking). Defense/offense frame: app is defense (integrity, auditability, legally defensible records), content is offense (capability, time to proficiency, production lift). THE ANTI-SPRAWL THREAD: every forensic design choice named as the answer to a documented industry failure mode — immutable audit log vs. no audit trail; self-healing access + Registry Manager + G6/G3-7 ownership split codified in a signed OPORD vs. orphaned ownership and credential debt; validation chains vs. flows that "mostly work"; anonymity-by-architecture and sterilization pipeline vs. data leaking into wrong environments; SOP + handoff docs + Tier 1/2/3 support model vs. undocumented estates. THE SUCCESSION CLAIM closes the thread: "The system was deliberately engineered to outlive its builder — codified ownership (OPORD-signed G6/G3-7 split), Tier 1/2/3 support model, self-healing access management, and full handoff documentation, designed from day one for the builder's planned departure. The number-one cause of low-code system death is the builder leaving; this system's succession plan shipped before launch." THE REUSABILITY THREAD: the AI-augmented tooling (Task Builder, ITG engine) framed as accelerator thinking — repeatable machinery, not one-offs. Constraint-questioning stories (nightly refresh "impossible," done without violating security; standard-license architecture). Design philosophy: the right path is the path of least resistance; data illuminates, it does not punish | Dig |
| 9 | Consultant Competency Map | Section 4 rendered as an interactive checklist: JD requirement to named artifact | Dig |
| 10 | Roadmap | Section 8, one line per module, no connectors drawn | Skim |
| 11 | About / Contact | Bio: 20 years Army, certified instructor and training developer, Master Trainer, MBA candidate Dec 2026, active Secret clearance, transitioning. Closing beat: performed this role verbatim for eighteen months before learning it had a name. Contact: [OPEN: email / LinkedIn, Drizzy provides at build time] | Skim |

---

## 4. Functional Consultant Competency Map

Synthesized from the Microsoft PL-200 role definition and current market job descriptions (requirements gathering, functional design, solution configuration, integration, documentation, training and enablement, adoption, governance). Procentrix-weighted but universal. Each row becomes a site element: requirement, evidence, artifact.

Render rule: each row is requirement → artifact → durability. The third element is one line on why the solution won't rot — the governance/lifecycle/documentation discipline that prevents the sprawl and technical debt failure modes.

| FC Competency | L.I.N.K. Evidence |
|---|---|
| Perform discovery, capture requirements, engage stakeholders and SMEs | Requirements gathered at every echelon from station to division HQ; SME interview pipeline (DeepWell reports) feeding training content |
| Translate business needs into functional designs | The ATP program design itself; checkpoint framework; forensic record architecture; anonymity pipeline design |
| Configure and build solutions (canvas apps, flows, BI) | 3 canvas apps, ~19 flows, 4 Power BI reports, SharePoint data layer, all solo under standard licensing |
| Implement integrations with external services | Palantir/Vantage ingestion (72-hour automated), official Army HR data source lookups, Microsoft Planner integration |
| Data modeling, migration, visualization | 115-column survey schema; sterilization pipeline; semantic model clearinghouse (Alpha Roster Lookup); "iPhone of Power BI" design standard |
| Generate documentation and solution artifacts | OPORD 26-0016, UR 350-1 Appendix J rewrite, SOP, G6 handoff documentation with Tier 1/2/3 support model |
| Facilitate training and enablement | 10/10 division sessions, 1,000+ leaders trained, 34 ITGs, video SOP, Recruiter's Guide, podcast series, leave-behind self-help tools |
| Drive user adoption and change management | Adoption engineering by design (one-click recruiter registration, path of least resistance); 2,000+ users in four weeks; advocacy campaign to general officers |
| Solution governance and lifecycle | Technical vs program ownership split (G6/G3-7), change authority gated by approval chains, curriculum modification workflows in the Task Manager app |
| Problem solving under constraints | Nightly refresh workaround, standard-license architecture, anonymity-by-architecture, self-healing access management |
| Communication across technical and non-technical audiences | Every artifact above had a different audience, from general officers to brand new recruiters |
| Federal compliance fluency | Entire system delivered in GCC High on standard connectors: sovereign-cloud constraints, records defensibility, role-gated access, anonymity-by-architecture — cleared, federal-native delivery |
| Certification | PL-200 in progress [exam retires 31 AUG 2026, urgent] |

---

## 5. Master Component Inventory

### 5.1 Canvas Apps (3)

**App 1: L.I.N.K. (hero).** Main user interface, system of record for the ATP. Launched division wide 01 JUN 2026 under OPORD 26-0016. Core functions: ATP progress tracking (4 domains / 23 capabilities / 34 tasks, date-time stamp on every action, immutable audit trail as the anti-pencil-whip mechanism), auto-generated ATP Completion Reports distributed up the chain of command, embedded adult-learning training resources at point of need, recruiter self-view dashboard, embedded ATP Monitor report producing monitor-and-manage in one place. [Drizzy will revise this description; good enough for now. Open flags: leader team-roster view confirm.]

**App 2: ATP Checkpoints.** Standalone by design. No-login recruiter survey interface. Collects checkpoint survey data, assures anonymity, sterilizes intake before routing. The separation from the identity layer IS the feature. Renders on the map as deliberately disconnected from L.I.N.K.'s identity layer, detail panel explains why.

**App 3: LINK Task Manager** (possible rebrand: Admin Portal). Program management console for the HQ training team. Field trouble tickets beyond self-service, suggestion intake, curriculum modifications behind approval chains. Physical embodiment of the ownership split: G6 owns the platform, G3/7 owns the program through this app. [HANDOFF]

### 5.2 Data Layer

**SharePoint lists directly connected to L.I.N.K. (9):**
1. LINK User Registry. User registration data.
2. ATP Master List. Permanent training records for the duration of assignment. Primary workhorse.
3. ATP Archive. Duplicate structure; scheduled weekly flow sweeps departed soldiers from Master to Archive.
4. ATP Audit Log. Every ticket and record change against the Master List. Entries roll into the Completion Report. Enables logged self-help.
5. ATP Documents Library. ITGs and resources for all 34 tasks.
6. Suggestion Box.
7. ATP Smart Card Master List. Content engine for digital ITGs; delivers the 8-step adult learning model in app so domain knowledge alone produces sound training.
8. Training Request List. Field-to-HQ outreach requests.
9. Battle Rhythm Tasks. Master task repository; spine of C-STAR, How2Hub, Battle Rhythm Planner. [ROADMAP]

**ATP Checkpoints data web:**
- Intake list: 115 columns, one per survey question (SharePoint auto-named most as field_NNN due to question-length names).
- Sterile list: receives scrubbed rows from the sterilization flow; sterile from day one.
- Vantage ingestor: every 72 hours, automated scrape of the sterile list into Palantir/Vantage, the permanent longitudinal home. Feed math: ~2,500 new recruiters/year x 5+ surveys = ~12,500 rows/year, fully autopilot, zero maintenance.
- Anonymity is architecture, not policy: identifiable data structurally cannot persist.

**Supporting lists:** two to three behind-the-scenes/static lists feeding Power BI. Not itemized on the public map by decision. [HANDOFF: itemize in handoff rendering.]

### 5.3 Power Automate Flows (~19 catalogued; public number "nearly 20")

**App-triggered (5):**
1. **Enroll ATP.** Live lookup against the official Army personnel data source. Validates identity and enrollment completeness. Nobody slips through the cracks.
2. **LINK_Register User.** Same validation engine, forensic-grade gate: accounts can touch official records feeding career-altering legal decisions.
3. **LINK_Register User_DOD ID Lookup.** Manual fail-safe keyed by DoD ID when the primary lookup cannot resolve.
4. **Recruiter Verification.** Fires when a trainer logs a session. Locks the record, initiates a Power Automate approval to the soldier: confirm the training happened as logged, or refute. Refute notifies the trainer's supervisor. The anti-pencil-whip mechanism made concrete. FEATURED DETAIL PANEL.
5. **Recruiter Register to LINK.** One-click pre-vetted registration for recruiters only (already validated via ATP enrollment; role grants read-only own-record access plus full resource library). Adoption engineering at the base of the pyramid.

**ATP Checkpoints cluster (4, fully automated):**
6. **ATP Checkpoints.** Scheduled nightly; sweeps days-in-program against CP1-4 thresholds (day 15/30/60/90); emails survey link.
7. **ATP Checkpoint 5 and 6.** Condition-based on a column value change; same behavior.
8. **ATP_Checkpoint Reporter.** On survey submission: intakes raw data, sanitizes PII, writes sterile copy to staging list, deletes original row.
9. **Daily Reminder ATP Checkpoints.** Scheduled daily; carbon-copy reminder email until completion.
Full checkpoint lifecycle (eligibility, notification, collection, anonymization, archival, delinquency) runs with zero human touches.

**Lifecycle and records (4):**
10. **ATP Welcome Letter.** On enrollment: welcome email with resources plus pre-generated one-click registration URL. Front door of the adoption funnel.
11. **ATP Completion Report.** On full certification: marks all required fields across lists, generates the whole-journey report (every training entry, every immutable trainer remark, complete Audit Log history, every attached document), emails soldier plus entire chain of command, appends to the soldier's permanent record. The payoff artifact of the forensic design.
12. **Weekly Archive Sweep.** Scheduled; moves departed soldiers' records from Master to Archive.
13. **ATP Ticket Tool.** Complex, app-triggered. Self-service tickets: executes the full forensic checklist, applies the change, stamps the Audit Log. Intervention tickets: same forensic front end, routes to admin inbox, stamps and reports on resolution. Why the Audit Log works; the system triages its own workload. [HANDOFF]

**Access and identity (2):**
14. **Auto Approval LINK Access Request.** Catches Power Platform access requests from in-processing personnel, adds requester to the correct security group, sends confirmation email. Self-healing access management.
15. **LINK User Registry Manager.** Simple function, remarkably complex execution: multistage multi-party approvals, lookups against official HR records, discrepancy-triggered validation chains. Never take anyone's word except official sources. FEATURED DETAIL PANEL. [HANDOFF]

**Battle Rhythm module (4).** [ROADMAP]
16. **Get Planners.** App-triggered; surfaces Planner boards the current user owns.
17. **Load Recurring Tasks.** Pushes tasks to selected planner. Merge candidate with 18.
18. **Load Nonrecurring Tasks.**
19. **Recruiting Calendar.** Pipes the recruiting calendar in; likely standalone.

**Utility flows (excluded from map):** ad hoc bulk edit / dedup one-offs. [HANDOFF: single line, "deprecated, do not maintain."]

### 5.4 Power BI (4)

1. **ATP Monitor.** Flagship. Solves the hard identity-resolution problem: ~28,000 total assigned personnel filtered to ~14,000 in-division, then to on-production, then to role. Sources: Vantage (Palantir) HR data plus the ATP Master List and two to three supporting lists. Tracks enrollment completeness and progress, zoomable division-to-station (3 to 20 members). Built for the non-Power-BI user: app-like, instantly readable, "the iPhone of Power BI reports." Embedded on L.I.N.K.'s main ATP screen: monitor and manage in one place, unprecedented in the business.
2. **Alpha Roster Lookup.** Not public facing. Semantic model serving as the validation clearinghouse; every forensic process resolves official-HR lookups through it. Renders as a hub node. [HANDOFF]
3. **ATP Checkpoint Findings.** [ROADMAP] Presents survey findings; shareable broadly because it aggregates at battalion level and higher only, protecting anonymity in the report layer as the pipeline does in the data layer. HTML mockup exists (Drizzy adding file to Project).
4. **LINK Registration Tracker.** Unit-level self-service registration tracking, hourly refresh. Feeds the adoption story: units watch their own numbers climb.

**Refresh story:** all reports auto-refresh nightly at midnight in an environment where multiple government data professionals said scheduled refresh could not be done. Done anyway, without violating security.

### 5.5 AI-Augmented Tooling

- **LINK Task Builder.** Permanent fixture. Standardizes How2Hub task formatting: extracts the right information from the user, outputs in a standardized AI-friendly method, makes indexing and placement trivial while providing immediate field value.
- **ITG Developer.** HTML tool used in ITG production.
- **Smart Card Builder.** Retired; did its job producing ITGs. One line max on the site, framed as proof of AI-augmented process design; superseded by the Task Builder.

### 5.6 Non-Code Artifact Stack (itemized by name on the site)

OPORD 26-0016 (general officer signed, division wide). UR 350-1 Appendix J rewrite. ATP SOP. 34 Interactive Trainer's Guides (concept originated and willed into existence, then scaled through the division HQ training development team). ATP Recruiter's Guide (13 pages, 4 domains, 23 capabilities, 34 tasks). 21-minute video SOP, private proof, every role from station commander up. Orientation videos. Checkpoint email content packages. Facilitator scripts. Dead Reckoning podcast series. White paper (authored four days after initial inspiration).

---

## 6. Numbers Ledger (single source of truth; must match resume exactly)

| Metric | Value | Status |
|---|---|---|
| Baseline ATP certification completion, prior 12 months | 13% | Measured |
| ATP certification completion | 13% baseline → >90%, maintained since launch | Measured. "Maintained since launch" is the only permitted time framing in public copy |
| Registered L.I.N.K. users, week four | 2,000+ | Measured |
| Soldiers enrolled in ATP, month one | ~5,000 | Measured |
| Tracked production personnel (ATP Monitor population) | ~14,000 | Measured (distinct claim from registered users; use each correctly) |
| Total assigned personnel in source data | ~28,000 | Context for the identity-resolution problem |
| Command teams trained | 1,800 (station: 1,328 · company: ~450 · battalion: 38 + staffs) — every echelon, division-wide, in person | Measured, resume-aligned. Unit of count is COMMAND TEAMS, never "leaders" or "people"; actual human count ~3,000+ but no hard headcount exists, so it is never cited publicly |
| Organization size (public framing) | 10,000-person organization | Resume-aligned. 14,000/28,000 reserved for internal Monitor mechanics only |
| Personnel aware of program | ~1,800 | Superseded by launch numbers; retire this figure |
| Checkpoint survey inflow | ~12,500 rows/year | Structural |
| Projected first-year production increase | +10% | Projection, labeled |
| Projected bottom line impact | ~4% | Projection, labeled |
| Launch date | 01 JUN 2026 | Fact |
| Flow run counts, app sessions, report views | TBD | [OPEN: pull from Power Platform analytics before access ends] |

---

## 7. Interactive System Map Specification

**Layout:** L.I.N.K. hub-and-spoke center. ATP Checkpoints web rendered as a deliberately separate island (the visual gap is the anonymity story). Task Manager as the governance node. Alpha Roster Lookup as a validation hub with edges into every forensic flow. Vantage as the external boundary node.

**Node classes:** app, SharePoint list, flow (badge by trigger type: app / scheduled / condition), Power BI report, external system.

**Interaction:** click node, side panel opens: what it does, who uses it, what it connects to, one screenshot. Hover highlights the data path. Trigger-type badges signal real production architecture (mixed app-fired, event-driven, scheduled).

**Guided tour default path (LOCKED): the checkpoint lifecycle.** Nightly eligibility sweep, survey email, anonymous companion app, sterilization flow, sterile list, 72-hour Vantage ingestion, battalion-aggregated findings report. One path demonstrating scheduling, event triggers, privacy architecture, external integration, and BI.

**Featured detail panels:** Recruiter Verification (integrity engineering), LINK User Registry Manager (validation complexity), ATP Completion Report (the payoff artifact), ATP Monitor (identity resolution plus embedded monitor-and-manage).

**Render rule:** nothing under construction gets drawn. [ROADMAP] items appear only in the Roadmap section, one line each.

---

## 8. Roadmap (site section; also the handoff to-be state)

Under construction, next three modules: **Battle Rhythm Planner** (Planner-integrated task scheduling from the shared library, a la carte or pre-canned bundles like Station Commander Weekly), **How2Hub** (view-in-app task library, tagged bundles plus free-floating), **C-STAR** (the decision engine: prior-quarter production data in, root-cause diagnosis, training prescriptions from How2Hub, scheduling against the SC's real planner and recruiting calendar, assignment and delegation out; composite of the planning engine, How2Hub, and external production data).

Bolt-on consolidation modules (1 to 2 days each): unit training tracker, schools management, inspections. Absorbs the field's primitive standalone apps into one platform.

Origin note: the battle rhythm tool was the original inspiration; the ATP was the detour that became the flagship.

---

## 9. Screenshot Shot-List

Capture on the closed network, scrub, transfer per policy. Scrub pass on every image: no names, DoD IDs, real production data, internal URLs, or unit identifiers beyond approved. Kill-list decision deferred to capture time.

| # | Shot | Purpose |
|---|------|---------|
| 1 | L.I.N.K. main ATP screen with embedded ATP Monitor | Hero image; the monitor-and-manage claim, proven |
| 2 | Recruiter Verification approval flow canvas | Engineering proof; the integrity mechanism |
| 3 | LINK User Registry Manager flow canvas (collapsed view) | Complexity proof |
| 4 | ATP Checkpoints app survey screen | The anonymity companion |
| 5 | ATP Monitor, division view and station drill-down | "iPhone of Power BI" |
| 6 | LINK Registration Tracker | Adoption story |
| 7 | ATP Completion Report sample (test record) | The payoff artifact |

Fallback: stylized vector recreations from description if scrubbing kills any shot.

---

## 10. Naming and Publication Decisions

| Item | Decision |
|---|---|
| OPORD 26-0016 | Named on site. LOCKED |
| UR 350-1 Appendix J | Named on site. LOCKED |
| Palantir / Vantage | Referenced as spoken (Vantage, a Palantir data source). Genericize only if Drizzy reverses. [OPEN: confirm] |
| Official Army HR/personnel source | [OPEN: name or genericize as "authoritative Army personnel system"] |
| Checkpoint email series | "ATP Checkpoint Package" or specific checkpoint reference only. Never "Heartbeat." LOCKED |
| Contact info | [OPEN: Drizzy provides at build time] |
| "~15 flows" figure | Retired. Use "nearly 20." LOCKED |
| Compliance stat framing | "Maintained above 90% since launch vs 13% baseline." No other time framing. LOCKED |
| Org size public figure | 10,000. LOCKED |
| Leaders-trained unit | Command teams (1,800), never individual headcount. LOCKED |

---

## 11. Parking Lot

1. G6 handoff system map rendering (own session; this document is its skeleton). [HANDOFF]
2. Screen-by-screen L.I.N.K. inventory (only as needed for detail panels and handoff).
3. Flow run metrics / app session / report view capture from Power Platform analytics before access ends.
4. Video snippets for the site (revisit after launch).
5. Custom domain (post-launch).
6. Hero app description revision pass (Drizzy).
7. Resume reconciliation against the Numbers Ledger (Drizzy adding resume to Project files).
8. HTML tool files into Project files (Drizzy).

---

## 12. Build Sequence (future sessions)

1. **Session 2: Site build.** Full HTML/JS single page per Sections 2, 3, 7. Placeholder media slots. Visual design language locked before code.
2. **Session 3: Media integration and deploy.** Scrubbed screenshots in, GitHub repo, Pages deployment, live URL. Deployment itself is a 10-minute task.
3. **Handoff session(s): G6 system map** rendered from this inventory. [HANDOFF]
