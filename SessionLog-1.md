# Develop CSS curriculum plan integrating AI education

**Session:** `bc75044a-4bb2-4671-83ca-056ceb1fddee`  
**Project:** `Users/pisan/bitbucket/pisanuw/curriculum-css`  
**Date:** 2026-06-06 10:56 UTC  

---

## User

/init

<details>
<summary>/init steps</summary>

# /init — Entry Protocol

Run this at the start of every session. Do not proceed with any task until complete.

## Steps

1. Check if `./BRIEFING.md` exists (list or stat). Check if `./CHANGES.md` exists.

2. If `BRIEFING.md` is missing, create it with:

```markdown
# Briefing

- Purpose:
- Current scope:
- Key decisions:
- Non-goals:
```

3. If `CHANGES.md` is missing, create it with:

```markdown
# Changes

Format: `YYYY-MM-DD [type] description` (max 200 chars). Types: decision, plan, doc, scope, code, note.

YYYY-MM-DD [note] Initialized.
```

(Use today's date.)

4. Read `BRIEFING.md` completely.

5. Read `CHANGES.md` (at least the last 30 lines).

5. Output exactly this, then stop:

```
OK. Ready.
BRIEFING.md: <one-sentence summary of current briefing>
CHANGES.md: <one-sentence summary of recent changes>
```

Do not proceed with any other task until this output is complete.

</details>

<details>
<summary>Assistant (6 steps)</summary>

Checking for BRIEFING.md and CHANGES.md.

**Tool: Bash**
*Check if BRIEFING.md and CHANGES.md exist*
```bash
ls /Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md /Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md 2>&1
```

<details><summary>Tool Result</summary>

**Error:**
```
Exit code 1
ls: /Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md: No such file or directory
ls: /Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md: No such file or directory
```

</details>


Creating both files.

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md`
```md
# Briefing

- Purpose:
- Current scope:
- Key decisions:
- Non-goals:

```

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md`
```md
# Changes

Format: `YYYY-MM-DD [type] description` (max 200 chars). Types: decision, plan, doc, scope, code, note.

2026-06-06 [note] Initialized.

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md (file state is current in your context — no need to Read it back)
```

</details>


<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md (file state is current in your context — no need to Read it back)
```

</details>


OK. Ready.
BRIEFING.md: Empty template just created (purpose, scope, decisions, non-goals not yet filled in).
CHANGES.md: Initialized today (2026-06-06); no prior entries.

</details>

## User

Advances in AI have had significant impact on companies. As companies try to restructure, the types of jobs at companies are changing. It has become much harder for computer science graduates to find internships and entry level positions.

The goal is to develop a multi-year plan on how CSS Department at UW Bothell can modify its curriculum to equip graduates with the necessary skills in this changing environment. Some courses may need to be modified to integrate AI (usage, ethics, underlying technologies, etc). Other courses may need to be phased out over time, and of course new courses will need to be introduced as necessary.

The audience for this document is CSS Faculty.

Some of the initial material under ./sources
 - syllabusses from several quarters
- course descriptions
- curriculum requirements for CSSE and AC

First, determine what other infromation needs to be collected to understand the landscape

Next, try to list the assumptions or decisions that would need to be made in creating a multi-year curriculum change proposal

Finally, putting together a proposal with guidance on how courses could change in 26-27, how additional changes can be incorporated in 27-28 and a goal curriculum that might be in place for 28-29 or possibly later.

Additional information that might be worth downloading

CSS Website: https://www.uwb.edu/stem/about/departments/css
UWB Mission & Vision Statement: https://www.uwb.edu/about/mission-vision
About UWB: https://www.uwb.edu/about
ACM Curricula Guidelines: https://www.acm.org/education/curricula-recommendations - This might be outdated and not as relevant due to advances in AI

Ask questions, record assumptions into Assumptions.md file, start with a draft document and iterate multiple times, suggest surveys or other information gathering activities that might be necessary to put together a solid transition plan and a concrete final curriculum

<details>
<summary>Assistant (29 steps)</summary>

Let me start by surveying the sources directory and fetching the external URLs in parallel.

**Tool: Bash**
*List all files in sources directory*
```bash
find /Users/pisan/bitbucket/pisanuw/curriculum-css/sources -type f | sort
```

<details><summary>Tool Result</summary>

```
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/.DS_Store
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/course-descriptions.html
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-ac.html
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-csse.html
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/B IMD 233 A Aut21_Dame_Stephen.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/B IMD 250 A Aut 21_Dailey_Dharma.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/B IMD 351 A Aut21_Gregory_Wanda.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/B IMD 481 Aut21_Chen_Mark.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/B IMD 491 A Aut21_Gregory_Wanda.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/BCORE 107 D Aut21_ Stiber_Michael.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 101 A Aut21_Kim_Jeffrey.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 107 A Aut21_Oliver_Dawn_Marie.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 107 B Aut21_Oliver_Dawn_Marie.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 112 Aut21_Gunnerson_Kim.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 132 A Aut21_Pisan_Yusuf.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 142 A Aut21_ Gunnerson_Kim.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 142 B Aut21_Kim_Jeffrey.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 142 C Aut21 _Ong_Hansel.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 142 D Aut21_Pisan_Yusuf.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 143 A Aut21_Kalmin_Lesley.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 143 B Aut21_Kalmin_Lesley.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 211 A Aut 21_Lin_Johnny.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 295 A Aut 21_Retik_Arkady.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 301 A Aut21_ Oliver_Dawn_Marie.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Autumn 2021/CSS 301 B Aut21_Kool_Nancy.pdf

... (218 lines omitted) ...

/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 490 D Wi 22 Folsom_T.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 496 A Wi 22 Kochansky_M.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 502 A Wi 22_Chen_M.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 502 B Wi22_Olson_C.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 507 A Wi 22_Brechner_E.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 507 B Wi 22_Kim_J & Socha_D.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 519 A Wi 22_Leblanc_D.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 535 A Wi22_Parsons_E.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 537 A Wi 22_Thamilarasu_G.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 539 A Wi 22 Lagesse_B.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 555 A Wi 22 Hamdan_O.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 565 A Wi 22 Erdly_B.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 584 A Wi 22 Chen_M.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSS 586 A Wi 22 Si_D.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 133 A Wi 22_Khobragade_M.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 142 A Wi 22_Khobragade_M.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 142 B Wi 22_Suse_S.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 142 C Wi 22_Kline-Sharpe_C.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 142 D Wi 22 Behdarvandian_P.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 143 A Wi 22 Kline-Sharpe_C.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 143 B Wi 22 Behdarvandian_P.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 143 C Wi 22 Suse_S.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 342 A Wi 22 Sung_K.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 511 A Wi 22 Kool_N.pdf
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/syllabuses/Winter 2022/CSSSKL 594 A Wi 22 Oliver_D.pdf
```

</details>


**Tool: ToolSearch**
```json
{
  "query": "select:WebFetch",
  "max_results": 1
}
```

<details><summary>Tool Result</summary>

```
{'type': 'tool_reference', 'tool_name': 'WebFetch'}
```

</details>


Now let me read the curriculum files and fetch the external URLs in parallel.

**Tool: Read**
Reading `/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/course-descriptions.html`

<details><summary>Tool Result</summary>

```
1	<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
2	
3	
4	<html>
5	
6	<head>
7	
8	<meta http-equiv='Content-Type' content='text/html;charset=utf-8'>
9	
10	<title>COMPUTING &amp; SOFTWARE SYSTEMS</title>
11	
12	<link rel='stylesheet' href='/home/home.css' type='text/css'>
13	
14	<script type='text/javascript'>var _gaq=_gaq || [];_gaq.push(['_setAccount','UA-39299338-3']);_gaq.push(['_trackPageview']);(function(){var ga=document.createElement('script');ga.type='text/javascript';ga.async=true;ga.src=('https:'==document.location.protocol?'https://ssl':'http://www')+'.google-analytics.com/ga.js';var s=document.getElementsByTagName('script')[0];s.parentNode.insertBefore(ga,s);})();</script>
15	
16	</head>
17	
18	<body>
19	
20	
21	
22	
23	
24	 
25	

... (221 lines omitted) ...

247	<a name="css593"><p><b>CSS 593 Cybersecurity Engineering Capstone ([1-5]-, max. 10)</b><br/>Students apply their knowledge and skills related to cybersecurity engineering in a culminated capstone project. Prerequisite: minimum grade of 2.7 in each of CSS 514, CSS 517, CSS 519, CSS 527, CSS 537, CSS 577, and CSS 578.<br/><a href="https://myplan.washington.edu/course/#/courses/CSS593" target="_blank">View course details in MyPlan: CSS 593</a></p></a>
248	<a name="css595"><p><b>CSS 595 Master's Project ([1-10]-, max. 40)</b><br/>Students apply their knowledge and skills related to computer science and software engineering in a culminating capstone project. Credit/no-credit only.<br/><a href="https://myplan.washington.edu/course/#/courses/CSS595" target="_blank">View course details in MyPlan: CSS 595</a></p></a>
249	<a name="css599"><p><b>CSS 599 Faculty Research Seminar (1)</b><br/>Weekly seminars on current research topics in computer science, software engineering, or cybersecurity engineering.<br/><a href="https://myplan.washington.edu/course/#/courses/CSS599" target="_blank">View course details in MyPlan: CSS 599</a></p></a>
250	<a name="css600"><p><b>CSS 600 Independent Study or Research (1-10, max. 30)</b><br/>Independent study or research on computing topics conducted under the direction of one or more instructors. Offered: AWSpS.<br/><a href="https://myplan.washington.edu/course/#/courses/CSS600" target="_blank">View course details in MyPlan: CSS 600</a></p></a>
251	<a name="css601"><p><b>CSS 601 INTERNSHIP (1-5, max. 10)</b><br/>Graduate internship under the supervision of a CSS faulty member.<br/><a href="https://myplan.washington.edu/course/#/courses/CSS601" target="_blank">View course details in MyPlan: CSS 601</a></p></a>
252	<a name="css700"><p><b>CSS 700 Master's Thesis (*-)</b><br/><a href="https://myplan.washington.edu/course/#/courses/CSS700" target="_blank">View course details in MyPlan: CSS 700</a></p></a>
253	
254	<div id="footer"><div id="footerseal">
255	<a href="http://www.washington.edu/"><img src="/home/graphics/blockw.gif" width="53" height="37" alt="UW Logo" /></a>
256	</div>
257	<div id="addressright"></div>
258	<div id="address"><ADDRESS>
259	Bothell Course Descriptons<br>
260	uwbsa@u.washington.edu<br>
261	Modified: June 4, 2026
262	</ADDRESS>
263	</div>
264	</div>
265	
266	
267	</body>
268	
269	</html>
270	<!--Created by chtml 1.47 on Jun 4, 2026 8:58am-->
271	
```

</details>


**Tool: Read**
Reading `/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-csse.html`

<details><summary>Tool Result</summary>

**Error:**
```
File content (304.4KB) exceeds maximum allowed size (256KB). Use offset and limit parameters to read specific portions of the file, or search for specific content instead of reading the whole file.
```

</details>


**Tool: Read**
Reading `/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-ac.html`

<details><summary>Tool Result</summary>

**Error:**
```
File content (303.6KB) exceeds maximum allowed size (256KB). Use offset and limit parameters to read specific portions of the file, or search for specific content instead of reading the whole file.
```

</details>


**Tool: WebFetch**
`https://www.uwb.edu/stem/about/departments/css`

**Tool: WebFetch**
`https://www.uwb.edu/about/mission-vision`

<details><summary>Tool Result</summary>

```
# UW Bothell Mission and Vision

## Mission Statement
"UW Bothell holds the student-faculty relationship to be paramount. We provide access to excellence in higher education through innovative and creative curricula, interdisciplinary teaching and research, and a dynamic community of multicultural learning."

The institution also commits to nine specific goals, including serving diverse student populations, developing critical thinking skills, recruiting distinguished faculty, and fostering inclusive community learning.

## Vision Statement
"The University of Washington Bothell will be a transformational learning community. We will serve as a catalyst to enhance the quality of life throughout our region."

The university aspires to become recognized for cross-disciplinary scholarship and attract highly motivated, diverse students alongside exceptional faculty and staff members.

## Core Values
The institution emphasizes three foundational principles:

1. **Transformational Education** — Providing challenging programs and innovative instruction that foster lifelong learning
2. **Engaged Scholarship** — Supporting rigorous, innovative research that transcends traditional disciplines and benefits the community
3. **Inclusive Culture** — Promoting collaboration across differences while valuing flexibility and multiple perspectives
```

</details>


<details><summary>Tool Result</summary>

```
# Department of Computing & Software Systems - Overview

## Department Mission & Philosophy
The Department of Computing & Software Systems (CSS) emphasizes "software engineering-oriented computer science degrees" focused on creating quality systems with real-world impact. The department aims to provide a "transformative educational experience" that equips students with both technical fundamentals and professional perspective.

## Leadership
**Department Chair:** Geethapriya Thamilarasu, Associate Professor
- **Contact:** csschair@uw.edu

## Faculty Expertise
CSS faculty specialize across nine research areas including Artificial Intelligence/Machine Learning, Cybersecurity, Data Science, Software Engineering, Human-Computer Interaction, Computational Biology, Graphics & Gaming, Parallel/Distributed Computing, and Computer Science Education.

## Undergraduate Programs
- Bachelor of Arts in Applied Computing
- Bachelor of Science in Computer Science & Software Engineering (with Information Assurance/Cybersecurity option)
- Bachelor of Science in Computer Engineering

## Graduate Programs
- Master of Science in Computer Science & Software Engineering
- Master of Science in Cybersecurity Engineering
- Graduate Certificate in Software Design & Development

## Facilities
CSS operates four specialized labs: Advanced Projects Lab, Open Lab, Embedded Systems Lab, and Cybersecurity Lab, serving as collaborative hubs for research and student engagement.

## Strategic Focus
The department prioritizes preparing students for "rewarding careers" while building "effective, confident, and respected" computing professionals.
```

</details>


Now let me read the curriculum files in chunks and fetch the ACM curricula page.

**Tool: Read**
Reading `/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-csse.html`

<details><summary>Tool Result</summary>

**Error:**
```
File content (62941 tokens) exceeds maximum allowed tokens (25000). Use offset and limit parameters to read specific portions of the file, or search for specific content instead of reading the whole file.
```

</details>


**Tool: Read**
Reading `/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-ac.html`

<details><summary>Tool Result</summary>

**Error:**
```
File content (62983 tokens) exceeds maximum allowed tokens (25000). Use offset and limit parameters to read specific portions of the file, or search for specific content instead of reading the whole file.
```

</details>


**Tool: WebFetch**
`https://www.acm.org/education/curricula-recommendations`

<details><summary>Tool Result</summary>

```
The server returned HTTP 403 Forbidden.

The response body was not retrieved. If this URL requires authentication, use an authenticated tool (e.g. `gh` for GitHub, or an MCP-provided fetch tool) instead of WebFetch.
```

</details>


**Tool: Bash**
*Extract text from CSSE and AC curriculum HTML files*
```bash
cd /Users/pisan/bitbucket/pisanuw/curriculum-css/sources && python3 -c "
from html.parser import HTMLParser
import re

class TextExtractor(HTMLParser):
    def __init__(self):
        super().__init__()
        self.text = []
        self.skip = False
    def handle_starttag(self, tag, attrs):
        if tag in ('script','style'):
            self.skip = True
    def handle_endtag(self, tag):
        if tag in ('script','style'):
            self.skip = False
    def handle_data(self, data):
        if not self.skip:
            s = data.strip()
            if s:
                self.text.append(s)

for fname in ['curriculum-csse.html','curriculum-ac.html']:
    p = TextExtractor()
    p.feed(open(fname).read())
    text = '\n'.join(p.text)
    print(f'=== {fname} ===')
    print(text[:8000])
    print()
"

```

<details><summary>Tool Result</summary>

```
=== curriculum-csse.html ===
CSSE Curriculum - School of Science, Technology, Engineering & Mathematics
Skip To Content
Current site
All UW Bothell
Search keywords
Search
Open mobile menu
Quick Links
School of Science, Technology, Engineering & Mathematics
Close mobile menu
School of Science, Technology, Engineering & Mathematics
Search keywords
Current site
All UW Bothell
About
Expand Navigation
STEM Advisory Board
Departments
Expand Navigation
Biological Sciences
Computing & Software Systems
Engineering & Mathematics
Physical Sciences
Awards & Endowments

... (786 lines omitted) ...

Curriculum
Research
Expand Navigation
Computer Engineering
Power & Energy
Signal Processing
Biomedical Systems and Devices
Microelectronics and Devices
Wireless, RF/Microwave, and Telecommunications
Advising
Careers
Graduate Certificate in Software Design & Development
Expand Navigation
Admissions
Prerequisites guide
Tuition
Curriculum
Careers
Frequently Asked Questions
Graduate Certificate in Electrical & Computer Engineering Foundations
Expand Navigation
Admissions
Prerequisites guide
Tuition
C
```

</details>


The nav repeats heavily - let me extract the actual curriculum content.

**Tool: Bash**
*Extract curriculum requirement sections from HTML files*
```bash
python3 -c "
from html.parser import HTMLParser
import re

class TextExtractor(HTMLParser):
    def __init__(self):
        super().__init__()
        self.text = []
        self.skip = False
        self.in_main = False
    def handle_starttag(self, tag, attrs):
        if tag in ('script','style'):
            self.skip = True
        attrs_d = dict(attrs)
        if tag == 'main' or (tag == 'div' and attrs_d.get('id') in ('content','main-content','page-content')):
            self.in_main = True
    def handle_endtag(self, tag):
        if tag in ('script','style'):
            self.skip = False
    def handle_data(self, data):
        if not self.skip:
            s = data.strip()
            if s:
                self.text.append(s)

for fname in ['curriculum-csse.html','curriculum-ac.html']:
    content = open(fname).read()
    # Find main content area - look for table with course requirements
    # Extract everything after the breadcrumb/nav
    idx = content.find('required')
    if idx < 0:
        idx = content.find('Required')
    snippet = content[max(0,idx-200):idx+15000]
    p = TextExtractor()
    p.feed(snippet)
    text = '\n'.join(p.text)
    print(f'=== {fname} ===')
    print(text[:6000])
    print()
" 2>&1 | head -300

```

<details><summary>Tool Result</summary>

```
=== curriculum-csse.html ===
requirements
CSS Electives (25 credits / usually 5 courses)
All CSS electives must be 200-level or higher, and they may not be courses that are already required for your degree. Of the 25 credits:
At least 15 credits must be 400-level
Up to 10 credits may be 200-level
Up to 10 credits combined of CSS 397 (Internship), 498 (Independent Study), or 499 (Undergraduate Research)
Up to 10 credits combined of CSS 290, 390, or 490 (Special Topics)
300-400 Level Electives (15 credits / usually 3 courses)
May be additional CSS electives or electives from other subject areas
These courses may overlap with your General Education requirements (A&H, SSc, DIV, etc.), above, as long as they are 300-level or higher.
Information Assurance and Cybersecurity (IAC) option
Information Assurance and Cybersecurity (IAC) is a Computer Science & Software Engineering pathway that covers the creation and management of safe and secure systems. All organizations—large or small, public or private—rely on secure systems for individual and organizational privacy and security. The IAC option prepares students to create, deploy, and manage systems that ensure the security of any organization.
This tri-campus pathway allows students to select from an approved list of courses offered from all three UW campuses: Bothell, Seattle, and Tacoma. The electives at each campus emphasize the strengths found in the programs offered there, and course topics include information assurance policy, secure coding, and networking and systems security.
Declaring the IAC option
After admission into the general CSSE major, you can contact the advising office at
cssadv@uw.edu
to switch into the IAC option. Please include your name and student ID number.
Requirements
IAC-option students take the same core courses as those of the general CSSE major, but replace the 25 credits of “CSS Electives” with the courses below:
CSS 310: Information Assurance and Cybersecurity
Minimum 15 credits (3 courses) of elective coursework from the lists below. Only one networking class (CSS 432, INFO 314, or T INFO 250; marked with an
asterisk *
) may be taken.
Minimum of 5 additional credits (usually 1 course) of 200-level or higher CSS Elective coursework in any topic.

... (67 lines omitted) ...

Technical Level
General Business, Social & Technical
Business Case Justification: Justifies project expenditures, equipment and other resources in terms of business costs, benefits and risks.
Technology Evaluation and Selection: Evaluates and selects software and hardware appropriate to the application, architecture and resource constraints; maintains awareness and understanding of emerging technology.
Process Reengineering: Performs business requirement analysis, using appropriate tools and methodologies to maximize organizational performance.
Mathematical Principles and Techniques: Understands theory and application of numerical, statistical, set theory, and other mathematical techniques in the context of applications and systems programming.
General Software Systems: Has general understanding of the principles and applications of software development and design; understands the relationship between software development and other functions in the business organization.
Social Implications of Science & Technology: Understands the interaction between science and technology and the broader social, political, and organizational environment; critically assesses ethical implications of computing technology.
Technical Writing: Designs and writes effective guidelines, standards, procedures, processes, applications, using appropriate methods, tools and delivery options.
Application Programming
Requirements Definition and Analysis: Elicits and clearly defines user\’s needs, assessing potential solutions against benefits and risks; uses appropriate tools for analyzing requirements and creating appropriate data and work flow models.
Software Development Life Cycle: Understands and effectively manages the process of developing designing, testing, and delivering a software application.
Functional Design: Identifies system platform, components, inputs, interface requirements, and dependencies which ensure that the system will achieve its objectives.
Testing: Plans, executes, and validates results of unit, systems, and acceptance testing to ensure conformity to user\’s requirements.
Implementation: Plans and executes smooth integration of an application into the computing environment.
Programming: Comprehends and applies principles of programming; effectively translates design specifications into appropriate software components.
Collaborative Programming Techniques: Uses methods and tools that support cooperative software development among users in different locations.
Quality Assurance: Employs appropriate quality assurance standards and procedures to ensure delivery of bug-free applications that meet user\’s needs.
Infrastructure/Operations
Technology Integration: Integrates various technologies, systems, applications, database and components across multiple platforms.
Hardware Architecture: Understands hardware components, architecture, and interrelationship among hardware, software, and operating systems.
Performance Measurements & Tuning: Uses appropriate performance metrics to monitor, optimize and troubleshoot system performance.
Operating Systems: Understands operating systems fundamentals including: file systems, process, and memory management.
System Administration: Understands appropriate procedures and techniques for management and administrating a network, data center, or other computer system; manages changes to the computing environment.
Technical Training and Support: Provides user support through analysis and problem solving to facilitate installation, implementation, maintenance, education, and documentation of computer ha
```

</details>


Now let me get the core required courses for both programs.

**Tool: Bash**
*Extract CSS course numbers from CSSE curriculum*
```bash
python3 -c "
content = open('/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-csse.html').read()
# Find the section listing required courses
idx = content.find('Core')
# Look for the table/list of CSS required courses
# Search for CSS ### patterns
import re
courses = re.findall(r'CSS\s*\d{3}[^<\"]*', content)
seen = set()
print('=== CSSE Required Courses mentioned ===')
for c in courses:
    c = c.strip()
    if c not in seen and len(c) < 100:
        seen.add(c)
        print(c)
" 2>&1 | head -100

```

<details><summary>Tool Result</summary>

```
=== CSSE Required Courses mentioned ===
CSS 301: Technical Writing for Computing Professionals
CSS 342: Data Structures and Algorithms I
CSS 343: Data Structures and Algorithms II
CSS 350: Management Principles for Computing Professionals
CSS 360: Software Engineering
CSS 370: Analysis and Design
CSS 422: Hardware and Computer Organization
CSS 430: Operating Systems
CSS 497: Capstone
CSS 397 (Internship), 498 (Independent Study), or 499 (Undergraduate Research)
CSS 290, 390, or 490 (Special Topics)
CSS 310: Information Assurance and Cybersecurity
CSS 432, INFO 314, or T INFO 250; marked with an
CSS 337 Secure Systems
CSS 411 Computer Technology and Public Policy
CSS 415 Emerging Topics in Information Assurance and Cybersecurity
CSS 432 Computer Networking
```

</details>


**Tool: Bash**
*Find core required courses section in CSSE curriculum*
```bash
python3 -c "
content = open('/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-csse.html').read()
# Find the required core courses section
idx = content.find('Required Courses')
if idx < 0:
    idx = content.find('Core Courses')
print(content[idx:idx+5000])
" 2>&1 | head -200

```

<details><summary>Tool Result</summary>

```
Core Courses</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/cybersecurity/curriculum/elective-courses">Elective Courses</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/cybersecurity/curriculum/culminating-experience">Culminating Experience</a></li>
		</ul>
</li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/cybersecurity/advising">Advising</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/cybersecurity/careers">Careers</a></li>
	</ul>
</li>
<li class="menu-item menu-item-has-children"><a href="https://www.uwb.edu/stem/graduate/mscsse">Master of Science in Computer Science &amp; Software Engineering</a><button class="js-main-menu-child-toggle child-nav-toggle-btn" aria-haspopup="true">
<span class="show-for-sr" data-label='["Collapse Navigation","Expand Navigation"]'>Expand Navigation</span>
<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" viewBox="0 0 11.85 7.93" width="18" height="18" fill="currentColor" style="color:#4b2e83">
  <path d="M11.851,1.517 L5.887,7.93 0,1.452 1.6,0 5.887,4.76 10.235,0.077 11.851,1.517 Z" fill="currentColor"/>
</svg></button>

<ul class="mobile-sub-menu">
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/mscsse/admissions">Admissions</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/mscsse/admissions/apply">How to Apply</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/mscsse/tuition">Tuition</a></li>
<li class="menu-item menu-item-has-children"><a href="https://www.uwb.edu/stem/graduate/mscsse/curriculum">Curriculum</a><button class="js-main-menu-child-toggle child-nav-toggle-btn" aria-haspopup="true">
<span class="show-for-sr" data-label='["Collapse Navigation","Expand Navigation"]'>Expand Navigation</span>
<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" viewBox="0 0 11.85 7.93" width="18" height="18" fill="currentColor" style="color:#4b2e83">
  <path d="M11.851,1.517 L5.887,7.93 0,1.452 1.6,0 5.887,4.76 10.235,0.077 11.851,1.517 Z" fill="currentColor"/>
</svg></button>


... (6 lines omitted) ...

<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/mscsse/advising">Advising</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/mscsse/careers">Careers</a></li>
	</ul>
</li>
<li class="menu-item menu-item-has-children"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering">Master of Science in Electrical &amp; Computer Engineering</a><button class="js-main-menu-child-toggle child-nav-toggle-btn" aria-haspopup="true">
<span class="show-for-sr" data-label='["Collapse Navigation","Expand Navigation"]'>Expand Navigation</span>
<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" viewBox="0 0 11.85 7.93" width="18" height="18" fill="currentColor" style="color:#4b2e83">
  <path d="M11.851,1.517 L5.887,7.93 0,1.452 1.6,0 5.887,4.76 10.235,0.077 11.851,1.517 Z" fill="currentColor"/>
</svg></button>

<ul class="mobile-sub-menu">
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering/admissions">Admissions</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering/admissions/apply">How to Apply</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering/tuition">Tuition</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering/curriculum">Curriculum</a></li>
<li class="menu-item menu-item-has-children"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering/research">Research</a><button class="js-main-menu-child-toggle child-nav-toggle-btn" aria-haspopup="true">
<span class="show-for-sr" data-label='["Collapse Navigation","Expand Navigation"]'>Expand Navigation</span>
<svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" viewBox="0 0 11.85 7.93" width="18" height="18" fill="currentColor" style="color:#4b2e83">
  <path d="M11.851,1.517 L5.887,7.93 0,1.452 1.6,0 5.887,4.76 10.235,0.077 11.851,1.517 Z" fill="currentColor"/>
</svg></button>

<ul class="mobile-sub-menu">
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering/research/computer-engineering">Computer Engineering</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-computer-engineering/research/power-energy">Power &#038; Energy</a></li>
<li class="menu-item"><a href="https://www.uwb.edu/stem/graduate/ms-electrical-co
```

</details>


**Tool: Bash**
*Extract CSS course numbers from AC curriculum*
```bash
python3 -c "
content = open('/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-ac.html').read()
import re
courses = re.findall(r'CSS\s*\d{3}[^<\"]*', content)
seen = set()
print('=== AC Required/Mentioned Courses ===')
for c in courses:
    c = c.strip()
    if c not in seen and len(c) < 120:
        seen.add(c)
        print(c)
" 2>&1

```

<details><summary>Tool Result</summary>

```
=== AC Required/Mentioned Courses ===
CSS 496 capstone course
CSS 301: Technical Writing
CSS 340: Applied Algorithmics; or
CSS 342: Advanced Data Structures, Algorithms, and Discrete Mathematics I; or
CSS 350: Management for Computing Professionals; or
CSS 360: Software Engineering
CSS 421: Hardware and Operating Systems
CSS 496: Applied Computing Capstone
CSS 495: Applied Computing Internship
CSS 397/495/498/499 (Variable Credit Courses)
CSS 290/390/490 (Special Topics Courses)
```

</details>


**Tool: Bash**
*Extract CSSE core course list with credits*
```bash
python3 -c "
content = open('/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/curriculum-csse.html').read()
# Find the actual required course list in the CSSE page
# Look for a section that lists the courses with credit counts
import re
# Find where the main curriculum table starts
idx = content.find('143')
section = content[max(0,idx-500):idx+8000]
# Remove HTML tags
clean = re.sub(r'<[^>]+>', ' ', section)
clean = re.sub(r'\s+', ' ', clean)
print(clean[:5000])
" 2>&1

```

<details><summary>Tool Result</summary>

```
53h-4.21l1.225 1.253v13.205l-1.225 1.253Zm-3.888 0v-2.872l-1.693 1.693h-4.769v-6.6h3.544l1.253 1.253V9.227l-1.253 1.247h-3.544V4.881h4.769l1.693 1.693V3.752h-9.4l1.225 1.253v13.206l-1.225 1.253Zm-22.822-7.9h6.608v6.631l-1.253 1.253h4.238l-1.247-1.253V4.966l1.247-1.253h-4.2l1.253 1.253v5.4h-6.608v-5.4l1.253-1.253h-4.2l1.225 1.253v13.205l-1.225 1.253h4.2l-1.253-1.253v-6.608Zm-10.384 6.631V4.881h2.985l1.693 1.693V3.752h-11.05v2.822l1.693-1.693h2.951v13.29l-1.225 1.253h4.21l-1.253-1.253Zm-15.1.4c-3.143 0-4.233-3.753-4.233-7s1.089-7 4.233-7 4.261 3.753 4.261 7-1.089 7-4.261 7m-6.281-6.992c0 4 2.257 8.2 6.281 8.2s6.315-4.2 6.315-8.2-2.257-8.2-6.315-8.2-6.281 4.2-6.281 8.2m-8.222 6.687h-2.472v-6.123h2.472a3.245 3.245 0 0 1 3.251 3.251 3.105 3.105 0 0 1-3.251 2.906m-2.472-13.375h1.913a3.143 3.143 0 0 1 3.014 3.149 2.97 2.97 0 0 1-3.014 2.9h-1.913V4.881Zm-2.948 14.515h5.429c2.506 0 5.079-1.01 5.079-4.075a4.3 4.3 0 0 0-3.516-4.046 3.96 3.96 0 0 0 2.743-3.273c0-3.2-2.37-4.317-4.876-4.317h-4.859l1.225 1.253v13.205Z"/> Open mobile menu Quick Links School of Science, Technology, Engineering &amp; Mathematics Close mobile menu School of Science, Technology, Engineering &amp; Mathematics Search keywords Current site All UW Bothell About Expand Navigation STEM Advisory Board Departments Expand Navigation <path d="M11.851,1.517 L5.887,7.93 0,1.452 1.6,0 5.887,4.76 10.235,
```

</details>


I now have enough to create the initial documents. Let me write them all now.

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md`
```md
# Briefing

- **Purpose:** Develop a multi-year curriculum change proposal for the UWB CSS Department to equip graduates with skills needed in an AI-transformed job market.
- **Audience:** CSS Faculty
- **Current scope:** Three phased deliverables - (1) information gaps and what to collect, (2) assumptions/decisions inventory, (3) draft proposal covering 26-27, 27-28, and 28-29+ with concrete course-level guidance.
- **Key decisions:** Which courses to modify vs. phase out vs. create; how fast to move given UW approval timelines; how to handle faculty upskilling; whether to require AI content in core vs. electives; how to differentiate the AC and CSSE tracks.
- **Non-goals:** Operational implementation details (scheduling, room assignments, faculty assignments); changes to graduate programs (separate effort); changes to admissions criteria.

## Source material on hand
- Full CSS course catalog (CSS 101 - CSS 700)
- CSSE curriculum requirements (BS in Computer Science & Software Engineering)
- AC curriculum requirements (BA in Applied Computing)
- Syllabuses from Autumn 2021, Winter 2022, Spring 2022, Summer 2022
- UWB CSS Department overview (faculty areas, labs, programs)
- UWB Mission & Vision

... (9 lines omitted) ...

CSS 301 + CSS 340 or 342 + CSS 350 + CSS 360 + CSS 421 → CSS 496 (capstone)
Plus concentration courses + general electives

### Existing AI-related courses (all elective, not required)
- CSS 382: Introduction to AI (undergrad)
- CSS 444: Analyzing Biases in the Age of Digital Data (undergrad)
- CSS 485: Artificial Neural Networks (undergrad)
- CSS 486: Machine Intelligence (undergrad)
- CSS 487: Computer Vision (undergrad)
- CSS 488: Natural Language Processing (undergrad, new)
- CSS 576: Cybersecurity and AI (grad)
- CSS 581: Machine Learning (grad)
- CSS 582: Interpretable ML (grad)
- CSS 586: Deep Learning and AI (grad)

```

<details><summary>Tool Result</summary>

```
The file /Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md has been updated successfully. (file state is current in your context — no need to Read it back)
```

</details>


**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/Assumptions.md`
```md
# Assumptions and Key Decisions

Working document for the CSS Curriculum AI Transition Plan.
Each item is either an **assumption** (something we are treating as true without full verification) or a **decision** (a choice that faculty must make explicitly). Open items that require data or discussion are marked **[OPEN]**.

---

## 1. Context and Scope

**A1 (assumption):** The decline in CS internship and entry-level hiring is structural, not cyclical. AI is permanently changing the composition of software engineering teams, reducing demand for undifferentiated junior developers while increasing demand for engineers who can work effectively alongside AI tools.

**A2 (assumption):** Graduates who can use AI as a force-multiplier (prompting, evaluation, integration, safety) will be more competitive than those who cannot, even for traditional roles. This is analogous to how earlier generations had to learn version control or cloud tooling.

**A3 (assumption):** Foundational CS skills - algorithms, systems, software engineering process, mathematics - remain essential. AI tools are not a substitute for understanding what the code does.


... (105 lines omitted) ...

Format: 10 questions, confidential, via email
Estimated time: 10 minutes

---

## 8. Open Decisions Summary

| ID | Decision | Options | Recommendation |
|---|---|---|---|
| A4 | AI as core vs. specialization | Core requirement / Elective track | Hybrid: AI literacy as core, deep AI as track |
| A13 | Catalog year impact | New admits only / Phased / All students | New admits for structural changes; encourage current students |
| A20 | Integration approach | Modify existing / New courses / Both | Both, phased: modify first, add new in yr 2 |
| A21 | CSS 382 required for CSSE? | Yes / No / New course instead | Defer to data; lean toward new course or modified 382 |
| A22 | New AI-for-SE course? | Create new / Absorb into existing | Create new 400-level; absorb basics into CSS 360 |

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/Assumptions.md (file state is current in your context — no need to Read it back)
```

</details>


Now creating the draft proposal:

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/CurriculumProposal-Draft1.md`
```md
# CSS Curriculum Transition Plan: Preparing Graduates for an AI-Transformed Industry

**Version:** Draft 1 (for faculty discussion)
**Date:** June 2026
**Audience:** CSS Faculty
**Status:** Working draft - requires data collection and faculty input before finalizing

---

## Executive Summary

The computing job market has undergone a structural shift. AI tools now automate a significant portion of the work previously done by junior software engineers - boilerplate code generation, basic debugging, documentation, simple testing - reducing demand for undifferentiated entry-level hires while simultaneously raising the baseline competency expected of those who are hired. CSS graduates who cannot work effectively alongside AI tools are at a disadvantage; those who understand AI deeply enough to build, evaluate, and responsibly deploy it are in high demand.

This proposal outlines a three-phase curriculum transition covering 2026-27 through 2028-29. The goal is not to replace foundational CS education - algorithms, systems, software engineering, mathematics remain essential - but to integrate AI throughout the curriculum and ensure every graduate has practical AI fluency alongside their technical depth.


... (285 lines omitted) ...


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

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/CurriculumProposal-Draft1.md (file state is current in your context — no need to Read it back)
```

</details>


Now update CHANGES.md:

**Tool: Edit**
Editing `/Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md`
```diff
- 2026-06-06 [note] Initialized.
+ 2026-06-06 [note] Initialized.
+ 2026-06-06 [plan] Created Assumptions.md (28 assumptions/decisions, 3 surveys, info-gap table) and CurriculumProposal-Draft1.md (3-phase plan 26-27 through 28-29+). Updated BRIEFING.md with project scope and curriculum snapshot.
```

<details><summary>Tool Result</summary>

```
The file /Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md has been updated successfully. (file state is current in your context — no need to Read it back)
```

</details>


Here is where things stand and what I found.

---

## What was created

**[Assumptions.md](Assumptions.md)** - 28 numbered items covering:
- Context assumptions (AI disruption is structural, foundations still matter)
- 9 "OPEN" items that require explicit faculty decisions or data before the proposal can be finalized
- Three recommended surveys with audience, questions, and time estimates
- A table of all information still needed, with suggested owners and timelines

**[CurriculumProposal-Draft1.md](CurriculumProposal-Draft1.md)** - Full three-phase draft:
- Phase 1 (2026-27): No new course numbers, no approval needed - targeted content additions to CSS 360, 211, 343, 350, 301, 370; capstone rubric update; faculty bootcamp; CSS 390/490 special topics pilot
- Phase 2 (2027-28): New CSS 4xx course ("AI Systems for Software Engineers"), CSS 382 modernization, AI-area elective requirement added to both CSSE and AC, review of 3 candidates for phase-out (CSS 482, 484, 483)
- Phase 3 (2028-29+): Introductory course updates, goal-state degree map, 2-3 additional new courses

---

## Key questions I'd raise for faculty before the next draft

1. **Is CSS 382 the vehicle, or do we need a new course?** CSS 382 (Intro AI) is theoretical. The gap is practical: LLM integration, responsible deployment, evaluating AI output. A separate 400-level "AI Systems for Software Engineers" would serve a different student than CSS 382.

2. **Does the required core have room?** Making any AI course required in CSSE means something else must shrink or leave. Faculty need to decide what they are willing to trade.

3. **Do we have the data we need?** Three surveys (faculty skills, student readiness, employer needs) are prerequisites to a concrete final proposal. Would it be useful to draft those survey instruments next?

4. **What's the ABET situation?** Any change to required courses in CSSE has ABET implications. That timeline needs to be known before Phase 2 planning can be locked.

</details>

## User

1. 382 can be modified but a new course is needed
2. No, there is no room. The proposal must have several options on what might need to be excluded.
3. Draft the surveys now, can update as needed
4. Can note and ignore ABET accreditation for the time being

Not every course is offered each quarter. Some courses might be on the books but have not been offered for many years. A new directory sources/uwb/ has information on courses that are offered each quarter, including how many sections, so that can provide additional information

<details>
<summary>Assistant (18 steps)</summary>

Let me first explore the new sources/uwb/ directory to understand what's there.

**Tool: Bash**
*List files in sources/uwb directory*
```bash
find /Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb -type f | sort | head -60
```

<details><summary>Tool Result</summary>

```
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/.DS_Store
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/catalog_index.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/course_index.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20ACCT%20501.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20ACCT%20504.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20ACCT%20568.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BECN%20300.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BECN%20302.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BECN%20303.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BECN%20382.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BECN%20458.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BECN%20460.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BECN%20469.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20180.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20200.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20220.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20231.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20233.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20285.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20293.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20310.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20320.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20330.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20335.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20340.json

... (10 lines omitted) ...

/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20380.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20383.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20385.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20390.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20393.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20394.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20460.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20466.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20470.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20471.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20480.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20485.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20495.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20498.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BIO%20499.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20110.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20120.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20201.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20210.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20211.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20215.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20220.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20221.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20230.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20BUS%20300.json
```

</details>


**Tool: Bash**
*List all CSS course JSON files*
```bash
find /Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses -name "CSS*" | sort
```

<details><summary>Tool Result</summary>

```
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20101.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20107.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20110.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20112.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20123.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20132.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20133.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20142.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20143.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20173.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20198.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20199.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20211.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20225.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20290.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20295.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20301.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20310.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20315.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20320.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20337.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20340.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20342.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20343.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20350.json

... (42 lines omitted) ...

/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20499.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20506.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20507.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20517.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20518.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20527.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20533.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20535.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20537.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20539.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20545.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20552.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20553.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20566.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20578.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20579.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20581.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20586.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSS%20590.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSSSKL%20123.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSSSKL%20132.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSSSKL%20133.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSSSKL%20142.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSSSKL%20143.json
/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/CSSSKL%20342.json
```

</details>


**Tool: Bash**
*Inspect JSON file structure*
```bash
cat /Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20ACCT%20501.json | head -5
# Check the structure of one file
python3 -c "import json; d=json.load(open('/Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses/B%20ACCT%20501.json')); print(json.dumps(d, indent=2))" 2>&1 | head -40
```

<details><summary>Tool Result</summary>

```
{"generatedAt": "2026-05-15T13:37:20Z", "uni": "uwb", "id": "B%20ACCT%20501", "course": "B ACCT 501", "recordCount": 2, "records": [{"uni": "uwb", "dept": "bacct", "deptName": "Master of Science in Accounting", "term": "WIN2025", "course": "B ACCT 501", "courseTitle": "ACCOUNTING THEORY", "section": "B", "instructor": "TBA"}, {"uni": "uwb", "dept": "bacct", "deptName": "Master of Science in Accounting", "term": "WIN2023", "course": "B ACCT 501", "courseTitle": "ACCOUNTING THEORY", "section": "B", "instructor": "TBA"}]}{
  "generatedAt": "2026-05-15T13:37:20Z",
  "uni": "uwb",
  "id": "B%20ACCT%20501",
  "course": "B ACCT 501",
  "recordCount": 2,
  "records": [
    {
      "uni": "uwb",
      "dept": "bacct",
      "deptName": "Master of Science in Accounting",
      "term": "WIN2025",
      "course": "B ACCT 501",
      "courseTitle": "ACCOUNTING THEORY",
      "section": "B",
      "instructor": "TBA"
    },
    {
      "uni": "uwb",
      "dept": "bacct",
      "deptName": "Master of Science in Accounting",
      "term": "WIN2023",
      "course": "B ACCT 501",
      "courseTitle": "ACCOUNTING THEORY",
      "section": "B",
      "instructor": "TBA"
    }
  ]
}
```

</details>


Good - each JSON record is an actual section offering with term and instructor. Let me now analyze all CSS courses for their offering frequency.

**Tool: Bash**
*Analyze CSS course offering frequency from JSON files*
```bash
cd /Users/pisan/bitbucket/pisanuw/curriculum-css/sources/uwb/courses && python3 -c "
import json, glob, os
from collections import defaultdict

results = []
for f in sorted(glob.glob('CSS*.json')):
    d = json.load(open(f))
    course = d['course']
    records = d.get('records', [])
    terms = sorted(set(r['term'] for r in records))
    sections_per_term = defaultdict(list)
    for r in records:
        sections_per_term[r['term']].append(r.get('section','?'))
    
    results.append({
        'course': course,
        'total_sections': len(records),
        'total_terms': len(terms),
        'terms': terms,
        'sections_per_term': dict(sections_per_term)
    })

# Sort by total sections desc
results.sort(key=lambda x: -x['total_sections'])

print(f'{'Course':<15} {'Terms Offered':<14} {'Total Sections':<16} {'Latest Term':<12} {'Terms'}')
print('-' * 120)
for r in results:
    latest = r['terms'][-1] if r['terms'] else 'NEVER'
    # Summarize sections per term
    spt = {t: len(s) for t, s in r['sections_per_term'].items()}
    print(f'{r[\"course\"]:<15} {r[\"total_terms\"]:<14} {r[\"total_sections\"]:<16} {latest:<12} {\" \".join(r[\"terms\"])}')
" 2>&1

```

<details><summary>Tool Result</summary>

```
Course          Terms Offered  Total Sections   Latest Term  Terms
------------------------------------------------------------------------------------------------------------------------
CSS 497         23             123              WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 301         23             92               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 342         22             74               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 360         23             72               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 142         23             70               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSSSKL 142      23             70               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 143         23             56               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSSSKL 143      23             56               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 343         23             54               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 198         23             52               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 199         23             46               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 498         23             46               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 499         23             46               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 422         23             45               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 370         18             42               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 350         18             41               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 430         22             40               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 475         23             35               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 310         23             33               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 107         18             31               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 490         19             30               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 397         23             23               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2021 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026
CSS 495         22             23               WIN2026      AUT2020 AUT2021 AUT2022 AUT2023 AUT2024 AUT2025 SPR2021 SPR2022 SPR2023 SPR2024 SPR2025 SPR2026 SUM2022 SUM2023 SUM2024 SUM2025 WIN2021 WIN2022 WIN2023 WIN2024 WIN2025 WIN2026

... (44 lines omitted) ...

CSS 590         4              5                SUM2024      AUT2024 SPR2022 SPR2026 SUM2024
CSS 225         4              4                SPR2026      SPR2022 SPR2024 SPR2025 SPR2026
CSS 444         4              4                WIN2026      WIN2022 WIN2023 WIN2024 WIN2026
CSS 452         4              4                WIN2024      WIN2021 WIN2022 WIN2023 WIN2024
CSS 484         4              4                WIN2023      AUT2023 AUT2024 WIN2022 WIN2023
CSS 123         3              3                SPR2025      SPR2023 SPR2024 SPR2025
CSS 518         3              3                WIN2026      WIN2024 WIN2025 WIN2026
CSS 578         3              3                SPR2025      SPR2022 SPR2024 SPR2025
CSS 581         3              3                WIN2026      WIN2023 WIN2025 WIN2026
CSS 315         2              2                WIN2026      WIN2025 WIN2026
CSS 535         2              2                WIN2026      WIN2025 WIN2026
CSS 553         2              2                SPR2025      SPR2024 SPR2025
CSS 488         1              1                SPR2025      SPR2025
CSS 506         1              1                AUT2024      AUT2024
CSS 507         1              1                WIN2024      WIN2024
CSS 517         1              1                AUT2025      AUT2025
CSS 527         1              1                AUT2025      AUT2025
CSS 533         1              1                SPR2026      SPR2026
CSS 537         1              1                WIN2024      WIN2024
CSS 539         1              1                SPR2026      SPR2026
CSS 545         1              1                SPR2024      SPR2024
CSS 552         1              1                WIN2026      WIN2026
CSS 566         1              1                SPR2024      SPR2024
CSS 579         1              1                AUT2024      AUT2024
CSS 586         1              1                SPR2023      SPR2023
```

</details>


Excellent data. Now let me check which catalog courses have no JSON file at all (truly dormant) and look at a few key files in detail.

**Tool: Bash**
*Find dormant courses and compute annual section counts*
```bash
python3 -c "
import json, glob, os

# Courses in JSON
json_courses = set()
for f in glob.glob('CSS*.json'):
    d = json.load(open(f))
    json_courses.add(d['course'])

# All CSS courses from catalog (extracted earlier)
catalog_courses = [
    'CSS 101','CSS 107','CSS 110','CSS 112','CSS 123','CSS 130','CSS 132','CSS 133',
    'CSS 142','CSS 143','CSS 173','CSS 198','CSS 199','CSS 205','CSS 211','CSS 225',
    'CSS 250','CSS 290','CSS 295','CSS 301','CSS 305','CSS 310','CSS 315','CSS 320',
    'CSS 330','CSS 337','CSS 340','CSS 342','CSS 343','CSS 350','CSS 360','CSS 370',
    'CSS 371','CSS 382','CSS 383','CSS 385','CSS 390','CSS 397','CSS 405','CSS 411',
    'CSS 415','CSS 416','CSS 421','CSS 422','CSS 427','CSS 430','CSS 431','CSS 432',
    'CSS 434','CSS 436','CSS 444','CSS 448','CSS 449','CSS 450','CSS 451','CSS 452',
    'CSS 455','CSS 457','CSS 458','CSS 461','CSS 473','CSS 474','CSS 475','CSS 477',
    'CSS 478','CSS 480','CSS 481','CSS 482','CSS 483','CSS 484','CSS 485','CSS 486',
    'CSS 487','CSS 488','CSS 490','CSS 495','CSS 496','CSS 497','CSS 498','CSS 499',
]

print('=== Undergrad courses in catalog but NEVER in schedule data (dormant) ===')
for c in catalog_courses:
    if c not in json_courses:
        print(f'  {c}')

print()
print('=== Undergrad courses: sections per year (AUT+WIN+SPR+SUM) ===')
# Load all and compute annual sections
from collections import defaultdict
for f in sorted(glob.glob('CSS*.json')):
    d = json.load(open(f))
    if not d['course'].startswith('CSS '):
        continue
    num = int(d['course'].split()[1])
    if num >= 500:
        continue  # skip grad
    records = d.get('records', [])
    by_year = defaultdict(int)
    for r in records:
        term = r['term']
        year = term[-4:]
        by_year[year] += 1
    years = sorted(by_year.keys())
    total = len(records)
    latest = sorted(set(r['term'] for r in records))[-1] if records else 'N/A'
    print(f\"  {d['course']:<10} total={total:<4} latest={latest}  by_year={dict(sorted(by_year.items()))}\")
" 2>&1

```

<details><summary>Tool Result</summary>

```
=== Undergrad courses in catalog but NEVER in schedule data (dormant) ===
  CSS 130
  CSS 205
  CSS 250
  CSS 305
  CSS 330
  CSS 405
  CSS 416
  CSS 450
  CSS 455
  CSS 457
  CSS 477
  CSS 482

=== Undergrad courses: sections per year (AUT+WIN+SPR+SUM) ===
  CSS 101    total=18   latest=WIN2026  by_year={'2020': 1, '2021': 3, '2022': 3, '2023': 3, '2024': 3, '2025': 3, '2026': 2}
  CSS 107    total=31   latest=WIN2026  by_year={'2020': 2, '2021': 6, '2022': 4, '2023': 5, '2024': 6, '2025': 5, '2026': 3}
  CSS 110    total=6    latest=WIN2026  by_year={'2021': 1, '2022': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 112    total=18   latest=WIN2026  by_year={'2020': 1, '2021': 3, '2022': 3, '2023': 3, '2024': 3, '2025': 3, '2026': 2}
  CSS 123    total=3    latest=SPR2025  by_year={'2023': 1, '2024': 1, '2025': 1}
  CSS 132    total=6    latest=AUT2025  by_year={'2020': 1, '2021': 1, '2022': 1, '2023': 1, '2024': 1, '2025': 1}
  CSS 133    total=6    latest=WIN2026  by_year={'2021': 1, '2022': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 142    total=70   latest=WIN2026  by_year={'2020': 4, '2021': 12, '2022': 12, '2023': 12, '2024': 12, '2025': 12, '2026': 6}
  CSS 143    total=56   latest=WIN2026  by_year={'2020': 2, '2021': 9, '2022': 9, '2023': 9, '2024': 10, '2025': 10, '2026': 7}
  CSS 173    total=5    latest=WIN2026  by_year={'2020': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}

... (33 lines omitted) ...

  CSS 444    total=4    latest=WIN2026  by_year={'2022': 1, '2023': 1, '2024': 1, '2026': 1}
  CSS 448    total=5    latest=WIN2022  by_year={'2021': 1, '2022': 2, '2023': 1, '2024': 1}
  CSS 449    total=5    latest=SPR2026  by_year={'2022': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 451    total=6    latest=AUT2025  by_year={'2020': 1, '2021': 1, '2022': 1, '2023': 1, '2024': 1, '2025': 1}
  CSS 452    total=4    latest=WIN2024  by_year={'2021': 1, '2022': 1, '2023': 1, '2024': 1}
  CSS 458    total=5    latest=SPR2025  by_year={'2021': 1, '2023': 1, '2024': 1, '2025': 2}
  CSS 461    total=6    latest=WIN2025  by_year={'2021': 1, '2022': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 473    total=5    latest=WIN2022  by_year={'2021': 1, '2022': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 474    total=7    latest=SPR2026  by_year={'2020': 1, '2021': 1, '2022': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 475    total=35   latest=WIN2026  by_year={'2020': 1, '2021': 6, '2022': 6, '2023': 6, '2024': 6, '2025': 6, '2026': 4}
  CSS 478    total=22   latest=WIN2026  by_year={'2020': 1, '2021': 4, '2022': 4, '2023': 4, '2024': 4, '2025': 4, '2026': 1}
  CSS 480    total=11   latest=SUM2024  by_year={'2021': 3, '2022': 2, '2023': 2, '2024': 2, '2025': 1, '2026': 1}
  CSS 481    total=9    latest=WIN2026  by_year={'2021': 1, '2023': 1, '2024': 2, '2025': 3, '2026': 2}
  CSS 483    total=5    latest=WIN2026  by_year={'2021': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 484    total=4    latest=WIN2023  by_year={'2022': 1, '2023': 2, '2024': 1}
  CSS 485    total=5    latest=WIN2026  by_year={'2021': 1, '2023': 1, '2024': 1, '2025': 1, '2026': 1}
  CSS 486    total=6    latest=WIN2025  by_year={'2020': 1, '2021': 1, '2022': 1, '2023': 1, '2025': 2}
  CSS 487    total=5    latest=SPR2026  by_year={'2020': 1, '2021': 1, '2022': 1, '2023': 1, '2026': 1}
  CSS 488    total=1    latest=SPR2025  by_year={'2025': 1}
  CSS 490    total=30   latest=WIN2026  by_year={'2020': 2, '2021': 5, '2022': 5, '2023': 4, '2024': 5, '2025': 5, '2026': 4}
  CSS 495    total=23   latest=WIN2026  by_year={'2020': 1, '2021': 4, '2022': 4, '2023': 4, '2024': 4, '2025': 4, '2026': 2}
  CSS 496    total=20   latest=WIN2026  by_year={'2020': 1, '2021': 2, '2022': 3, '2023': 3, '2024': 3, '2025': 5, '2026': 3}
  CSS 497    total=123  latest=WIN2026  by_year={'2020': 2, '2021': 26, '2022': 26, '2023': 9, '2024': 28, '2025': 18, '2026': 14}
  CSS 498    total=46   latest=WIN2026  by_year={'2020': 2, '2021': 8, '2022': 8, '2023': 8, '2024': 8, '2025': 8, '2026': 4}
  CSS 499    total=46   latest=WIN2026  by_year={'2020': 2, '2021': 8, '2022': 8, '2023': 8, '2024': 8, '2025': 8, '2026': 4}
```

</details>


**Tool: Bash**
*Detail view of AI courses and phase-out candidates*
```bash
python3 -c "
import json
# Look at specific AI-related and candidate-for-change courses in detail
for course in ['CSS 382','CSS 486','CSS 487','CSS 488','CSS 444','CSS 485','CSS 434','CSS 448','CSS 484','CSS 452']:
    fname = course.replace(' ','%20') + '.json'
    try:
        d = json.load(open(fname))
        terms = [(r['term'], r.get('section','?'), r.get('instructor','?')) for r in d.get('records',[])]
        print(f'{course}: {len(terms)} sections')
        for t,s,i in sorted(terms):
            print(f'  {t} sec={s} instr={i}')
        print()
    except FileNotFoundError:
        print(f'{course}: NOT IN DATA (never offered)')
        print()
" 2>&1

```

<details><summary>Tool Result</summary>

```
CSS 382: 16 sections
  SPR2021 sec=A instr=Pisan,Yusuf
  SPR2022 sec=A instr=Kartha,Neelakantan
  SPR2023 sec=A instr=Pisan,Yusuf
  SPR2024 sec=A instr=Stanev,Roger
  SPR2025 sec=A instr=Kartha,Neelakantan
  SPR2026 sec=A instr=Pisan,Yusuf
  SUM2021 sec=A instr=Stanev,Roger
  SUM2022 sec=A instr=Stanev,Roger
  SUM2023 sec=A instr=Stanev,Roger
  SUM2024 sec=A instr=Stanev,Roger
  WIN2021 sec=A instr=Pisan,Yusuf
  WIN2022 sec=A instr=Pisan,Yusuf
  WIN2023 sec=A instr=Stanev,Roger
  WIN2024 sec=A instr=Stanev,Roger
  WIN2025 sec=A instr=Stanev,Roger
  WIN2026 sec=A instr=Champion,Mia

CSS 486: 6 sections
  AUT2020 sec=A instr=Si,Dong
  AUT2021 sec=A instr=Si,Dong
  AUT2022 sec=A instr=Si,Dong
  AUT2023 sec=A instr=Si,Dong
  AUT2025 sec=A instr=Si,Dong
  WIN2025 sec=A instr=Mashhadi,Afra

... (25 lines omitted) ...

  AUT2022 sec=A instr=Alicherry,Mansoor
  AUT2023 sec=A instr=Fukuda,Munehiro
  AUT2024 sec=A instr=Fukuda,Munehiro
  AUT2025 sec=A instr=Joshi,Sanjay
  SPR2021 sec=A instr=Fukuda,Munehiro
  SPR2022 sec=A instr=Fukuda,Munehiro

CSS 448: 5 sections
  AUT2022 sec=A instr=Hogg,Jim
  AUT2023 sec=A instr=Hogg,Jim
  AUT2024 sec=A instr=Rahman,Muntasir Raihan
  WIN2021 sec=A instr=Hogg,Jim
  WIN2022 sec=A instr=Hogg,Jim

CSS 484: 4 sections
  AUT2023 sec=A instr=Chen,Min
  AUT2024 sec=A instr=Chen,Min
  WIN2022 sec=A instr=Chen,Min
  WIN2023 sec=A instr=Chen,Min

CSS 452: 4 sections
  WIN2021 sec=A instr=Sung,Kelvin
  WIN2022 sec=A instr=Sung,Kelvin
  WIN2023 sec=A instr=Sung,Kelvin
  WIN2024 sec=A instr=Sung,Kelvin
```

</details>


Now I have the complete picture. Let me now produce the updated proposal (Draft 2) and the three surveys simultaneously.

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/CurriculumProposal-Draft2.md`
```md
# CSS Curriculum Transition Plan: Preparing Graduates for an AI-Transformed Industry

**Version:** Draft 2
**Date:** June 2026
**Audience:** CSS Faculty
**Changes from Draft 1:** Incorporated actual course offering data from schedule records (AUT2020-WIN2026); clarified CSS 382 role (modify AND add new course); added three options for creating room in the required core; moved ABET to a note only; added course activity tiers.

---

## Executive Summary

The computing job market has undergone a structural shift. AI tools now automate a significant portion of the work previously done by junior software engineers, reducing demand for undifferentiated entry-level hires while raising the baseline competency expected of those who are hired. CSS graduates who cannot work effectively alongside AI tools are at a disadvantage; those who understand AI deeply enough to build, evaluate, and responsibly deploy it are in high demand.

This proposal outlines a three-phase curriculum transition covering 2026-27 through 2028-29. The goal is not to replace foundational CS education - algorithms, systems, software engineering, and mathematics remain essential - but to integrate AI throughout the curriculum and ensure every graduate has practical AI fluency.


... (406 lines omitted) ...


3. **CSS 370 status:** Would faculty support moving CSS 370 from required to recommended elective (Option C)? What would be lost?

4. **Dormant course cleanup:** Are there any courses on the Tier 4 list that faculty believe should be retained and scheduled? If so, who would teach them?

5. **Faculty capacity:** Which instructors are willing to pilot Phase 1 modifications in Autumn 2026? Who could lead the CSS 4xx course development?

6. **CSS 488 (NLP):** This was offered only once (SPR2025). Is it continuing? Should it be developed further or folded into CSS 4xx as a module?

7. **Assessment:** How will the department measure whether changes are producing intended outcomes? Who is responsible for tracking placement rates and employer feedback year over year?

---

*Draft 2 - For faculty discussion. All sections are provisional until faculty decisions are made on the open questions in Assumptions.md.*

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/CurriculumProposal-Draft2.md (file state is current in your context — no need to Read it back)
```

</details>


Now create the three surveys:

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/Survey-Faculty-AIReadiness.md`
```md
# CSS Faculty AI Readiness Survey

**Purpose:** Inform the curriculum transition planning process. Responses will be used to identify professional development needs, understand current AI integration in courses, and plan who can teach new or modified AI-focused content.

**Audience:** All CSS teaching faculty (full-time, affiliate, lecturer)
**Delivery:** Email link; anonymous option available; ~10 minutes to complete
**Suggested deadline:** July 31, 2026

---

## Section 1: Background

**Q1.** What is your primary teaching track?
- [ ] Full-time (tenure-track or tenured)
- [ ] Full-time teaching faculty (non-tenure-track)

... (142 lines omitted) ...


## Section 6: Course Development Interest

**Q19.** Are there specific new courses you would be interested in developing or teaching? (Open-ended)

**Q20.** Would you be willing to volunteer for the Curriculum AI Task Force (estimated 2-3 hours/month, Autumn 2026 - Spring 2027)?
- [ ] Yes
- [ ] Possibly - contact me to discuss
- [ ] No, but I want to be kept informed
- [ ] No

---

*Thank you for completing this survey. Results will be shared with the full faculty in aggregate form before the end of Summer 2026 to inform the curriculum planning process.*

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/Survey-Faculty-AIReadiness.md (file state is current in your context — no need to Read it back)
```

</details>


**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/Survey-Student-AIReadiness.md`
```md
# CSS Student AI Readiness Survey

**Purpose:** Help the CSS Department understand students' current AI skills, how prepared students feel for the job market, and what curriculum changes would be most valuable.

**Audience:** All CSS undergraduate majors (CSSE and AC programs)
**Delivery:** Canvas announcement + email; anonymous; ~8 minutes
**Suggested deployment:** First week of Autumn 2026

---

## Section 1: About You

**Q1.** Which program are you in?
- [ ] BS Computer Science & Software Engineering (CSSE)
- [ ] BA Applied Computing (AC)

... (150 lines omitted) ...

- [ ] Probably not - my schedule is too full already

**Q19.** What would be most useful to you right now in terms of AI skill development? (Choose one)
- [ ] A 1-2 credit workshop or seminar on AI tools and prompt engineering (no prereqs)
- [ ] A full 5-credit course on building AI-powered applications
- [ ] AI content integrated into existing required courses (SE, algorithms, capstone)
- [ ] More AI electives I can choose from
- [ ] Practical industry-style AI projects through capstone or internships

**Q20.** Is there anything else the CSS Department should know as it updates the curriculum? (Open-ended, optional)

---

*Your responses are anonymous and will be used to improve the CSS curriculum. Results will be shared with faculty in aggregate form. Thank you for taking the time to respond.*

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/Survey-Student-AIReadiness.md (file state is current in your context — no need to Read it back)
```

</details>


**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/Survey-Employer-SkillsNeeded.md`
```md
# Employer and Industry Partner Skills Survey

**Purpose:** Inform the CSS Department's curriculum planning as it prepares graduates for an AI-transformed job market. We want to understand what skills you most need from new computing hires, and how the job market has shifted in the past two years.

**Audience:** CSS capstone sponsors, industry advisory board members, alumni who are hiring managers, and employers who have hired CSS graduates.
**Delivery:** Email with survey link; 10-15 minutes; all responses confidential.
**Suggested deployment:** October 2026

---

## Section 1: About Your Organization

**Q1.** What best describes your organization?
- [ ] Large tech company (1000+ employees)
- [ ] Mid-size tech company (100-999 employees)

... (146 lines omitted) ...

- [ ] Participating in an industry advisory session on curriculum
- [ ] Offering a summer project or research collaboration
- [ ] None of the above at this time

**Q18.** Contact information (optional, for follow-up)

Name: _______________
Title: _______________
Organization: _______________
Email: _______________

---

*Thank you for your input. Results will be shared with CSS faculty in aggregate form and will directly inform curriculum decisions. Individual responses will remain confidential.*

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/Survey-Employer-SkillsNeeded.md (file state is current in your context — no need to Read it back)
```

</details>


Now update CHANGES.md and BRIEFING.md:

**Tool: Edit**
Editing `/Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md`
```diff
- 2026-06-06 [plan] Created Assumptions.md (28 assumptions/decisions, 3 surveys, info-gap table) and CurriculumProposal-Draft1.md (3-phase plan 26-27 through 28-29+). Updated BRIEFING.md with project scope and curriculum snapshot.
+ 2026-06-06 [plan] Created Assumptions.md (28 assumptions/decisions, 3 surveys, info-gap table) and CurriculumProposal-Draft1.md (3-phase plan 26-27 through 28-29+). Updated BRIEFING.md with project scope and curriculum snapshot.
+ 2026-06-06 [code] Analyzed sources/uwb/ schedule data (AUT2020-WIN2026); produced 4-tier course activity classification. Created CurriculumProposal-Draft2.md: two-track AI approach (modernize 382 + new CSS 4xx), 4 options for making room in CSSE core, dormant course cleanup list, ABET noted but not a blocker. Created 3 survey instruments: Survey-Faculty-AIReadiness.md, Survey-Student-AIReadiness.md, Survey-Employer-SkillsNeeded.md.
```

<details><summary>Tool Result</summary>

```
The file /Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md has been updated successfully. (file state is current in your context — no need to Read it back)
```

</details>


Here is what was produced and the key findings from the course data.

---

## What was built

**[CurriculumProposal-Draft2.md](CurriculumProposal-Draft2.md)** replaces Draft 1 with data-grounded content:

**[Survey-Faculty-AIReadiness.md](Survey-Faculty-AIReadiness.md)** - 20 questions covering expertise self-assessment, current tool use, course integration, capacity for new content, and opinions on curriculum direction (including the sensitive "which core course would you least object to changing" question).

**[Survey-Student-AIReadiness.md](Survey-Student-AIReadiness.md)** - 20 questions covering job market confidence, skill gaps vs. job postings, tool use, curriculum satisfaction ratings by area, and desired changes.

**[Survey-Employer-SkillsNeeds.md](Survey-Employer-SkillsNeeded.md)** - 18 questions covering hiring trends, skill importance ratings, common gaps in recent graduates, AI-related work new hires do, and curriculum advice.

---

## Key findings from the schedule data

**Confirming concerns:**
- CSS 382 is healthy (3 instructors, consistent) but only runs once per term - it cannot carry required AI load alone
- CSS 486 (Machine Intelligence) is almost entirely one instructor (Si Dong) with gaps; a single departure risk
- CSS 448 (Compilers) and CSS 484 (Multimedia Data Processing) have quietly stopped being offered (no 2025-26 offerings)
- CSS 482 (Expert Systems) has never appeared in the UWB schedule data - it is already de facto dormant
- CSS 488 (NLP) has been offered exactly once

**For the options on making room in the CSSE core:** the proposal presents 4 options (A: required AI elective with no core change; B: expand CSS 360; C: drop CSS 370 from required; D: merge CSS 350 and 360), with a recommendation to start with Option A while gathering data to support Option C if needed.

**Next questions:** Are there additional data points you want pulled from the sources? And should we start refining any of the three surveys now, or move to a different section of the proposal?

</details>

## User

A4. AI fluency is a core competency

A6. What is the best way to inventory faculty skills? Suggest multiple ways forward

A7. Current teaching load is 8 courses for teaching track faculty per year and 5 courses for tenure track faculty per year. Plan for moderate and generous funding scenarios. CSS already uses a lot of adjunct professors, 50% of courses is taught by adjuncts, so providing additional course releases to faculty even if there is funding can be difficult.

A8. 3 new teaching track faculty and 1 new tenure track faculty is tarting in Sept 2026. Expecting additional retirments, so more faculty will be hired, but total number of lines will be stable with the new additions.

A13. Changes will only apply to new incoming students but existing students will have the option to switch to new requirements if they request it

A15. Will leave out ABET concerns at this time

A20. It will require some of both. In the short term, modifying existing courses to weave in AI content with the intention fo bringing in new AI courses in 27-28 or later

A22.  A new course on "AI for Software Engineers" will be better as it wont have curriculum baggage 

A23. Not all courses are offered each quarter. Eliminating low enrollment and outdated courses is possible.

<details>
<summary>Assistant (6 steps)</summary>

Let me update Assumptions.md with all these decisions, then produce a Draft 3 proposal that reflects them.

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/Assumptions.md`
```md
# Assumptions and Key Decisions

Working document for the CSS Curriculum AI Transition Plan.
Status markers: **DECIDED**, **OPEN**, or **ASSUMPTION**.

Last updated: June 2026

---

## 1. Context and Scope

**A1 (assumption):** The decline in CS internship and entry-level hiring is structural, not cyclical. AI is permanently changing the composition of software engineering teams, reducing demand for undifferentiated junior developers while increasing demand for engineers who can work effectively alongside AI tools.

**A2 (assumption):** Graduates who can use AI as a force-multiplier will be more competitive than those who cannot, even for traditional roles.


... (154 lines omitted) ...


---

## 8. Open Decisions Remaining

| ID | Decision | Status | Notes |
|---|---|---|---|
| A16 | Graduate employment data | OPEN | Career Center pull needed |
| A17 | Student skill gap data | OPEN | Deploy student survey Autumn 2026 |
| A18 | Employer feedback | OPEN | Deploy employer survey Oct 2026 |
| Which core course makes room for CSS 4xx | OPEN | Options C or D from Draft 3 proposal; faculty vote needed |
| New hire AI expertise | OPEN | Need to confirm AI teaching capacity of Sept 2026 new hires |
| CSS 4xx lead instructor | OPEN | Depends on new hire or volunteer from existing faculty |
| Catalog phase-out process | OPEN | Need confirmation from advising on degree audit impact |

```

<details><summary>Tool Result</summary>

```
The file /Users/pisan/bitbucket/pisanuw/curriculum-css/Assumptions.md has been updated successfully. (file state is current in your context — no need to Read it back)
```

</details>


Now Draft 3 of the proposal:

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/CurriculumProposal-Draft3.md`
```md
# CSS Curriculum Transition Plan: Preparing Graduates for an AI-Transformed Industry

**Version:** Draft 3
**Date:** June 2026
**Audience:** CSS Faculty
**Changes from Draft 2:** Reflects faculty decisions: AI fluency is a core competency (required, not elective); new standalone CSS 4xx confirmed; course elimination confirmed as in-scope; two funding scenarios added; ABET removed; teaching load and faculty capacity constraints incorporated; 4 new faculty hires (Sept 2026) noted as key capacity variable.

---

## Executive Summary

The computing job market has undergone a structural shift. AI tools now handle a significant portion of the work previously done by junior software engineers, raising the bar for what employers expect from new graduates. The CSS Department has made a clear decision: **AI fluency is a core competency** required of all graduates, not an optional specialization.

This proposal outlines a three-phase curriculum transition from 2026 through 2028-29:


... (476 lines omitted) ...


4. **CSS 4xx in AC:** Should CSS 4xx be required for all AC students, or required only in certain concentrations?

5. **Dormant course confirmation:** Are there instructors who plan to resume offering CSS 448, CSS 452, or CSS 484? If so, they should not be on the phase-out list.

6. **CSS 488 (NLP) future:** Offered once by one instructor. Should it continue, grow, or be integrated into CSS 4xx as a module?

7. **Funding scenario:** Which funding scenario is the department working toward? This determines the Phase 1 scope.

8. **Task Force formation:** Who volunteers for the Curriculum AI Task Force?

---

*Draft 3 - For faculty vote on the key structural question (Option C vs. alternatives) and for Task Force formation. Decisions made here will be reflected in Draft 4, which will be the version shared with the Dean's office.*

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/CurriculumProposal-Draft3.md (file state is current in your context — no need to Read it back)
```

</details>


**Tool: Edit**
Editing `/Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md`
```diff
- 2026-06-06 [code] Analyzed sources/uwb/ schedule data (AUT2020-WIN2026); produced 4-tier course activity classification. Created CurriculumProposal-Draft2.md: two-track AI approach (modernize 382 + new CSS 4xx), 4 options for making room in CSSE core, dormant course cleanup list, ABET noted but not a blocker. Created 3 survey instruments: Survey-Faculty-AIReadiness.md, Survey-Student-AIReadiness.md, Survey-Employer-SkillsNeeded.md.
+ 2026-06-06 [code] Analyzed sources/uwb/ schedule data (AUT2020-WIN2026); produced 4-tier course activity classification. Created CurriculumProposal-Draft2.md: two-track AI approach (modernize 382 + new CSS 4xx), 4 options for making room in CSSE core, dormant course cleanup list, ABET noted but not a blocker. Created 3 survey instruments: Survey-Faculty-AIReadiness.md, Survey-Student-AIReadiness.md, Survey-Employer-SkillsNeeded.md.
+ 2026-06-06 [decision] Key decisions recorded: AI fluency is core competency (A4); A6 five faculty inventory methods; A7 8/5 course loads, 50% adjuncts, moderate+generous funding scenarios; A8 4 new faculty Sept 2026; A13 new students only with opt-in; A15 ABET dropped; A20 modify existing then new courses; A22 standalone CSS 4xx confirmed; A23 course elimination in scope. Updated Assumptions.md, created CurriculumProposal-Draft3.md with Option C recommendation (CSS 370 demoted to recommended to make room for required CSS 4xx).
```

<details><summary>Tool Result</summary>

```
The file /Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md has been updated successfully. (file state is current in your context — no need to Read it back)
```

</details>


Here is a summary of what changed and why.

---

## Key changes in Draft 3 and updated Assumptions

**A4 (AI as core competency)** cascades into the entire proposal: CSS 4xx is now a required course, not a required elective. This forced a concrete answer to "what makes room for it."

**Recommended answer: Option C - CSS 370 moves from required to strongly recommended.** The rationale is that CSS 370's content (UML, DFDs, formal requirements modeling) has the most overlap with CSS 360 and CSS 350, and the industry has moved away from heavy upfront modeling. CSS 370 keeps running and students are advised to take it, but it no longer crowds out the AI requirement. This is the one faculty decision the proposal explicitly calls for a vote on.

**A6 (faculty inventory)** now has five concrete methods ranked by accuracy vs. cost: anonymous survey (fast), syllabus audit (reveals actual vs. reported), publication review (identifies hidden expertise), chair conversations (most accurate), and bootcamp observation (practical gauge). The recommendation is to combine methods 1, 4, and 5.

**A7 (teaching loads and adjuncts)** shapes the two funding scenarios into concrete dollar estimates. The Moderate scenario (~$24K-34K for Phase 1) is achievable through discretionary funds; the Generous scenario (~$56K-78K) requires a budget request to the Dean. Both scenarios acknowledge that adjunct supply for AI content is the real constraint, not money alone.

**A8 (4 new faculty)** is flagged as the biggest near-term lever: if even one or two of the new hires has AI teaching capacity, the CSS 4xx timeline becomes much easier. The proposal explicitly recommends making AI teaching a criterion in all future hiring decisions.

**Remaining open questions for faculty:** (1) Vote on Option C vs. alternatives, (2) confirm which new hires have AI expertise, (3) form the Curriculum AI Task Force, (4) choose the funding scenario to pursue.

</details>

## User

/close

<details>
<summary>/close steps</summary>

# /close — Session Close Protocol

Run this at the end of a session to persist state for the next session.

## Steps

1. Read the current `CHANGES.md` and `BRIEFING.md`.

2. Review all work done in this session. For each unrecorded shift in decisions, plans, scope, documents, external context, or code needing project-level explanation:
   - Append a line to `CHANGES.md`: `YYYY-MM-DD [type] description` (one line, max 200 chars)
   - Types: `decision`, `plan`, `doc`, `scope`, `code`, `note`

3. Review whether any of the following changed during this session:
   - Project purpose or scope
   - Key architectural or design decisions
   - Non-goals or explicit exclusions
   - Breaking changes (note reason and impact)

   If any of the above changed, update `BRIEFING.md` accordingly. Keep it concise but sufficient to brief a new contributor.

4. Write both files.

5. Compute this session's token usage and estimated cost from the Claude Code
   transcript (Claude Code records per-turn `usage` there). Run this (stdlib
   only; it picks the most-recently-modified transcript for the current project,
   which is this session):

   ```bash
   python3 - <<'PY'
   import json, glob, os
   proj = os.path.expanduser("~/.claude/projects/" + os.getcwd().replace("/", "-"))
   files = sorted(glob.glob(proj + "/*.jsonl"), key=os.path.getmtime)
   if not files:
       files = sorted(glob.glob(os.path.expanduser("~/.claude/projects/*/*.jsonl")), key=os.path.getmtime)
   if not files:
       print("session usage: unavailable (no transcript found)"); raise SystemExit
   path = files[-1]
   PRICES = {"opus": (5.0, 25.0), "sonnet": (3.0, 15.0), "haiku": (1.0, 5.0)}  # $/1M (in, out)
   def rate(m):
       m = (m or "").lower()
       for k, v in PRICES.items():
           if k in m: return v
       return PRICES["opus"]
   tin = tout = tcw = tcr = 0; cost = 0.0; models = {}
   with open(path) as f:
       for line in f:
           try: o = json.loads(line)
           except Exception: continue
           msg = o.get("message") or {}
           u = msg.get("usage")
           if not u: continue
           model = msg.get("model", "") or ""
           if model: models[model] = models.get(model, 0) + 1
           i = u.get("input_tokens", 0) or 0; out = u.get("output_tokens", 0) or 0
           cw = u.get("cache_creation_input_tokens", 0) or 0
           cr = u.get("cache_read_input_tokens", 0) or 0
           tin += i; tout += out; tcw += cw; tcr += cr
           ri, ro = rate(model)
           cost += i/1e6*ri + out/1e6*ro + cw/1e6*ri*1.25 + cr/1e6*ri*0.10
   print(f"models: {', '.join(sorted(models)) or 'unknown'}")
   print(f"tokens_total: {tin+tcw+tcr+tout}")
   print(f"breakdown: in {tin:,} / cache-write {tcw:,} / cache-read {tcr:,} / out {tout:,}")
   print(f"est_cost_usd: {cost:.2f}")
   PY
   ```

   Cost is at list price (cache writes billed 1.25x input, cache reads 0.1x).
   If it prints "unavailable" or errors, report usage as unavailable rather than
   failing the close.

6. Output exactly this, then stop:

```
Session closed.
CHANGES.md: [number] new entries appended.
BRIEFING.md: [updated | unchanged].
Session usage: [tokens_total] tokens (in / cache-write / cache-read / out: [breakdown]) on [models].
Estimated cost at API list price: $[est_cost_usd] (subscription marginal cost: ).
```

Do not skip this protocol. If nothing recordable changed, say so and confirm both files are unchanged.

</details>

<details>
<summary>Assistant (6 steps)</summary>

**Tool: Read**
Reading `/Users/pisan/bitbucket/pisanuw/curriculum-css/CHANGES.md`

**Tool: Read**
Reading `/Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md`

<details><summary>Tool Result</summary>

```
1	# Changes
2	
3	Format: `YYYY-MM-DD [type] description` (max 200 chars). Types: decision, plan, doc, scope, code, note.
4	
5	2026-06-06 [note] Initialized.
6	2026-06-06 [plan] Created Assumptions.md (28 assumptions/decisions, 3 surveys, info-gap table) and CurriculumProposal-Draft1.md (3-phase plan 26-27 through 28-29+). Updated BRIEFING.md with project scope and curriculum snapshot.
7	2026-06-06 [code] Analyzed sources/uwb/ schedule data (AUT2020-WIN2026); produced 4-tier course activity classification. Created CurriculumProposal-Draft2.md: two-track AI approach (modernize 382 + new CSS 4xx), 4 options for making room in CSSE core, dormant course cleanup list, ABET noted but not a blocker. Created 3 survey instruments: Survey-Faculty-AIReadiness.md, Survey-Student-AIReadiness.md, Survey-Employer-SkillsNeeded.md.
8	2026-06-06 [decision] Key decisions recorded: AI fluency is core competency (A4); A6 five faculty inventory methods; A7 8/5 course loads, 50% adjuncts, moderate+generous funding scenarios; A8 4 new faculty Sept 2026; A13 new students only with opt-in; A15 ABET dropped; A20 modify existing then new courses; A22 standalone CSS 4xx confirmed; A23 course elimination in scope. Updated Assumptions.md, created CurriculumProposal-Draft3.md with Option C recommendation (CSS 370 demoted to recommended to make room for required CSS 4xx).
9	
```

</details>


<details><summary>Tool Result</summary>

```
1	# Briefing
2	
3	- **Purpose:** Develop a multi-year curriculum change proposal for the UWB CSS Department to equip graduates with skills needed in an AI-transformed job market.
4	- **Audience:** CSS Faculty
5	- **Current scope:** Three phased deliverables - (1) information gaps and what to collect, (2) assumptions/decisions inventory, (3) draft proposal covering 26-27, 27-28, and 28-29+ with concrete course-level guidance.
6	- **Key decisions:** Which courses to modify vs. phase out vs. create; how fast to move given UW approval timelines; how to handle faculty upskilling; whether to require AI content in core vs. electives; how to differentiate the AC and CSSE tracks.
7	- **Non-goals:** Operational implementation details (scheduling, room assignments, faculty assignments); changes to graduate programs (separate effort); changes to admissions criteria.
8	
9	## Source material on hand
10	- Full CSS course catalog (CSS 101 - CSS 700)
11	- CSSE curriculum requirements (BS in Computer Science & Software Engineering)
12	- AC curriculum requirements (BA in Applied Computing)
13	- Syllabuses from Autumn 2021, Winter 2022, Spring 2022, Summer 2022
14	- UWB CSS Department overview (faculty areas, labs, programs)
15	- UWB Mission & Vision
16	
17	## Current curriculum snapshot
18	
19	### CSSE BS core required courses
20	CSS 143 → CSS 342 → CSS 343 → CSS 422 + CSS 430 (systems)
21	CSS 301 (writing) + CSS 350 (management) + CSS 360 (SE) + CSS 370 (design) → CSS 497 (capstone)
22	Plus 25 credits CSS electives (15 must be 400-level) + 15 credits 300-400 level electives
23	
24	### AC BA core required courses
25	CSS 301 + CSS 340 or 342 + CSS 350 + CSS 360 + CSS 421 → CSS 496 (capstone)
26	Plus concentration courses + general electives
27	
28	### Existing AI-related courses (all elective, not required)
29	- CSS 382: Introduction to AI (undergrad)
30	- CSS 444: Analyzing Biases in the Age of Digital Data (undergrad)
31	- CSS 485: Artificial Neural Networks (undergrad)
32	- CSS 486: Machine Intelligence (undergrad)
33	- CSS 487: Computer Vision (undergrad)
34	- CSS 488: Natural Language Processing (undergrad, new)
35	- CSS 576: Cybersecurity and AI (grad)
36	- CSS 581: Machine Learning (grad)
37	- CSS 582: Interpretable ML (grad)
38	- CSS 586: Deep Learning and AI (grad)
39	
```

</details>


CHANGES.md is fully current. BRIEFING.md needs updating to reflect the key decisions made this session. Let me update it, then compute costs.

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md`
```md
# Briefing

- **Purpose:** Develop a multi-year curriculum change proposal for the UWB CSS Department to equip graduates with skills needed in an AI-transformed job market.
- **Audience:** CSS Faculty
- **Current scope:** Three phased deliverables - (1) information gaps and what to collect, (2) assumptions/decisions inventory, (3) iterating draft proposal covering 26-27, 27-28, and 28-29+ with concrete course-level guidance. Now at Draft 3.
- **Non-goals:** Operational implementation details (scheduling, room assignments); changes to graduate programs (separate effort); changes to admissions criteria; ABET compliance analysis (explicitly excluded for now).

## Key Decisions Made (as of June 2026)

- **AI fluency is a core competency** for all graduates - not a specialization or optional elective track
- **Two-track AI response:** Modernize CSS 382 (conceptual foundations) AND create new standalone CSS 4xx "AI for Software Engineers" (practical integration) - both needed, different purposes
- **CSS 4xx is required**, not just recommended; must appear in CSSE required core and AC required core
- **Recommended restructuring (Option C):** CSS 370 (Analysis and Design) moves from required to strongly recommended elective, freeing the 5-credit slot for CSS 4xx
- **Timeline:** Modify existing courses in 2026-27; new courses launch 2027-28
- **Faculty context:** 8 courses/year teaching track; 5 courses/year tenure track; ~50% adjuncts; course releases are hard even with funding

... (46 lines omitted) ...

CSS 301 + CSS 340 or 342 + CSS 350 + CSS 360 + CSS 421 → CSS 496 (capstone)
Plus concentration courses + general electives

### Existing AI-related courses (all elective, thin offering history)
- CSS 382: Intro AI - healthiest; 3 instructors; 2-3 sections/year (to be modernized)
- CSS 444: Biases in Digital Data - 1/year, Winter only
- CSS 485: Artificial Neural Networks - 1/year, reviving
- CSS 486: Machine Intelligence - 1/year, single instructor risk (Si Dong)
- CSS 487: Computer Vision - 1/year; was absent 2023-25; returned SPR2026
- CSS 488: NLP - offered once only (SPR2025); future uncertain

### Dormant courses confirmed for phase-out
CSS 130, 250, 416, 450, 455, 457, 477, 482 (never offered at UWB in data)
CSS 448, 452, 484 (near-dormant; confirm with instructors before removing)

```

<details><summary>Tool Result</summary>

```
The file /Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md has been updated successfully. (file state is current in your context — no need to Read it back)
```

</details>


**Tool: Bash**
*Compute session token usage and estimated cost*
```bash
python3 - <<'PY'
import json, glob, os
proj = os.path.expanduser("~/.claude/projects/" + os.getcwd().replace("/", "-"))
files = sorted(glob.glob(proj + "/*.jsonl"), key=os.path.getmtime)
if not files:
    files = sorted(glob.glob(os.path.expanduser("~/.claude/projects/*/*.jsonl")), key=os.path.getmtime)
if not files:
    print("session usage: unavailable (no transcript found)"); raise SystemExit
path = files[-1]
PRICES = {"opus": (5.0, 25.0), "sonnet": (3.0, 15.0), "haiku": (1.0, 5.0)}  # $/1M (in, out)
def rate(m):
    m = (m or "").lower()
    for k, v in PRICES.items():
        if k in m: return v
    return PRICES["opus"]
tin = tout = tcw = tcr = 0; cost = 0.0; models = {}
with open(path) as f:
    for line in f:
        try: o = json.loads(line)
        except Exception: continue
        msg = o.get("message") or {}
        u = msg.get("usage")
        if not u: continue
        model = msg.get("model", "") or ""
        if model: models[model] = models.get(model, 0) + 1
        i = u.get("input_tokens", 0) or 0; out = u.get("output_tokens", 0) or 0
        cw = u.get("cache_creation_input_tokens", 0) or 0
        cr = u.get("cache_read_input_tokens", 0) or 0
        tin += i; tout += out; tcw += cw; tcr += cr
        ri, ro = rate(model)
        cost += i/1e6*ri + out/1e6*ro + cw/1e6*ri*1.25 + cr/1e6*ri*0.10
print(f"models: {', '.join(sorted(models)) or 'unknown'}")
print(f"tokens_total: {tin+tcw+tcr+tout}")
print(f"breakdown: in {tin:,} / cache-write {tcw:,} / cache-read {tcr:,} / out {tout:,}")
print(f"est_cost_usd: {cost:.2f}")
PY
```

<details><summary>Tool Result</summary>

```
models: claude-sonnet-4-6
tokens_total: 6198216
breakdown: in 1,469 / cache-write 500,447 / cache-read 5,571,541 / out 124,759
est_cost_usd: 5.42
```

</details>


Session closed.
CHANGES.md: 0 new entries appended (all entries were already current).
BRIEFING.md: updated - reflects key decisions made, open questions remaining, documents produced, Option C recommendation, and dormant course list.
Session usage: 6,198,216 tokens (in 1,469 / cache-write 500,447 / cache-read 5,571,541 / out 124,759) on claude-sonnet-4-6.
Estimated cost at API list price: $5.42 (subscription marginal cost: $0).

</details>

## User

BRIEFING.md was accidentally overwritten. No saved version. Recreate it based on session history

<details>
<summary>Assistant (2 steps)</summary>

**Tool: Write**
Writing `/Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md`
```md
# Briefing

- **Purpose:** Develop a multi-year curriculum change proposal for the UWB CSS Department to equip graduates with skills needed in an AI-transformed job market.
- **Audience:** CSS Faculty
- **Current scope:** Three phased deliverables - (1) information gaps and what to collect, (2) assumptions/decisions inventory, (3) iterating draft proposal covering 26-27, 27-28, and 28-29+ with concrete course-level guidance. Now at Draft 3.
- **Non-goals:** Operational implementation details (scheduling, room assignments); changes to graduate programs (separate effort); changes to admissions criteria; ABET compliance analysis (explicitly excluded for now).

## Key Decisions Made (as of June 2026)

- **AI fluency is a core competency** for all graduates - not a specialization or optional elective track
- **Two-track AI response:** Modernize CSS 382 (conceptual foundations) AND create new standalone CSS 4xx "AI for Software Engineers" (practical integration) - both needed, different purposes
- **CSS 4xx is required**, not just recommended; must appear in CSSE required core and AC required core
- **Recommended restructuring (Option C):** CSS 370 (Analysis and Design) moves from required to strongly recommended elective, freeing the 5-credit slot for CSS 4xx
- **Timeline:** Modify existing courses in 2026-27; new courses launch 2027-28
- **Faculty context:** 8 courses/year teaching track; 5 courses/year tenure track; ~50% adjuncts; course releases are hard even with funding

... (46 lines omitted) ...

CSS 301 + CSS 340 or 342 + CSS 350 + CSS 360 + CSS 421 → CSS 496 (capstone)
Plus concentration courses + general electives

### Existing AI-related courses (all elective, thin offering history)
- CSS 382: Intro AI - healthiest; 3 instructors; 2-3 sections/year (to be modernized)
- CSS 444: Biases in Digital Data - 1/year, Winter only
- CSS 485: Artificial Neural Networks - 1/year, reviving
- CSS 486: Machine Intelligence - 1/year, single instructor risk (Si Dong)
- CSS 487: Computer Vision - 1/year; was absent 2023-25; returned SPR2026
- CSS 488: NLP - offered once only (SPR2025); future uncertain

### Dormant courses confirmed for phase-out
CSS 130, 250, 416, 450, 455, 457, 477, 482 (never offered at UWB in data)
CSS 448, 452, 484 (near-dormant; confirm with instructors before removing)

```

<details><summary>Tool Result</summary>

```
File created successfully at: /Users/pisan/bitbucket/pisanuw/curriculum-css/BRIEFING.md (file state is current in your context — no need to Read it back)
```

</details>


Restored. The content is identical to what was written at the end of the session - I had it in full context. No information was lost.

</details>

