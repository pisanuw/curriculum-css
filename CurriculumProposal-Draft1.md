# CSS Curriculum Transition Plan: Preparing Graduates for an AI-Transformed Industry

**Version:** Draft 1 (for faculty discussion)
**Date:** June 2026
**Audience:** CSS Faculty
**Status:** Working draft - requires data collection and faculty input before finalizing

---

## Executive Summary

The computing job market has undergone a structural shift. AI tools now automate a significant portion of the work previously done by junior software engineers - boilerplate code generation, basic debugging, documentation, simple testing - reducing demand for undifferentiated entry-level hires while simultaneously raising the baseline competency expected of those who are hired. CSS graduates who cannot work effectively alongside AI tools are at a disadvantage; those who understand AI deeply enough to build, evaluate, and responsibly deploy it are in high demand.

This proposal outlines a three-phase curriculum transition covering 2026-27 through 2028-29. The goal is not to replace foundational CS education - algorithms, systems, software engineering, mathematics remain essential - but to integrate AI throughout the curriculum and ensure every graduate has practical AI fluency alongside their technical depth.

The three phases are:
- **Phase 1 (2026-27):** Rapid integration of AI content into existing courses; minimal structural change; faculty upskilling begins.
- **Phase 2 (2027-28):** Structural additions including new or significantly revised courses; AI content formalized in required curriculum.
- **Phase 3 (2028-29+):** Goal-state curriculum with AI as a first-class thread throughout the degree.

---

## 1. Current State Assessment

### 1.1 What the Current Curriculum Does Well

The CSSE and AC programs provide a rigorous foundation:
- Strong algorithms and data structures sequence (CSS 342/343)
- Systems depth (CSS 422 hardware, CSS 430 OS)
- Software engineering process (CSS 360, CSS 370)
- Professional communication (CSS 301, CSS 350)
- Existing AI electives (CSS 382, 486, 487, 488) for interested students

### 1.2 Current Gaps

**AI is entirely optional.** A student can graduate from either program without encountering any formal AI content. This was acceptable when AI was a specialized subfield; it is not acceptable when AI tools are used daily in industry software development.

**Ethics and societal impact coverage is siloed.** CSS 211 and CSS 411 cover computing's social implications, but AI-specific ethical issues (bias, explainability, autonomy, generative AI misuse) are not systematically addressed.

**Prompt engineering and LLM integration are absent.** No current course teaches students how to effectively use, evaluate, or build applications on top of large language models - the dominant AI paradigm as of 2026.

**Data literacy is thin in the required core.** Students can graduate without meaningful exposure to data pipelines, statistical reasoning applied to model evaluation, or working with real datasets.

**The capstone does not require AI engagement.** Industry capstone sponsors increasingly use AI tools in their workflows; our capstone project expectations have not caught up.

---

## 2. Guiding Principles

1. **Foundations first.** AI fluency built on a weak CS foundation is brittle. Algorithms, data structures, and systems remain in the required core.

2. **Principles over tools.** Specific AI tools will change; courses must teach underlying concepts (how transformers work, what bias means statistically, how to evaluate a model) that outlast any particular product.

3. **Integration over isolation.** AI should be woven into existing courses where natural, not confined to one "AI course" that can be skipped.

4. **Ethics is not optional.** Every course with AI content must include responsible use, limitations, and potential harms - not as a separate module but as integral to the technical content.

5. **Faculty must be supported.** Curriculum change without faculty development is unfair and ineffective. Professional development resources must accompany this proposal.

6. **Iterate and measure.** Each phase should include assessment checkpoints. If a change is not producing the intended outcomes, adjust rather than doubling down.

---

## 3. Phase 1: AY 2026-27 - Integration and Foundation

**Goal:** Within existing course structures, ensure every CSS student encounters AI in a meaningful way. No new course numbers; no change to degree requirements. Changes can begin immediately.

**Mechanism:** Targeted content additions to existing required courses, opt-in faculty pilots, and professional development.

### 3.1 Modifications to Required Courses

| Course | Current Focus | Proposed AI Addition | Effort Level |
|---|---|---|---|
| CSS 360 (Software Engineering) | SDLC, testing, process | Add module: AI-assisted development (Copilot/LLM coding assistants), when to trust AI-generated code, testing AI-assisted code; update project requirements to reflect AI tool use policies | Medium |
| CSS 370 (Analysis and Design) | UML, requirements, modeling | Add module: requirements analysis in AI-integrated systems; designing systems that incorporate ML components; documenting AI system behavior | Low |
| CSS 343 (Data Structures/Alg II) | Trees, graphs, hash tables | Add examples: how AI systems use these structures (knowledge graphs, embeddings, search); optional: compare brute-force vs. heuristic approaches | Low |
| CSS 350 (Management) | Team dynamics, project management | Add: managing AI tool use in teams; intellectual property and code ownership with AI assistance; documentation standards when AI is involved | Low |
| CSS 301 (Technical Writing) | Technical communication | Add: writing about AI systems and their limitations; prompt documentation; communicating uncertainty and model behavior to non-technical stakeholders | Low |
| CSS 211 (Computers and Society) | Privacy, ethics, IP, labor | Expand: AI-specific ethics (bias, fairness, explainability, automation and labor displacement, generative AI and attribution); case studies from 2024-2026 | Medium |

### 3.2 Modifications to Elective Courses

| Course | Proposed Change |
|---|---|
| CSS 475 (Database Systems) | Add module on vector databases and embedding storage, which are foundational to RAG (retrieval-augmented generation) systems |
| CSS 432 (Networking) | Add discussion of distributed AI inference, model serving infrastructure |
| CSS 444 (Biases in Digital Data) | Expand from statistical bias to LLM bias and fairness in generative AI; update datasets used |
| CSS 480 (HCI) | Add: UX for AI-integrated interfaces; communicating AI confidence and uncertainty to users; designing for human-AI collaboration |

### 3.3 Capstone Update (CSS 497, CSS 496)

Beginning Autumn 2026, capstone project rubrics should include:
- A section requiring teams to document their AI tool use (what tools, how used, what was accepted vs. rejected and why)
- At least one design decision explicitly analyzing an AI-assisted vs. manual approach
- Projects proposing to build AI-integrated systems must include bias and failure mode analysis

### 3.4 Faculty Development in 2026-27

- **AI Tool Bootcamp (Summer 2026):** One to two day workshop for all teaching faculty on current AI coding assistants, prompt engineering, and pedagogical approaches to AI in CS courses. Invite industry practitioners.
- **Learning Community:** Monthly faculty lunch meeting to share what's working and what isn't as integration experiments run.
- **Course Release or Stipend:** At least one faculty member should receive support to develop the new 400-level AI course proposed in Phase 2.
- **Guest Lecturer Series:** Invite 3-4 practitioners per quarter to speak in CSS 390/490 special topics slots about AI in industry contexts.

### 3.5 New Offering: CSS 390/490 Special Topics on AI

Immediately leverage the existing special topics mechanism to offer:
- "AI Tools for Software Development" (introductory, 1-2 credits, credit/no credit option)
- "Large Language Models: How They Work and When They Fail" (3-5 credits, for students with CSS 342)

These do not require curriculum committee approval and can pilot in Winter or Spring 2027.

---

## 4. Phase 2: AY 2027-28 - Structural Addition

**Goal:** Formalize AI content in the degree requirements; introduce new course(s) that reflect Phase 1 learnings; begin phasing out low-value courses.

**Mechanism:** New course creation (requires curriculum committee approval, submit by Spring 2027 for Autumn 2027 launch); modification of elective requirements to include AI.

### 4.1 New Course: CSS 4xx - AI Systems for Software Engineers

**Proposed credits:** 5
**Proposed prerequisites:** CSS 343; recommended CSS 382 or CSS 486
**Target audience:** CSSE seniors and AC advanced students; also valuable for graduate students without undergrad AI background

**Content:**
- Practical LLM integration: APIs, prompt engineering, retrieval-augmented generation (RAG), agents
- Building applications on top of AI components: design patterns, testing, evaluation
- Model evaluation: metrics, benchmarks, the limits of benchmarks
- Responsible AI: bias auditing, explainability methods (LIME, SHAP), documentation standards (model cards)
- Organizational and legal context: IP ownership of AI output, liability, regulatory landscape (EU AI Act, US executive orders)
- Hands-on project: build and evaluate a software system that integrates an AI component

**Rationale:** This course is distinct from CSS 382 (theoretical AI) and CSS 486 (ML algorithms). It targets students who will use AI systems as components, not those who will research AI algorithms. It is the most directly applicable to the current job market gap.

**Phase 2 curriculum committee actions needed:**
1. Submit CSS 4xx for approval (Spring 2027 target)
2. Add language to CSSE and AC elective requirements: "At least one AI-area elective required" (CSS 382, 444, 485, 486, 487, 488, or CSS 4xx)
3. Update CSS 382 to modernize content (deep learning and LLMs now dominate; historical AI approaches like expert systems and symbolic reasoning can be reduced to historical context)

### 4.2 Course Review: Candidates for Phase-Out or Consolidation

The following courses should be reviewed. Phase-out does not mean immediate deletion - courses can be "sunset" (no new sections scheduled) while continuing to exist in the catalog for students already enrolled.

| Course | Issue | Recommendation |
|---|---|---|
| CSS 482 (Expert Systems) | Expert systems as a standalone paradigm are largely superseded; content now belongs in a historical survey within CSS 382 | Sunset; absorb key concepts into CSS 382 update |
| CSS 484 (Multimedia Data Processing) | Low enrollment; content overlaps with signal processing and ML courses | Review enrollment; if consistently < 10 students, sunset; move relevant content to CSS 457 or new 4xx course |
| CSS 483 (Bioinformatics Algorithms) | Niche; may be better housed as a joint offering | Keep but consider joint offering with Biology or as a CSS 490 special topics |

**Note:** Before sunsetting any course, verify enrollment data (last 5 years) and ensure no students have it on their degree audit as a required elective. Faculty who primarily teach these courses must be involved in the conversation.

### 4.3 CSS 382 Modernization

CSS 382 (Introduction to AI) is well-positioned as the entry point to the AI elective cluster but needs modernization:
- Reduce or condense symbolic AI, expert systems, and early search algorithms to historical context
- Add substantial coverage of machine learning (supervised, unsupervised, reinforcement)
- Add practical content on modern LLMs, diffusion models, and multimodal AI
- Add ethics and societal impact as integrated thread, not separate lecture
- Consider co-listing with a graduate section (CSS 582 modernization) to enable small cohorts

### 4.4 Sequence Clarification for AC Students

The AC program's flexibility is a strength but can leave students without AI exposure. In 2027-28:
- Add AI-area elective requirement to the AC elective section (same language as CSSE above)
- Consider adding CSS 360 (Software Engineering) as required for AC (currently required; verify this) to ensure all AC students get the Phase 1 CSS 360 AI integration
- Encourage AC concentration advisors to include CSS 444, CSS 486, or CSS 4xx in recommended paths for every concentration

---

## 5. Phase 3: AY 2028-29+ - Goal State Curriculum

**Goal:** A curriculum where AI literacy is as fundamental as programming literacy - present at every level, from introductory courses through capstone.

**Note:** This section is explicitly speculative and should be revisited after Phase 1 and 2 data are available.

### 5.1 Introductory Level

- **CSS 142 (Computer Programming I):** Introduce AI tools in the first week as a context-setting exercise (what can AI code do, what can it not do). Assign students to evaluate AI-generated code, not just write their own. This positions AI as a tool to understand, not a replacement for learning.
- **CSS 107 (Programming through Storytelling):** Use AI image and story generation as a creative tool; discuss authorship and attribution.
- **CSS 101 (Digital Thinking):** Update to include AI literacy - how generative AI works at a conceptual level, societal implications, how to evaluate AI claims.

### 5.2 Intermediate Level

- **CSS 342 (Data Structures & Algorithms I):** Add optional AI lens: how neural networks are graphs, how embedding lookup is a hash table operation, how transformers use attention as a weighted graph traversal.
- **CSS 360 (Software Engineering):** By this phase, a full module (2-3 weeks) on engineering AI-integrated systems, testing ML components, and responsible deployment should be standard, not a pilot.

### 5.3 New or Restructured Advanced Courses (2028-29 possibilities)

| Course | Description |
|---|---|
| CSS 4xx: AI Safety and Alignment (new) | Technical and policy dimensions of ensuring AI systems behave as intended; prerequisites CSS 4xx AI Systems for SE + CSS 411 |
| CSS 4xx: Applied Data Science (new or evolved from CSS 444) | End-to-end data science pipeline for software engineers; data collection, cleaning, feature engineering, model training, deployment, monitoring |
| CSS 4xx: AI Product Development (new) | Cross-functional course (co-taught with business or policy faculty?) on building products with AI components; addresses go-to-market, ethics review, user research |
| CSS 360 → CSS 360/361 split | Split Software Engineering into a core course + a separate AI-integrated SE course (361) required for advanced students |

### 5.4 Capstone Goal State

By 2028-29, every capstone project (CSS 497, CSS 496) should:
- Include an AI feasibility analysis (should this problem use AI? what are the tradeoffs?)
- If AI is used, include a model card or equivalent documentation
- Demonstrate student ability to critically evaluate AI-generated artifacts, not just produce them
- Have at least one team present a project that is primarily AI-integrated (not require it, but actively encourage it)

### 5.5 Goal State Degree Map (CSSE)

```
Year 1: CSS 142 (intro programming, AI as tool context) → CSS 143
Year 2: CSS 342/343 (algorithms, AI lens optional) + CSS 211 (AI ethics integrated)
         + CSS 301 (writing about AI systems)
Year 3: CSS 360 (SE with AI module) + CSS 370 + CSS 350 (managing AI-assisted teams)
         + CSS 382 or CSS 4xx AI Systems (required elective)
Year 4: CSS 422 + CSS 430 + AI-area elective(s) + CSS 497 (AI-aware capstone)
```

---

## 6. What Success Looks Like

By 2028-29, a CSS graduate should be able to:
1. Use AI coding assistants effectively and critically evaluate their output
2. Integrate a cloud AI API (LLM, vision, speech) into a software system with appropriate error handling and evaluation
3. Explain at a conceptual level how transformer-based LLMs work, including their limitations
4. Identify and analyze bias in an AI system and document risks
5. Articulate the legal and ethical responsibilities of a software engineer deploying AI
6. Make an informed argument about when to use AI vs. traditional algorithmic approaches
7. Evaluate and compare AI systems using appropriate metrics

---

## 7. Questions for Faculty Discussion

The following are open questions that faculty should discuss and resolve before the proposal is finalized:

1. **Scope of required AI content:** Should CSS 4xx (AI Systems for SE) become a required course for CSSE, or remain a required elective? What would have to leave the required core to make room?

2. **CSS 382 vs. new course:** Should the department modernize CSS 382 to fill the role of "AI Systems for SE," or create a separate new course with a different focus and prerequisite level?

3. **AC program differentiation:** The AC program is more flexible but may need a stronger AI signal to be competitive. Should AC add a mandatory AI elective or a required AI course to the core?

4. **Faculty capacity:** Which faculty members are positioned to teach new or modified AI courses by Autumn 2027? What professional development support is needed?

5. **Ethical AI as standalone vs. integrated:** Is a standalone ethics course needed, or is integrated ethics (in every course with AI content) sufficient? Some programs are adding dedicated "AI Ethics" courses.

6. **Industry advisory input:** Has the department's industry advisory board weighed in on what skills are most urgently needed? If not, who will lead that outreach?

7. **Graduate program coordination:** Graduate courses (CSS 581, 582, 586) are ahead of the undergrad program in AI depth. How do we prevent duplication and enable undergrads to take graduate AI courses as electives?

8. **Assessment:** How will the department measure whether these changes are producing the intended outcomes? (Employer surveys, graduation rates, first-job placement, alumni follow-up after 2 years?)

---

## 8. Proposed Timeline

| Milestone | Date |
|---|---|
| Faculty AI skills inventory survey | July 2026 |
| Student AI readiness survey | September 2026 (start of Autumn) |
| Employer/industry partner survey | October 2026 |
| Faculty AI bootcamp | August 2026 (before Autumn quarter) |
| Phase 1 course modifications begin | Autumn 2026 |
| Phase 1 special topics offerings | Winter/Spring 2027 |
| Draft new CSS 4xx course proposal | February 2027 |
| Curriculum committee submission for new course | March 2027 |
| Phase 1 assessment checkpoint | Spring 2027 |
| New CSS 4xx course offered (pilot) | Autumn 2027 |
| CSS 382 modernization complete | Autumn 2027 |
| CSSE/AC elective requirement updated (AI area) | AY 2027-28 |
| Phase 2 assessment checkpoint | Spring 2028 |
| Phase 3 planning workshop | Summer 2028 |
| Goal-state curriculum in place | AY 2028-29 |

---

## 9. Risks and Mitigations

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| AI landscape changes faster than curriculum can adapt | High | Medium | Design courses around principles, not tools; use special topics (CSS 390/490) for cutting-edge content |
| Faculty resistance or capacity constraints | Medium | High | Opt-in Phase 1 pilots; adequate professional development support; do not mandate content without preparation |
| ABET constraints block required course changes | Medium | High | Consult ABET coordinator early; frame AI integration as meeting existing ABET outcomes, not adding new requirements |
| New course has low enrollment (students don't choose it) | Medium | Medium | Make it a required elective; market it via capstone advisors and career center |
| Industry moves faster than a 3-year plan | High | Low | Annual review mechanism; Phase 3 is explicitly provisional |
| Equity concerns (students without personal AI tool access) | Medium | High | Ensure all AI-integrated course content uses free-tier or institutionally licensed tools; do not assume personal subscriptions |

---

## 10. Next Steps

**Immediate (before Autumn 2026):**
- [ ] Form a Curriculum AI Task Force (3-5 faculty volunteers + department chair)
- [ ] Design and deploy the three surveys (faculty, student, employer) - see Assumptions.md
- [ ] Identify faculty willing to pilot Phase 1 modifications in Autumn 2026
- [ ] Plan faculty AI bootcamp for August 2026
- [ ] Identify who will draft the CSS 4xx course proposal

**Autumn 2026:**
- [ ] Launch Phase 1 modifications in participating courses
- [ ] Launch CSS 390/490 special topics pilot
- [ ] Begin collecting employer interview data

**Winter 2027:**
- [ ] First faculty assessment checkpoint: what's working in Phase 1?
- [ ] Draft CSS 4xx course proposal
- [ ] Survey first cohort of students in modified courses

**Spring 2027:**
- [ ] Submit CSS 4xx to curriculum committee
- [ ] Present Phase 1 results to full faculty
- [ ] Plan Phase 2 in detail based on data

---

*This document is a working draft and should be revised after the information-gathering activities in Section 7 of Assumptions.md are complete. Faculty are encouraged to annotate, question, and revise any section.*
