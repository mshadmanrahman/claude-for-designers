---
created: 2026-07-27
type: workbook
status: complete
tags: [ostad, batch-02, career-vault, class-08, resume]
---

# Resume Content

**What this file is for:** the source content for your resume, kept structured here so you never write one from scratch again.

**Why Claude needs it:** when you ask Claude to tailor a resume to a specific job posting, this file is what it works from. A resume built from the job description instead of from your own work reads as hollow, because it is.

**Class:** Class 8. First version in class, then updated every time you finish a project or start a job hunt.

The resume is not the document. This file is. The PDF is just formatted output. When you apply somewhere, you copy from here into a template and cut what does not fit the role. That takes twenty minutes instead of an evening.

One rule that runs through the whole file: a bullet is a decision you made with a result attached, not a task you completed. "Designed the booking screen" is a task. "Redirected the brief from student-first to parent-first after brief interrogation, which changed the whole flow" is a decision.

---

## The EduBridge example

This is the example, filled in by a designer whose only real project so far is the EduBridge screen from Class 6. That is a normal starting point. Do not copy it.

### Header

Name: full name, as it appears on your NID.
Title: the role half of your positioning sentence. "Product Designer" or "UX Designer". Not "Designer". Not "UI/UX/Graphic Designer".
Location: Dhaka, Bangladesh.
Contact: one email, one phone, one portfolio link. No more links than that.

### Profile, three or four lines

The most-read block on the page. Most recruiters read this and skip the rest, so it carries the weight.

"Product designer in Dhaka. I work on trust-first mobile experiences for people using entry-level Android phones and slow connections. One project shipped end to end so far, from a broken client brief to working HTML. I direct the decisions; Claude accelerates the execution."

Three or four lines, not a paragraph. Note what the last sentence does: it names the AI question before the recruiter has to ask it, and frames it as direction rather than dependence.

### Experience

Reverse chronological. For each role, one summary line and three to five bullets.

**Junior Product Designer, [Company] ([Month Year] to present)**

Mobile product work for a BD-market edtech marketplace.

- Interrogated the incoming client brief before design started and surfaced four contradictions, including a desktop-first requirement that conflicted with the project's own success metric. Brief was rewritten to mobile-first with client sign-off in 24 hours.
- Established the design token system before any screen existed. Colors, type scale and spacing locked in one file, which removed pixel arguments during engineering handoff.
- Built the parent-facing booking screen end to end, including HTML and CSS, on a sub-15K taka Android with throttled 3G as the test target.
- Cut a hero image and a 400ms load animation from the first build, both of which pushed the primary action below the fold on the target device.

A note on numbers. If you have a real metric, use it. If you do not, do not invent one. A made-up "improved conversion by 40%" falls apart in the first interview when someone asks how it was measured. A specific decision with no number is stronger than a fake number.

### Selected projects

If your experience section is thin, which it will be early on, this section carries the resume. Two or three projects, one line each, each pointing at its story in `career-vault/portfolio-stories/`.

- **EduBridge BD, tutor booking flow** (course project, 2026). Parent-first mobile flow with document-verified trust signals, bKash payment path, Bangla and English support. Built end to end including the HTML.

### Skills

Group them. Be specific. Cut anything you would not want to be tested on in the interview.

Design: mobile-first product design, design systems, information architecture, interaction design.

Tools: Figma, Claude Code, VS Code.

Specialized: BD market design (low-end Android, slow networks, bKash and Nagad patterns), bilingual interfaces in Bangla and English, token-based design systems.

Five items per group is plenty. "Proficient in 47 tools" tells a recruiter you are proficient in none.

### Education

- [Degree], [Institution] ([year])
- Claude for UI/UX Designers, Ostad (2026)

### What is deliberately not on this resume

The discipline half. These all look like effort and read as weakness.

- Self-rated skill bars. Figma four stars out of five reads as juvenile.
- "Team player." Empty. Replace it with one bullet describing an actual disagreement you handled.
- "Detail-oriented." Same problem.
- "Passionate about design." Everyone writes this, so it carries no information.
- A photo. Default to none unless the posting explicitly asks.
- Personal interests, unless they connect to the work. "I redesign government forms for fun" earns its line. "I love travelling" does not.

### Variants

Keep the profile and bullet selection per role type, so applying is assembly rather than writing.

Product design roles: profile and bullets emphasizing information architecture, research and system thinking.

Frontend-leaning roles: profile and bullets emphasizing Claude Code, HTML and CSS familiarity, and design-to-engineering handoff.

Agency or consulting roles: profile and bullets emphasizing brief interrogation, client pushback and owning more than one project at a time.

---

## YOUR TURN

<!-- COURSE SCAFFOLDING: delete everything above YOUR TURN once you have filled it in. This becomes your real working file. -->

Fill in each section below in place. Pull from `01-positioning.md` and `02-portfolio-story.md` rather than starting fresh; if those two files are honest, most of this is already written.

When the draft is done, open Claude Code at the root of this workspace on the latest Sonnet at medium effort and ask it to do two passes. First, find every bullet that describes a task rather than a decision, and every number you cannot source. Second, cut the whole thing to one page. Then make the edits yourself. Fits in one session.

### 1. Header and profile

Name, title, location, contact. Then the profile in three or four lines, built from your positioning sentence. Include one line that names how you work with AI, so the recruiter does not have to guess.

### 2. Experience

For each role you have had, one summary line and three to five bullets. Every bullet is a decision plus a result. Before you move on, read each bullet and ask: could someone who did nothing on this project have written this sentence? If yes, rewrite it.

If you have no design job yet, skip to section 3 and say so plainly. Nobody expects a first-year designer to have three roles.

### 3. Selected projects

Two or three, one line each. Include the Class 6 screen. For each one, link to its story file in `career-vault/portfolio-stories/`.

### 4. Skills

Three groups: design, tools, specialized. Five items maximum per group. Then delete anything you could not demonstrate live if an interviewer opened a laptop and asked you to.

### 5. Which variant are you sending?

Name the kind of role you are actually applying for right now, and write the profile paragraph for that variant. Then list which of your bullets from section 2 make the cut for it, and which get dropped.
