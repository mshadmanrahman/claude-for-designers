---
created: 2026-07-27
type: brief
status: template
tags: [edubridge, class-3, workbook, brief]
project: EduBridge Bangladesh
brief-version: "3: interrogated synthesis"
---

# EduBridge BD: Interrogated Brief

**What this file is for:** the one brief you actually design from, written by you after you have pulled apart the client brief (v1) and the PM thread (v2).

**Why Claude needs it:** v1 and v2 contradict each other in seven places. If you hand Claude both and no decision, it picks for you, quietly, and you get a screen built on the wrong user, the wrong device and the wrong payment method.

**Which class:** Class 3. You keep using it in Classes 4, 5 and 6.

<!--
COURSE NOTE for the student. This is not an instruction to Claude.

Everything between here and `## YOUR TURN` is teaching material. Delete it once your own answers are in.
-->

## How you produce it

Read `brief-v1-client.md` and `brief-v2-pm-thread.md` first. Both, in full, before you write anything.

Then, in one Claude Code session on the latest Sonnet at medium effort, opened at this project folder:

1. Run `/design-brief` with both briefs in context. It will not resolve the contradictions for you. It will name them, and it will ask you to decide.
2. Write your decisions into `## YOUR TURN` below. In your words, not Claude's.
3. Run `/persona-acid-test` on what you wrote. If the confused user, the skeptical engineer or the impatient PM can knock a section over, that section is not finished.

The skills surface the conflict. You make the call. That is the whole point of the class: a brief you agreed to without reading is a brief you will be blamed for.

## Example: the instructor's filled version

Labelled as the example. This is one designer's set of decisions, not the answer key. If your version comes out identical to this, you did not interrogate anything, you copied. The full worked version is in `brief-v3-interrogated.example.md`.

**Who is actually using this.** A 42-year-old parent in Dhaka on a sub-15K taka Android, home Wi-Fi in the evening or slow 4G during the day. Choosing a tutor for a 16-year-old preparing for HSC. Afraid of being scammed by someone claiming qualifications they do not have. Will not book until they see proof of verification, and will not commit until the total cost is obvious.

**What the contradictions actually were.** Desktop-first (v1) versus mobile-must (v2): mobile-first, because the sub-15K taka Android is the default device and desktop is the edge case. One global checkout (v1) versus the flow this market needs (v2): both paths, SSLCOMMERZ for the card minority and bKash or Nagad for everyone else. The finding is not the brand name, it is that mobile money is a different flow shape: an app switch, a PIN, an OTP, a hand-typed transaction ID and an async verification wait, which adds three to four screens and five error states the brief never budgeted for. English-only (v1) versus Bengali "strongly preferred" (v2): plan Bengali UI strings now, retrofitting is more expensive later. Students as primary (v1) versus parents as decision-makers (v2): parents, because they hold the money.

**Scope.** Building first: the parent-facing tutor booking request screen (tutor name, subject, verified badge, qualifications, hourly rate in BDT, one CTA). Out: video calling, search and discovery, tutor onboarding, translation of tutor-written content.

**Assumptions carried forward.** bKash first with Nagad likely second, priority unconfirmed. Tutors will hand over NID and qualification documents. Bengali means UI strings only. The 3-lakh budget is firm.

**Open questions.** Who issues the verified badge and who checks the documents; without an issuer the badge is decoration. What "trust is the main thing" means in practice: badge, video, phone call, or all three. Whether Nagad is in MVP.

---

## YOUR TURN

Answer each question in place. Replace the italic line with your answer; keep the heading.

### Who is actually using this

***One paragraph. Who is the primary user, on what device, on what connection, in what language, trying to do what, and afraid of what? Name the fear. Trust work is designed against a fear.***

### What the contradictions actually were

***List every place v1 and v2 disagree. For each one: your decision, and the reason. If you cannot give a reason, you have not decided, you have guessed.***

### Scope: what I am building first, and what I am not

***One sentence on the single screen or flow you will spend the rest of the course on. Then a list of things the brief hints at that you are deliberately not building.***

### Assumptions I am carrying forward

***What are you treating as true without confirmation? Write each one down so it stops being invisible. An unwritten assumption becomes someone else's fault later.***

### Open questions for Rafi or Jamie

***What blocks design progress until someone answers it? These questions are the raw material for the pushback email you send this week, so write them the way you would send them.***

<!-- COURSE SCAFFOLDING: delete everything above YOUR TURN once you have filled it in. This becomes your real working file. -->
