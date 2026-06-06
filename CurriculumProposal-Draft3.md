# CSS Curriculum Transition Plan: Preparing Graduates for an AI-Transformed Industry

**Version:** Draft 3
**Date:** June 2026
**Audience:** CSS Faculty
**Changes from Draft 2:** Reflects faculty decisions: AI fluency is a core competency (required, not elective); new standalone CSS 4xx confirmed; course elimination confirmed as in-scope; two funding scenarios added; ABET removed; teaching load and faculty capacity constraints incorporated; 4 new faculty hires (Sept 2026) noted as key capacity variable.

---

## Executive Summary

The computing job market has undergone a structural shift. AI tools now handle a significant portion of the work previously done by junior software engineers, raising the bar for what employers expect from new graduates. The CSS Department has made a clear decision: **AI fluency is a core competency** required of all graduates, not an optional specialization.

This proposal outlines a three-phase curriculum transition from 2026 through 2028-29:

- **Phase 1 (2026-27):** Weave AI content into existing required courses; launch special topics pilots; begin faculty upskilling. No new course numbers needed.
- **Phase 2 (2027-28):** Launch new CSS 4xx (AI for Software Engineers) as a required course; modernize CSS 382; execute dormant course phase-out to free capacity.
- **Phase 3 (2028-29+):** Goal-state curriculum with AI present at every level.

The proposal is planned against two resource scenarios (Moderate and Generous) and takes into account the 4 new faculty hires beginning September 2026 as a significant capacity variable.

---

## 1. Current State: What the Data Shows

### 1.1 Course Activity Summary (AUT2020-WIN2026)

Six years of schedule data reveals a clear divide between the high-volume required-core courses and the thin, often single-instructor AI elective layer.

**High-volume required core (Tier 1) - 7-14+ sections/year:**
CSS 142, 143, 342, 343, 301, 360, 370, 422, 350, 430, 497

**Active electives (Tier 2) - 2-6 sections/year:**
CSS 475 (DB), 310 (Cybersec), 478 (HCI), 211 (Society), 382 (Intro AI), 432 (Networking), 371, 385, 421

**Thin/specialist electives (Tier 3) - 1 section/year or fewer:**
CSS 486 (ML - single instructor Si Dong), 485 (Neural Nets), 444 (Biases), 487 (Computer Vision - was absent 2023-25), 488 (NLP - offered once), 434, 449, 461, 451

**Dormant (not offered 2025-26, or never offered at UWB):**
CSS 448 (Compilers - no 2025-26 offerings), 452 (Game Engine - stopped WIN2024), 484 (Multimedia Data - stopped AUT2024), 482 (Expert Systems - never offered in data), 130, 250, 416, 450, 455, 457, 477 (never offered)

### 1.2 Key Structural Problem: AI Courses Are Thin and Instructor-Dependent

All AI-area courses are Tier 2-3. A student can graduate without taking any of them. The courses that do exist are each taught by one or two instructors:
- CSS 382 is the healthiest: 3 instructors over 6 years, consistent schedule
- CSS 486 is almost entirely Si Dong; missed 2024 entirely
- CSS 487 (Olson) was absent from the schedule for two full years
- CSS 488 (NLP) has been offered exactly once

If any one instructor leaves or changes focus, an entire content area disappears. The solution is not to build more single-instructor AI courses, but to integrate AI broadly across many courses so the curriculum is resilient.

### 1.3 The New Faculty Opportunity

Four new faculty join in September 2026 (3 teaching track, 1 tenure track). This is the most significant capacity increase in recent years. Their areas of expertise are not yet known in this planning document, but if any have AI/ML teaching capability, they could be the primary instructors for CSS 4xx and/or expanded AI electives.

**Recommendation:** Make explicit AI teaching capacity a priority criterion in these hires and all future hires. Even one new faculty member who can own CSS 4xx and CSS 382 substantially changes the feasibility of the Phase 2 timeline.

---

## 2. Guiding Principles

1. **AI fluency is required, not optional.** Every graduate of CSSE and AC must demonstrate core AI competency.
2. **Foundations remain.** Algorithms, systems, SE process, and mathematics stay in the required core.
3. **Principles over tools.** Courses teach concepts that outlast specific products.
4. **Integration and dedicated instruction.** Phase 1 uses integration; Phase 2 adds a dedicated required course.
5. **Resilience over depth.** Avoid single-instructor AI bottlenecks; spread AI across many courses.
6. **Faculty must be supported.** No mandate without resources, even if those resources are modest.
7. **Clean the catalog.** Dormant courses create confusion and imply false capacity; remove them.

---

## 3. The Two-Track AI Curriculum Response

Both tracks are being pursued in parallel. They serve different purposes and different student populations.

| | CSS 382 (Modernized) | CSS 4xx (New) |
|---|---|---|
| **Level** | 300-level | 400-level |
| **Focus** | How AI works: search, ML, neural nets, LLMs conceptually | Building *with* AI: APIs, RAG, evaluation, responsible deployment |
| **Audience** | Any CSS major after CSS 340/342 | CSSE seniors; required; advanced AC students |
| **Role in requirements** | Prerequisite or co-req for CSS 4xx; recommended elective for AC | **Required course for CSSE; required elective for AC** |
| **Timeline** | Revised syllabus by Spring 2027; new version Autumn 2027 | Course proposal submitted March 2027; first offering Autumn 2027 |
| **Instructor model** | Currently 3 instructors rotating; maintain this | Start with 1 lead instructor; add second by 2028-29 |

---

## 4. Making Room: Recommended Curriculum Restructuring

Since AI fluency is a core competency, CSS 4xx must be a required course, not merely a recommended one. Adding a required course without removing or restructuring another creates degree bloat and burdens students. Two feasible options are presented.

### Option C (Recommended): Move CSS 370 from Required to Strongly Recommended

**What changes:** CSS 370 (Analysis and Design, 5 cr) moves from the CSSE required core to a "strongly recommended" elective. It remains available and continues to be offered; students are advised to take it, particularly if they plan roles in systems analysis, enterprise software, or consulting. The 5 credits freed become the slot for CSS 4xx.

**Why CSS 370 is the best candidate:**
- Its content (UML, data flow diagrams, entity-relationship modeling, requirements specification) is the most overlapping with material already covered in CSS 360 (Software Engineering) and CSS 350 (Management). Students encounter requirements analysis and design documentation in both.
- In practice, modern software teams have moved away from heavy upfront UML modeling toward lighter-weight approaches. CSS 370's content remains valuable but is less universally essential than it was when the curriculum was designed.
- CSS 370 currently has 7 sections/year - it is well-enrolled and will not disappear; students who want it can still take it.
- CSS 360 already includes design and requirements coverage; a module on AI-aware system design can be added there (Phase 1).

**What students would lose:** Dedicated deep coverage of formal modeling techniques. Students heading into roles that use UML or formal requirements processes (some enterprise and government contexts) would be advised to take it.

**Tradeoff summary:**

| Factor | Impact |
|---|---|
| Student impact | Applies to new admits only; existing students keep current requirements |
| Faculty impact | CSS 370 instructors still teach the course; enrollment may dip slightly |
| Curriculum committee | Requires formal approval; submit alongside CSS 4xx proposal |
| Signal sent | The department values AI literacy as highly as formal modeling |

### Option D (Alternative): Restructure CSS 350 and CSS 360 Together

**What changes:** CSS 350 (Management, 5 cr) and CSS 360 (Software Engineering, 5 cr) are redesigned as a single two-quarter sequence: CSS 360 (Software Engineering and Teamwork, 5 cr) + CSS 361 (AI-Aware Software Engineering, 5 cr). CSS 360 absorbs the most essential management content; CSS 361 covers both AI-integrated SE and the remaining management topics. CSS 4xx then becomes the third leg of an AI-focused sequence.

**Why this is harder:**
- Requires two new course proposals plus retirement of CSS 350 (complex for advising and degree audits)
- Affects 7-14 sections/year of two of the highest-volume courses - large disruption risk
- Requires coordinating 10+ instructors across two courses simultaneously
- Longer approval timeline

**Recommendation:** Pursue Option C in Phase 2. If it proves insufficient or if Option C faces strong faculty opposition, Option D is the backup for Phase 3.

### For the AC Program

The AC required core is lighter and more flexible. The recommended approach:
- Add CSS 4xx as a required course for AC (replacing one existing required elective slot or adding 5 credits to the degree if credit totals permit)
- CSS 382 becomes a recommended prerequisite for CSS 4xx in AC as well
- Existing concentration requirements are not affected

---

## 5. Phase 1: AY 2026-27 - Integration Without Restructuring

**Goal:** Every CSS student encounters AI meaningfully this year. No new course numbers. No curriculum committee changes. Faculty begin integration at whatever level they can manage.

**Catalyst:** The 4 new faculty starting Sept 2026 may be able to take on AI-related teaching immediately, depending on their expertise. Identify AI-capable new hires during onboarding and engage them in the Phase 1 planning early.

### 5.1 Required Course Modifications

Instructors implement these changes in their existing courses. These are targeted, not wholesale redesigns.

**CSS 360 (Software Engineering)** - Priority: HIGH
Add 2-week module on AI-assisted development:
- Using coding assistants with critical judgment: when to accept, reject, or modify AI output
- Testing strategies for AI-assisted code (AI introduces different failure modes than manual code)
- Team AI use policies and documentation practices
- Update project rubric: teams document their AI tool use throughout the project
- Effort: Medium. This is the most important Phase 1 change; CSS 360 is where the majority of CSSE students first do real team software development.

**CSS 211 (Computers and Society)** - Priority: HIGH
Refresh AI ethics content:
- Generative AI and attribution (authorship, IP, creative rights)
- Automation and the labor market students are entering - concrete, honest discussion
- Algorithmic bias and fairness: documented real harms (hiring, lending, criminal justice)
- AI in regulated domains (healthcare, financial services): what engineers are responsible for
- Retire pre-2022 case studies; replace with current examples
- Effort: Medium. Content refresh, new readings and assignments.

**CSS 301 (Technical Writing)** - Priority: MEDIUM
Add a module on writing about AI systems:
- Communicating model limitations, uncertainty, and risks to non-technical stakeholders
- Documentation standards when AI is involved in the development process (model cards, prompt logs, disclosure)
- Evaluating AI-generated text: recognizing hallucination, bias, and over-confidence in AI writing
- Effort: Low-Medium.

**CSS 350 (Management for Computing Professionals)** - Priority: MEDIUM
Add material on managing teams that use AI:
- IP ownership and code attribution when AI generates deliverables
- Disclosure obligations to clients and stakeholders
- Quality assurance when AI tools are in the workflow
- Effort: Low.

**CSS 343 (Data Structures & Algorithms II)** - Priority: LOW
Optional conceptual framing at relevant points:
- Graphs as the structure behind knowledge graphs and transformer attention mechanisms
- Hash tables as the basis for embedding lookup and vector search
- Trees and decision trees; parsing and LLM tokenization
- This is framing, not new algorithms; approximately 1-2 class periods
- Effort: Very Low.

### 5.2 Capstone Update (CSS 497 and CSS 496)

Starting Autumn 2026, all capstone project documentation must include:
- An AI feasibility section: should this problem use AI? What are the tradeoffs?
- AI tool use log: which tools were used, for what, what was kept vs. discarded and why
- If the system includes AI components: a brief bias and failure mode analysis

This is a rubric change, not a course number change. Capstone coordinators implement it.

### 5.3 Special Topics Pilots (CSS 490/390)

Pilot content for future new courses using existing special topics slots. No approval required.

**Pilot A: "AI Tools for Software Development" (1-2 cr, CR/NC)**
Seminar format; no prerequisites. Topics: coding assistants, prompt engineering basics, critical evaluation of AI output, responsible use policies. Target: all CSS students who want a low-stakes introduction.

**Pilot B: "Building with Large Language Models" (3-5 cr)**
Hands-on course; prerequisite CSS 342. Topics: LLM API integration, retrieval-augmented generation, agents, evaluation, responsible deployment. This pilots the content of CSS 4xx before it has a permanent number.

Both pilots are opt-in for instructors. If no existing faculty volunteers, identify a qualified AI-experienced adjunct or a new hire.

### 5.4 CSS 382 Revision Begins

Begin the revision process in 2026-27; deploy the revised course in 2027-28.

**Content to reduce:**
- Expert systems as standalone topic (CSS 482 is dormant; give this 1 lecture as historical context)
- Heavy symbolic AI and rule-based implementation detail
- Early neural network architectures as primary content (move to historical framing)

**Content to add:**
- ML foundations: supervised, unsupervised, reinforcement learning
- Deep learning and transformer architecture: conceptual level, not implementation detail
- Large language models: how they work, limitations, how to evaluate their outputs
- Hands-on: students work with real ML libraries and LLM APIs, not just algorithm simulations
- AI ethics as an integrated thread: each major topic includes its societal implications

**Timeline:** Draft revised syllabus by Spring 2027; review with CSS 382 instructors; deploy Autumn 2027.

### 5.5 Faculty Development in 2026-27

#### Moderate Funding
- **Summer 2026 AI Bootcamp (1 day):** Hands-on with AI coding tools, LLM APIs, pedagogical strategies. Run internally with 1-2 external guest practitioners. All teaching faculty; strongly encouraged. Targeted stipend of $500-1,000/attendee from discretionary budget.
- **Monthly Faculty AI Learning Community:** Informal lunch meeting; share what is working in Phase 1 course integrations; iterate.
- **Course development stipend:** 2-3 faculty receive summer stipends ($3,000-5,000 each) to redesign their courses for AI content.
- **1 course release (AY 2026-27):** For the CSS 4xx lead developer. If adjunct replacement is unavailable, negotiate overload arrangement or defer to AY 2027-28.
- **Institutional AI tool access:** GitHub Copilot Education tier for students; API credits for course labs. Estimated $3,000-5,000/year.

#### Generous Funding (adds)
- **Summer 2026 AI Bootcamp (2 days):** External facilitators, industry guests, travel stipends for faculty.
- **4-6 summer stipends** for course redesign at $4,000-5,000 each.
- **2 course releases** in AY 2026-27 for CSS 4xx development and CSS 382 revision.
- **AI-experienced adjunct recruitment:** Actively recruit 1-2 industry practitioners for CSS 490 pilots and eventual CSS 4xx sections.
- **Conference travel:** 2-3 faculty to AI education conferences (ACM SIGCSE, NeurIPS education track).

---

## 6. Phase 2: AY 2027-28 - Structural Addition

**Goal:** CSS 4xx launches as a required course; modernized CSS 382 deploys; dormant courses are formally removed from the catalog; CSS 370 transitions from required to recommended (if faculty approve Option C).

### 6.1 CSS 4xx - AI for Software Engineers (New Required Course)

**Credits:** 5
**Prerequisites:** CSS 343; CSS 382 recommended (or concurrent)
**Required for:** CSSE BS (replacing CSS 370 in required core under Option C); required elective for AC BA
**First offering:** Autumn 2027 (assumes curriculum committee approval by May 2027)
**Instructor model:** 1 lead instructor initially; identify co-instructor or second section by Spring 2028

**Course content:**

*Unit 1: AI as a Software Component (2 weeks)*
- AI APIs and SDK patterns; model hosting options (cloud, self-hosted, edge)
- Integrating AI into a software architecture: where it fits, what it depends on
- Cost, latency, and reliability characteristics of AI components

*Unit 2: Prompt Engineering and LLM Interaction (2 weeks)*
- Prompt design patterns: zero-shot, few-shot, chain-of-thought
- Structured output, function calling, and tool use
- Prompt versioning and testing; managing prompt drift over model updates

*Unit 3: Retrieval-Augmented Generation (RAG) (2 weeks)*
- Vector embeddings and semantic similarity
- Chunking strategies, retrieval architectures
- Building and evaluating a RAG system end to end

*Unit 4: Agents and Orchestration (1.5 weeks)*
- Agent design patterns: planning, tool use, memory
- Multi-agent systems; when they help and when they break
- Safety constraints and guardrails

*Unit 5: Evaluation (2 weeks)*
- Automated metrics (BLEU, ROUGE, F1, etc.) and their limits
- Human evaluation design; red-teaming
- Benchmarks: what they measure, how they can be gamed, how to interpret them
- A/B testing AI components in production

*Unit 6: Responsible Deployment (1.5 weeks)*
- Bias auditing: what to measure, how to measure it, what to do about it
- Explainability methods (LIME, SHAP) at a practical level
- Model cards and datasheets: documentation standards
- Legal and regulatory context: IP ownership of AI output, liability, disclosure obligations, EU AI Act overview

*Final project (across all units):*
Teams of 2-3 build and evaluate a software application that integrates at least one AI component. Deliverables: working system, evaluation report, bias analysis, model card or equivalent documentation.

**What this course is not:**
- Not a theory course (CSS 382 covers theory)
- Not a machine learning course (CSS 486 covers ML training)
- Not an ethics lecture course (ethics is integrated into every unit as an engineering consideration)

### 6.2 CSS 382 Modernized - Deploy Autumn 2027

Revised content as outlined in Phase 1. With the updated CSS 382 feeding into CSS 4xx, students have a coherent AI pathway:
```
CSS 342/343 → CSS 382 (Intro AI, theory) → CSS 4xx (AI Systems for SE, applied)
```
This two-course sequence can also feed graduate AI electives (CSS 486, 581, 586) for students who want depth.

### 6.3 Curriculum Committee Actions (Submit by March 2027)

| Action | Type | Timeline |
|---|---|---|
| New course: CSS 4xx (AI for Software Engineers) | New course proposal | Submit March 2027 |
| CSSE: CSS 370 from required to recommended (Option C) | Degree requirement change | Submit alongside CSS 4xx |
| AC: CSS 4xx added to required core | Degree requirement change | Submit alongside |
| CSS 4xx as prereq recommendation for relevant 400/500-level AI courses | Prerequisite update | Submit alongside |

All changes apply to new admits starting AUT2028. Existing students may opt in by request.

### 6.4 Dormant Course Phase-Out

Execute formal removal from the catalog of courses that have not been offered. Process: confirm with any responsible instructor; check with advising that no current student has the course on an active degree audit as a required elective; submit catalog deletion.

**Phase out immediately (never offered at UWB in data):**
- CSS 130 (Web Media Technology) - replaced functionally by CSS 481
- CSS 250 (Introduction to Interaction Design) - replaced by CSS 478
- CSS 416 (Ethical Hacking undergrad) - content covered in CSS 310, 337; graduate-level equivalent is CSS 578
- CSS 450 (Computer Graphics) - replaced by CSS 385, 451
- CSS 455 (Computational Science) - no faculty home identified
- CSS 457 (Signal Computing) - no recent offerings
- CSS 477 (Foundations of Secure Software Development) - content in CSS 310, 337; CSS 578 at grad level
- CSS 482 (Expert Systems) - never offered at UWB; content absorbed into modernized CSS 382

**Review with responsible instructor (near-dormant):**
- CSS 448 (Compilers, Hogg/Rahman): No 2025-26 offerings. Is this course continuing? If not, sunset.
- CSS 452 (Game Engine Development, Sung): Last offered WIN2024. Confirm status.
- CSS 484 (Multimedia Data Processing, Chen): Last offered AUT2024. Confirm status.

**Effect of phase-out:** Reduces catalog bloat; signals department priorities; frees advisor mental load; may free teaching capacity if instructors shift to AI-relevant courses.

### 6.5 Faculty Development in 2027-28

#### Moderate Funding
- Continue monthly learning community
- 1-2 additional summer stipends for CSS 4xx support instructors
- AI tool access renewals

#### Generous Funding (adds)
- Second CSS 4xx instructor hired or developed (internal + external)
- Begin development of Phase 3 courses (e.g., AI Safety, Applied Data Science)
- Conference travel for CSS 4xx instructor to present curriculum design work

---

## 7. Phase 3: AY 2028-29+ - Goal State

**Goal:** AI literacy is present at every level of the curriculum, from introductory courses through capstone. The required AI pathway is stable and resilient.

### 7.1 Introductory Level

**CSS 142 (Programming I):** Introduce AI coding tools in the first week as a learning aid. Students explicitly evaluate AI-generated code: find the bugs, explain what it does, then write their own. Frames AI as a tool to understand, not a substitute for learning.

**CSS 101 (Digital Thinking):** Add AI literacy module covering how generative AI works conceptually, societal implications, and how to evaluate AI-generated content critically.

**CSS 107 (Programming through Storytelling):** Use AI generation as a creative context; discuss authorship and attribution in computing.

### 7.2 Goal-State Degree Map

**CSSE BS (Option C implemented):**
```
Year 1:  CSS 142 (AI framing) → CSS 143
Year 2:  CSS 342 + CSS 343 + CSS 301 (AI writing module) + CSS 211 (AI ethics updated)
Year 3:  CSS 360 (SE with AI module) + CSS 350 + CSS 382 (Intro AI, required prereq)
Year 4:  CSS 422 + CSS 430 + CSS 4xx (AI for SE, required) + CSS 497 (AI-aware capstone)
Note:    CSS 370 available as recommended elective
```

**AC BA:**
```
Year 1:  CSS 142 → CSS 143
Year 2:  CSS 340 or 342 + CSS 301 + CSS 211
Year 3:  CSS 360 + CSS 350 + CSS 421 + CSS 382 (recommended prereq)
Year 4:  Concentration + CSS 4xx (required) + CSS 496 (AI-aware capstone)
```

### 7.3 Additional Courses to Consider (2028-29 or later)

These are possibilities for Phase 3 development; do not plan them until Phase 2 is stable.

| Course | Description | Prereqs |
|---|---|---|
| CSS 4yy: AI Safety and Alignment | Technical and policy dimensions of ensuring AI behaves as intended; societal stakes | CSS 4xx + CSS 411 |
| CSS 4zz: Applied Data Science | End-to-end data pipeline for software engineers: collection, cleaning, modeling, deployment, monitoring | CSS 4xx or CSS 486 |
| CSS 4ww: AI Product Design | Cross-functional: building products with AI components; user research, go-to-market, ethics review (possible co-teach with business faculty) | CSS 4xx + CSS 478 |

### 7.4 Two-Course AI Specialization Track

By 2028-29, students who want depth beyond the required CSS 4xx can follow a clear two-course sequence:
```
CSS 382 (Intro AI, foundations) → CSS 4xx (AI for SE, required) → one of: CSS 486 (ML), CSS 487 (CV), CSS 488 (NLP), CSS 444 (Biases)
```
This creates a visible, advise-able AI track within the existing elective structure without requiring a formal concentration.

### 7.5 Capstone Goal State

Every capstone project (CSS 497, CSS 496) by 2028-29 should:
- Include an explicit AI feasibility analysis
- If AI is used in development: include a tool use log with critical reflection
- If the system includes AI components: include a model card or equivalent documentation
- Have at least one team per cohort whose primary focus is an AI-integrated application (encouraged, not required)

### 7.6 What Success Looks Like

By 2028-29, a CSS graduate should be able to:
1. Use AI coding assistants effectively and critically evaluate their output
2. Integrate a cloud AI API (LLM, vision, speech) into a software system with appropriate error handling and evaluation
3. Explain at a conceptual level how transformer-based LLMs work and where they fail
4. Identify and analyze bias in an AI system; produce basic documentation of risks
5. Articulate the legal and ethical responsibilities of a software engineer deploying AI
6. Make an informed argument about when AI is appropriate vs. when traditional algorithmic approaches are better
7. Evaluate AI system performance using appropriate metrics and communicate results to non-technical stakeholders

---

## 8. Resource Requirements Summary

### Phase 1 (2026-27)

| Item | Moderate | Generous |
|---|---|---|
| Summer stipends (course redesign) | 2-3 faculty × $4,000 = $8,000-12,000 | 4-6 faculty × $5,000 = $20,000-30,000 |
| Course release (CSS 4xx developer) | 1 release; adjunct coverage ~$6,000-8,000 | 2 releases; ~$12,000-16,000 |
| Faculty AI Bootcamp | 1 day, ~$3,000-5,000 | 2 days, ~$8,000-12,000 |
| AI tool institutional access | $3,000-5,000/yr | $8,000-12,000/yr |
| Guest lectures | ~$4,000/yr | ~$8,000/yr |
| **Phase 1 total estimate** | **~$24,000-34,000** | **~$56,000-78,000** |

### Phase 2 (2027-28)

| Item | Moderate | Generous |
|---|---|---|
| Summer stipends | 1-2 faculty × $4,000 = $4,000-8,000 | 3-4 faculty × $5,000 = $15,000-20,000 |
| AI-experienced adjunct (new CSS 4xx sections) | 1-2 courses × $6,000-8,000 = $6,000-16,000 | 2-4 courses = $12,000-32,000 |
| AI tool access | $3,000-5,000/yr | $10,000/yr |
| Conference travel | None or 1 faculty | 2-3 faculty × $3,000 = $6,000-9,000 |
| **Phase 2 total estimate** | **~$13,000-29,000** | **~$43,000-71,000** |

*These estimates are rough orders of magnitude for planning purposes. Actual costs depend on specific adjunct arrangements, tool choices, and number of participating faculty.*

---

## 9. Timeline and Milestones

| Milestone | Target Date | Owner |
|---|---|---|
| Confirm AI teaching expertise of Sept 2026 new hires | August 2026 | Dept. Chair |
| Faculty AI skills inventory (survey + chair conversations) | July-August 2026 | Chair + Task Force |
| Deploy student AI readiness survey | Autumn 2026, Week 1 | Curriculum Committee |
| Deploy employer skills survey | October 2026 | Capstone coordinators |
| Faculty AI Bootcamp | August 2026 | Designated organizer |
| Phase 1 course modifications begin | Autumn 2026 | Individual instructors |
| CSS 490 special topics pilots | Winter or Spring 2027 | Volunteer instructor |
| Form Curriculum AI Task Force (3-5 faculty) | September 2026 | Dept. Chair |
| CSS 382 revised syllabus complete | Spring 2027 | CSS 382 instructors |
| CSS 4xx course proposal drafted | February 2027 | Course dev lead |
| CSS 4xx + Option C submitted to curriculum committee | March 2027 | Committee + Chair |
| Phase 1 assessment checkpoint | Spring 2027 | Task Force |
| CSS 382 modernized version launches | Autumn 2027 | CSS 382 instructors |
| CSS 4xx pilot offering | Autumn 2027 | CSS 4xx instructor |
| CSS 4xx as required course (new admits AUT2028+) | AUT2028 | Curriculum Committee |
| Dormant course catalog cleanup complete | AY 2027-28 | Advising + faculty |
| Phase 2 assessment checkpoint | Spring 2028 | Task Force |
| Phase 3 planning workshop | Summer 2028 | Full faculty |
| Goal-state curriculum in place | AY 2028-29 | All faculty |

---

## 10. Risks and Mitigations

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| New hires have no AI teaching expertise | Medium | High | Actively recruit for AI capacity in current search; if gap confirmed, prioritize external AI-experienced adjuncts for CSS 4xx |
| AI landscape changes faster than curriculum can adapt | High | Medium | Principles-focused courses; use CSS 490 for cutting-edge content that changes fast |
| Faculty resist Phase 1 modifications | Medium | Medium | Opt-in framing; stipend incentives; share employer and student survey results to build urgency |
| CSS 4xx curriculum committee approval delayed | Medium | Medium | Submit March 2027 with full documentation; pre-brief committee chair; run pilot via CSS 490 while waiting for approval |
| Single-instructor AI courses remain fragile | High (ongoing) | High | Cross-train at least 2 instructors per AI course by 2028-29; preference for team-taught pilots |
| Course release for CSS 4xx developer cannot be filled by adjunct | Medium | High | Identify qualified adjunct early (Summer 2026); consider teaching overload arrangement with compensation |
| Equity: students without personal AI tool access | Medium | High | All AI course content uses free-tier or institutionally licensed tools; no personal subscription required |
| Option C (CSS 370 demotion) meets strong faculty opposition | Medium | Medium | Present the four options fairly; allow full faculty vote; if Option C fails, re-evaluate Option D or Option A with stronger AI elective requirements |

---

## 11. Open Questions for Faculty Decision

1. **Option C vs. other options:** Do faculty support moving CSS 370 from required to strongly recommended to make room for CSS 4xx? Or is another option preferred?

2. **New hire expertise:** Do the 4 faculty starting September 2026 have AI teaching capability? Who among them could lead CSS 4xx?

3. **CSS 370 during transition:** If Option C is approved, how long does CSS 370 continue to be offered for existing students and by-request for new ones?

4. **CSS 4xx in AC:** Should CSS 4xx be required for all AC students, or required only in certain concentrations?

5. **Dormant course confirmation:** Are there instructors who plan to resume offering CSS 448, CSS 452, or CSS 484? If so, they should not be on the phase-out list.

6. **CSS 488 (NLP) future:** Offered once by one instructor. Should it continue, grow, or be integrated into CSS 4xx as a module?

7. **Funding scenario:** Which funding scenario is the department working toward? This determines the Phase 1 scope.

8. **Task Force formation:** Who volunteers for the Curriculum AI Task Force?

---

*Draft 3 - For faculty vote on the key structural question (Option C vs. alternatives) and for Task Force formation. Decisions made here will be reflected in Draft 4, which will be the version shared with the Dean's office.*
