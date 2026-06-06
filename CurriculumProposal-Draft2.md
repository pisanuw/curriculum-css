# CSS Curriculum Transition Plan: Preparing Graduates for an AI-Transformed Industry

**Version:** Draft 2
**Date:** June 2026
**Audience:** CSS Faculty
**Changes from Draft 1:** Incorporated actual course offering data from schedule records (AUT2020-WIN2026); clarified CSS 382 role (modify AND add new course); added three options for creating room in the required core; moved ABET to a note only; added course activity tiers.

---

## Executive Summary

The computing job market has undergone a structural shift. AI tools now automate a significant portion of the work previously done by junior software engineers, reducing demand for undifferentiated entry-level hires while raising the baseline competency expected of those who are hired. CSS graduates who cannot work effectively alongside AI tools are at a disadvantage; those who understand AI deeply enough to build, evaluate, and responsibly deploy it are in high demand.

This proposal outlines a three-phase curriculum transition covering 2026-27 through 2028-29. The goal is not to replace foundational CS education - algorithms, systems, software engineering, and mathematics remain essential - but to integrate AI throughout the curriculum and ensure every graduate has practical AI fluency.

The three phases are:
- **Phase 1 (2026-27):** Rapid AI content integration into existing courses; pilot special topics; faculty upskilling.
- **Phase 2 (2027-28):** Modernize CSS 382; add new CSS 4xx (AI Systems for Software Engineers); formalize AI as required elective in both programs.
- **Phase 3 (2028-29+):** Goal-state curriculum with AI woven from intro courses through capstone; phase out dormant courses.

---

## 1. Current State: What the Data Shows

### 1.1 Course Activity Tiers (AUT2020 - WIN2026)

Analysis of 6+ years of schedule data reveals four tiers of course activity. This directly informs which courses can absorb new content vs. which may be candidates for phase-out.

**Tier 1 - High Volume Core (offered every term, 5+ sections/year)**

These are the backbone of the program. Any changes here have large student impact and must be carefully managed.

| Course | Sections/yr | Notes |
|---|---|---|
| CSS 142 | ~12 | 4 sections/quarter in peak terms |
| CSS 143 | ~10 | |
| CSS 342 | ~12 | Core gateway |
| CSS 343 | ~10 | |
| CSS 301 | ~14 | Largest by section count |
| CSS 360 | ~12 | Primary SE course |
| CSS 370 | ~7 | Required CSSE core |
| CSS 422 | ~7 | Required CSSE core |
| CSS 350 | ~7 | Required CSSE core |
| CSS 430 | ~7 | Required CSSE core |
| CSS 497 | ~20+ | Variable credit capstone |

**Tier 2 - Active Electives (offered 2-4 times/year, steady)**

These courses are healthy but not dominant. Good candidates for content updates.

| Course | Sections/yr | Notes |
|---|---|---|
| CSS 475 | ~6 | Databases; very active |
| CSS 310 | ~6 | Cybersecurity; active |
| CSS 478 | ~4 | HCI/usability |
| CSS 211 | ~4 | Computers & Society |
| CSS 371 | ~3 | Business of Tech |
| CSS 382 | ~3 | **Intro AI; only 1 section/term but consistent** |
| CSS 432 | ~2 | Networking |
| CSS 385 | ~2 | Game dev |
| CSS 421 | ~2 | Hardware/OS (AC track) |
| CSS 436 | ~1 | Cloud computing |
| CSS 480 | ~2 | HCI (declining from 3 to 1) |

**Tier 3 - Low Volume / Specialist (1 section/year or less)**

These courses serve smaller audiences or are taught by a single faculty member. Vulnerable to disruption if the instructor leaves or changes focus.

| Course | Last yr active | Notes |
|---|---|---|
| CSS 486 | 2025 | Machine Intelligence; sole instructor: Si Dong |
| CSS 485 | 2026 | Neural Networks; Stiber → Rahman (growing) |
| CSS 444 | 2026 | Biases in Digital Data; Mashhadi (very active 2022-26 despite low total) |
| CSS 487 | 2026 | Computer Vision; Olson (gap 2023-2025, returned) |
| CSS 488 | 2025 | NLP; Ali Shiza; offered only once |
| CSS 434 | 2025 | Parallel/Distributed; Fukuda (Autumn only) |
| CSS 449 | 2026 | Algorithm Design; consistent 1/year |
| CSS 461 | 2025 | Project Management; consistent 1/year |
| CSS 451 | 2025 | 3D Graphics; consistent 1/year |
| CSS 458 | 2025 | Simulation; 1/year |
| CSS 481 | 2026 | Web Programming; growing (1→3/year) |

**Tier 4 - Dormant or Near-Dormant (not offered 2025-2026, or never in data)**

These courses exist in the catalog but have little or no recent activity. Candidates for formal phase-out.

| Course | Status | Last seen | Notes |
|---|---|---|---|
| CSS 448 | Near-dormant | AUT2024 | Compilers; ~1/year 2021-2024, nothing in 2025-26 |
| CSS 452 | Near-dormant | WIN2024 | Game Engine Dev; stopped after WIN2024 |
| CSS 484 | Near-dormant | AUT2024 | Multimedia Data Processing; stopped |
| CSS 482 | Never offered | N/A | Expert Systems; not in schedule data at all |
| CSS 130 | Never offered | N/A | Web Media Tech; not offered at UWB |
| CSS 250 | Never offered | N/A | Intro Interaction Design |
| CSS 416 | Never offered | N/A | Ethical Hacking (undergrad) |
| CSS 450 | Never offered | N/A | Computer Graphics |
| CSS 455 | Never offered | N/A | Computational Science |
| CSS 457 | Never offered | N/A | Signal Computing |
| CSS 477 | Never offered | N/A | Foundations of Secure Software Dev |

### 1.2 Key Observation: AI Courses Are Thin

All AI-area courses are Tier 2-3, offered once per term at most, by a small number of instructors:
- CSS 382 (Intro AI): most healthy - 3 instructors have taught it, consistent
- CSS 486 (Machine Intelligence): almost entirely one instructor (Si Dong); no 2024 offering
- CSS 444 (Biases): one instructor (Mashhadi); growing slowly
- CSS 485 (Neural Networks): shifted from Stiber to Rahman; growing
- CSS 487 (Computer Vision): one instructor (Olson); was absent 2023-25
- CSS 488 (NLP): brand new, one offering

**This is a systemic risk.** Our AI curriculum is instructor-dependent. If any one of these faculty leaves or changes focus, entire content areas disappear. The proposal addresses this by creating broader AI integration across many courses, not just isolated specialist electives.

### 1.3 Current Gap: No Required AI Content

A student can complete the CSSE BS or AC BA without encountering any formal AI instruction. CSS 382 is the natural entry point but is optional and offered only once per term.

---

## 2. Guiding Principles

1. **Foundations first.** AI fluency built on a weak CS foundation is brittle.
2. **Principles over tools.** Specific tools will change; teach underlying concepts.
3. **Integration over isolation.** AI woven throughout is more durable than a single "AI course."
4. **Ethics is not optional.** Responsible use is integrated into technical content, not a separate module.
5. **Faculty must be supported.** No mandate without preparation.
6. **Iterate and measure.** Each phase has checkpoints.
7. **Don't create dependency.** Avoid new content that lives or dies with a single instructor.

---

## 3. The Two-Track AI Curriculum Response

Faculty direction: CSS 382 will be **modernized** (not replaced), AND a new course will be created. These serve different purposes:

| | CSS 382 (modernized) | CSS 4xx (new) |
|---|---|---|
| **Level** | 300-level | 400-level |
| **Focus** | Concepts, theory, history of AI | Practical AI integration for software engineers |
| **Audience** | Any CSS major after 340/342 | CSSE seniors and advanced AC students |
| **Content** | How AI systems work: search, ML, neural nets, LLMs | Building *with* AI: APIs, RAG, evaluation, responsible deployment |
| **Current equivalent** | CSS 382 (needs updating) | Nothing - this is the gap |
| **Prereqs** | CSS 340 or CSS 342 | CSS 343; recommended CSS 382 or 486 |

---

## 4. Phase 1: AY 2026-27 - Integration Without Restructuring

**Goal:** Every CSS student encounters AI meaningfully this year. No new course numbers. No changes to degree requirements. Faculty choose their level of engagement.

### 4.1 Required Course Modifications

These are targeted content additions that individual instructors can implement within current course structures.

**CSS 360 (Software Engineering)** - Priority: HIGH
- Add 2-week module: AI-assisted development in practice
  - Using coding assistants (Copilot, Cursor, etc.) with critical judgment
  - When to accept, reject, or modify AI-generated code
  - Testing strategies for AI-assisted code
  - Team AI use policies; documentation expectations
- Update project rubric: teams must document AI tool use in their process log
- Effort: Medium (new assignments, one new lecture block)

**CSS 211 (Computers and Society)** - Priority: HIGH
- Expand AI ethics content from occasional topic to central thread:
  - Generative AI and attribution (who owns AI output?)
  - Automation, labor displacement, and the job market students are entering
  - Algorithmic bias and fairness with 2024-2026 case studies
  - AI in hiring, policing, healthcare, and credit - real harms documented
- Retire outdated case studies; replace with AI-era examples
- Effort: Medium (content refresh, new readings)

**CSS 301 (Technical Writing)** - Priority: MEDIUM
- Add module: writing about AI systems for non-technical audiences
  - How to communicate model limitations, uncertainty, and risks
  - Documentation standards for AI-assisted work (model cards, prompt logs)
  - Evaluating AI-generated text critically
- Update one major assignment to include an AI-assisted writing scenario
- Effort: Low-Medium

**CSS 343 (Data Structures & Algorithms II)** - Priority: LOW-MEDIUM
- Add optional "AI lens" framing at relevant points:
  - Graphs as the structure behind knowledge graphs and neural networks
  - Hash tables as the basis for embedding lookup
  - Tree traversal in decision trees and syntax parsing
- This is conceptual framing, not new algorithms; adds ~1-2 class periods
- Effort: Low

**CSS 350 (Management for Computing Professionals)** - Priority: MEDIUM
- Add material: managing teams that use AI tools
  - IP ownership and code attribution when AI is involved
  - Quality assurance when AI generates deliverables
  - Ethics of disclosing AI use to clients and stakeholders
- Effort: Low

**CSS 370 (Analysis and Design)** - Priority: LOW
- Add: modeling systems that include ML components
  - How do you specify behavior of a model (not deterministic)?
  - How do you document AI component interfaces in UML/ADL?
- Effort: Low (1 lecture + modified assignment)

### 4.2 Capstone Update (CSS 497, CSS 496) - Immediate

Starting Autumn 2026, all capstone projects must include in their documentation:
- An AI feasibility analysis: should this problem use AI? What are the tradeoffs?
- If AI tools were used in development: which tools, for what, what was kept vs. discarded
- If the system incorporates AI components: bias analysis and failure mode documentation

### 4.3 Special Topics Pilots (CSS 390/490)

Use existing special topics slots to pilot content for future new courses. No approval required.

- **"AI Tools for Software Development" (1-2 cr, CR/NC)**: Introduction to AI coding assistants, prompt engineering fundamentals, critical evaluation of AI output. Target: all CSS students. Could be a seminar-style course.
- **"Building with Large Language Models" (3-5 cr)**: LLM API integration, RAG, agents, evaluation. Target: students who have completed CSS 342+. This is a pilot for CSS 4xx.

### 4.4 CSS 382 Modernization (Begin in 2026-27)

CSS 382 is healthy (consistent 2-3 sections/year across 3 instructors) but the content needs updating. Begin the revision process:

**Remove or condense:**
- Expert systems as a standalone topic (CSS 482 is already dormant; this content can become 1 lecture of history)
- Heavy symbolic AI and rule-based system implementation details
- Dated coverage of early neural network architectures as primary content

**Expand:**
- Machine learning foundations: supervised, unsupervised, reinforcement
- Deep learning and transformer architecture at a conceptual level
- Large language models: how they work, what they can and cannot do, how to evaluate them
- AI ethics and societal impact as an integrated thread throughout (not a single lecture at the end)
- Hands-on: students should use real ML libraries and APIs, not just simulate algorithms

Goal: complete revised syllabus by Spring 2027 for adoption Autumn 2027.

### 4.5 Faculty Development in 2026-27

- **Summer 2026 AI Bootcamp (2 days, before Autumn quarter):** Hands-on with AI coding tools, LLM APIs, and pedagogical strategies for teaching AI concepts. Invite 2-3 industry practitioners. All teaching faculty encouraged; incentivized with a stipend.
- **Monthly Faculty AI Learning Community:** Share what's working in course integrations; track student reception; iterate.
- **Designate Course Development Lead:** Identify one faculty member with protected time (course release or summer stipend) to develop the CSS 4xx new course proposal. Target: submitted to curriculum committee by March 2027.
- **Guest Lecturer Series:** 3-4 practitioners per quarter in CSS 490 slots on AI in industry.

---

## 5. Phase 2: AY 2027-28 - Structural Addition

**Goal:** Formalize AI in degree requirements; launch modernized CSS 382 and new CSS 4xx; begin formal phase-out of dormant courses.

### 5.1 CSS 382 Modernization Deployed

Revised CSS 382 launches Autumn 2027. With modernized content, CSS 382 becomes a strong prerequisite or co-listed prerequisite for CSS 4xx.

### 5.2 New Course: CSS 4xx - AI Systems for Software Engineers

**Credits:** 5
**Prerequisites:** CSS 343; CSS 382 or CSS 486 recommended
**Target:** CSSE seniors, advanced AC students
**Proposed first offering:** Autumn 2027 (pilot), Winter 2028 (regular)

**Content outline:**
1. AI as a software component: APIs, SDKs, model hosting
2. Prompt engineering: principles, patterns, evaluation, versioning
3. Retrieval-Augmented Generation (RAG): architecture, chunking, embedding, retrieval
4. Agents and tool use: design patterns, safety, testing
5. Evaluation: metrics (BLEU, ROUGE, human eval), benchmarks and their limits, red-teaming
6. Responsible AI deployment: bias auditing, model cards, explainability methods (LIME, SHAP), regulatory context
7. AI system architecture: latency, cost, reliability, monitoring in production
8. Legal and organizational context: IP ownership, liability, disclosure obligations

**Hands-on project:** Design, build, and evaluate a software application that integrates at least one AI component. Includes a written evaluation report with bias analysis and failure mode documentation.

**Instructor note:** This course requires an instructor familiar with current LLM development practice. Identify primary instructor by Summer 2027; consider joint teaching or guest practitioners for sections.

### 5.3 Making Room: Three Options for Required AI Content

The CSSE required core currently has no space for a new required course. If faculty decide AI content should be required (not just a required elective), one of the following options must be chosen. These are presented for faculty discussion; each involves real tradeoffs.

**Option A - Required Elective (Lowest disruption)**
No change to the required core. Instead, add a requirement to the elective section: "Of the 25 CSS elective credits, at least 5 credits must come from the AI-area course list (CSS 382, CSS 444, CSS 486, CSS 487, CSS 488, or CSS 4xx)."
- Advantage: No courses removed; no ABET impact; implementable immediately
- Disadvantage: Students may choose the easiest AI elective; coverage depth varies; students with heavy cybersecurity or graphics elective loads may feel it as a constraint

**Option B - Absorb into CSS 360 (Minimal structural change)**
Expand CSS 360 from 5 to 8 credits (or add a required 3-credit companion course CSS 361) covering AI-aware software engineering. CSS 360 remains a required course; the AI content is baked in rather than optional.
- Advantage: Every CSSE student gets AI SE content; aligns with industry where AI tools are already in every SE team
- Disadvantage: Increases required credits or requires an existing elective to be dropped; instructor workload increases; CSS 360 is already heavily enrolled (12 sections/year - impact is large)

**Option C - Reduce CSS 370 from required to recommended elective**
CSS 370 (Analysis and Design, 5 cr) covers UML, requirements, and design modeling. In practice, much of this content overlaps with CSS 360 and CSS 350. Moving it from required to a recommended elective frees 5 credits for a required AI course.
- Advantage: Clean 5-credit swap; frees a required slot; CSS 370 remains available for students who want depth in modeling
- Disadvantage: CSS 370 has 42 sections over the data period (active, enrolled course); removing from core is a significant signal; some faculty may feel modeling is still essential; raises the question of what fills the analysis/design gap in the core

**Option D - Reduce CSS 350 scope or merge with CSS 360**
CSS 350 (Management, 5 cr) and CSS 360 (SE, 5 cr) both involve team projects and professional practice. Some content is complementary; some overlaps. A merged or restructured "Software Engineering and Professional Practice" course (8 or 10 credits) could release 2-5 credits.
- Advantage: Reduces redundancy; could modernize both courses simultaneously
- Disadvantage: Complex to implement; both courses have strong teaching histories; requires new unified course proposal

**Recommendation (for discussion):** Begin with Option A in 2027-28, which can be implemented without curriculum committee approval for required courses. Use the 2027-28 data on CSS 4xx enrollment and student outcomes to build the case for Option C or B in 2028-29 if a harder requirement is warranted.

### 5.4 AC Program Update

For the Applied Computing BA:
- Add AI-area elective requirement to the AC elective section (same language as CSSE Option A)
- Strongly encourage concentration advisors to list CSS 382 or CSS 4xx in recommended sequences for all concentrations
- CSS 421 (Hardware/OS for AC) should add brief content on AI hardware considerations (GPUs, TPUs, inference vs. training)

### 5.5 Phase-Out: Dormant Course Catalog Cleanup

The catalog currently lists courses that are never offered. This creates confusion for students and advisors. Formal phase-out process:

**Immediate candidates for catalog removal (never offered at UWB in 6+ years of data):**
- CSS 130 (Web Media Tech) - likely supplanted by CSS 481 (Web Programming)
- CSS 250 (Intro Interaction Design) - likely supplanted by CSS 478
- CSS 416 (Ethical Hacking undergrad) - content covered in CSS 310, 337, 415; graduate equiv is CSS 578
- CSS 450 (Computer Graphics) - CSS 385/451/452 cover this
- CSS 455 (Computational Science) - very niche; no faculty home
- CSS 457 (Signal Computing) - no recent offering
- CSS 477 (Secure Software Dev) - content in CSS 310/337; CSS 578 at grad level
- CSS 482 (Expert Systems) - never offered in UWB data; content absorbed into modernized CSS 382

**Near-dormant - schedule for review with affected instructors:**
- CSS 448 (Compilers) - no offering in 2025-26; only offered by Hogg/Rahman historically; check status
- CSS 452 (Game Engine Dev) - no offering since WIN2024; check with Sung if resuming
- CSS 484 (Multimedia Data Processing) - no offering since AUT2024; check with Chen

**Process:** Before removing any course, confirm with the responsible instructor and check no student has it in an active degree audit as a required elective. Catalog removal is separate from stopping offerings - can stop scheduling while keeping in catalog for audit purposes.

### 5.6 New Course to Consider: CSS 4xx - Responsible AI and Society

If CSS 211 is not sufficient to cover AI ethics depth, a dedicated course could be offered at the upper-division level. This would be co-taught or cross-listed, targeting both CSS majors and non-majors.

**Content:** AI governance, bias and fairness in deployed systems, generative AI and creative rights, AI in high-stakes domains (healthcare, criminal justice, hiring), regulatory landscape, professional ethics obligations.

**Note:** This is a 2028-29 consideration; do not overload Phase 2 with new courses.

---

## 6. Phase 3: AY 2028-29+ - Goal State

**Goal:** AI literacy is as fundamental as programming literacy; woven into every level of the curriculum.

### 6.1 Introductory Level Updates

- **CSS 142 (Programming I):** Introduce AI tools in Week 1 as a learning aid with explicit instructions on how to use them responsibly. Students evaluate AI-generated code - identify bugs, explain what it does, then write their own. Frames AI as a tool to understand, not a substitute for learning.
- **CSS 101 (Digital Thinking):** Add AI literacy module: how generative AI works at a conceptual level, societal implications, evaluating AI-generated content.
- **CSS 107 (Programming through Storytelling):** Use AI image and story generation as creative context; discuss authorship and attribution.

### 6.2 Goal State Degree Map

**CSSE BS (with Option A "required AI elective")**
```
Year 1:  CSS 142 (AI tool context) → CSS 143
Year 2:  CSS 342/343 (alg; AI lens optional) + CSS 301 (AI writing module) + CSS 211 (AI ethics)
Year 3:  CSS 360 (SE with AI module) + CSS 370 + CSS 350 + CSS 382* (required elective)
Year 4:  CSS 422 + CSS 430 + CSS 4xx (AI Systems for SE)* + CSS 497 (AI-aware capstone)

* one of these, or another AI-area course
```

**AC BA**
```
Year 1:  CSS 142 → CSS 143 or 143-equivalent
Year 2:  CSS 342 or 340 + CSS 301 + CSS 211
Year 3:  CSS 360 + CSS 350 + CSS 421 + AI-area elective (CSS 382 or CSS 4xx)
Year 4:  Concentration + CSS 496 (AI-aware capstone)
```

### 6.3 What Success Looks Like

By 2028-29, a CSS graduate should be able to:
1. Use AI coding assistants effectively and critically evaluate their output
2. Integrate a cloud AI API (LLM, vision, speech) into a software system with appropriate error handling and evaluation
3. Explain at a conceptual level how transformer-based LLMs work and what their limitations are
4. Identify and analyze bias in an AI system and document risks
5. Articulate the legal and ethical responsibilities of a software engineer deploying AI
6. Make an informed argument about when AI is appropriate vs. when traditional algorithmic approaches are better
7. Evaluate AI systems using appropriate metrics and communicate results to non-technical stakeholders

---

## 7. Risks and Mitigations

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| AI landscape changes faster than curriculum | High | Medium | Principles-focused courses; use CSS 490 for cutting-edge content |
| Faculty resistance or capacity limits | Medium | High | Opt-in Phase 1; adequate stipends and release time; no mandates without preparation |
| New course has low enrollment | Medium | Medium | Make it a required elective; advise into it from CSS 360 and capstone advisors |
| Single-instructor AI courses break on departure | High | High | Cross-train at least two instructors per AI-area course; integrate AI broadly so it doesn't depend on specialists |
| Equity - not all students have AI tool access | Medium | High | All course AI content uses free-tier or institutionally licensed tools; no personal subscription assumed |
| Catalog bloat causes student confusion | Current | Medium | Execute Phase 2 dormant course cleanup |

**Note on ABET:** CSSE is ABET-accredited. Major changes to required courses should be reviewed against current CAC criteria before submission to curriculum committee. However, ABET accreditation is not a barrier to content updates within existing courses (Phase 1) or adding new electives (Phase 2 Option A). Formal required-course restructuring (Options B-D) should be reviewed with the ABET coordinator.

---

## 8. Timeline

| Milestone | Target Date | Owner |
|---|---|---|
| Faculty AI skills inventory survey | July 2026 | Dept. Chair |
| Student AI readiness survey | Sept 2026 (Autumn week 1) | Curriculum Committee |
| Employer/industry partner survey | Oct 2026 | Capstone coordinators |
| Faculty AI Bootcamp | August 2026 | Designated organizer |
| Phase 1 course modifications begin | Autumn 2026 | Individual instructors |
| CSS 490 special topics pilot | Winter or Spring 2027 | Volunteer instructor |
| CSS 382 syllabus revision complete | Spring 2027 | CSS 382 instructors |
| CSS 4xx course proposal drafted | February 2027 | Course dev lead |
| CSS 4xx submitted to curriculum committee | March 2027 | Curriculum Committee |
| Phase 1 assessment checkpoint | Spring 2027 | Task Force |
| CSS 382 modernized version launches | Autumn 2027 | CSS 382 instructors |
| CSS 4xx first offering (pilot) | Autumn 2027 | CSS 4xx instructor |
| CSSE/AC AI elective requirement added | AY 2027-28 | Curriculum Committee |
| Dormant course catalog cleanup | AY 2027-28 | Advising + affected faculty |
| Phase 2 assessment checkpoint | Spring 2028 | Task Force |
| Phase 3 planning workshop | Summer 2028 | Full faculty |
| Goal-state curriculum implemented | AY 2028-29 | All faculty |

---

## 9. Questions for Faculty Discussion

1. **CSS 4xx vs. CSS 382:** Do faculty agree with the two-track approach (modernize 382 AND create new 4xx for practical AI integration)? Who is positioned to teach CSS 4xx by Autumn 2027?

2. **Required AI content:** Which Option (A-D in Section 5.3) do faculty favor for creating room in the CSSE required core? Or is Option A (required elective) sufficient?

3. **CSS 370 status:** Would faculty support moving CSS 370 from required to recommended elective (Option C)? What would be lost?

4. **Dormant course cleanup:** Are there any courses on the Tier 4 list that faculty believe should be retained and scheduled? If so, who would teach them?

5. **Faculty capacity:** Which instructors are willing to pilot Phase 1 modifications in Autumn 2026? Who could lead the CSS 4xx course development?

6. **CSS 488 (NLP):** This was offered only once (SPR2025). Is it continuing? Should it be developed further or folded into CSS 4xx as a module?

7. **Assessment:** How will the department measure whether changes are producing intended outcomes? Who is responsible for tracking placement rates and employer feedback year over year?

---

*Draft 2 - For faculty discussion. All sections are provisional until faculty decisions are made on the open questions in Assumptions.md.*
