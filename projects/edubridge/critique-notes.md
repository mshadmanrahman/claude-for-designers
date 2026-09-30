---
created: 2026-07-27
type: note
status: template
tags: [edubridge, class-4, workbook, critique]
project: EduBridge Bangladesh
---

# EduBridge BD: Critique Notes

**What this file is for:** the record of what was actually wrong with your first-pass screen, and what you decided to change because of it.

**Why Claude needs it:** "what do you think of this?" gets you flattery. A named perspective with a named constraint gets you a real finding. This file holds the findings so Class 5 and Class 6 build the post-critique screen instead of the pre-critique one.

**Which class:** Class 4. Class 5 and Class 6 read your synthesis out of it.

<!--
COURSE NOTE for the student. This is not an instruction to Claude.

Everything between here and `## YOUR TURN` is teaching material. Delete it once your own answers are in.
-->

## How you produce it

Generate a first-pass screen from the confused brief on purpose. Then, in one Claude Code session on the latest Sonnet at medium effort:

1. Run `/design-review` on the screen. It gives you the structured pass.
2. Run `/heuristic-evaluation` on the same screen. Nielsen's ten, every finding tied to one element and one fix.
3. Run the three forced-perspective prompts below yourself, one at a time, and paste what comes back.
4. Write your own synthesis last. Claude does not get to decide what you change.

Keep this file alive after the course. Every screen you critique goes in here in the same shape.

## Example: the instructor's filled version

Labelled as the example. Shortened to one finding per perspective so you can see the shape.

**Screen being critiqued.** Tutor booking request screen, v0.1, generated straight from the confused PM brief. Tutor name, large photo, hourly rate, a generic "verified" label, a "Book Now" button.

**Confused user on a 3G phone.** "I think you want me to pay someone, but I do not know who checked this person. The word verified is sitting there with no explanation. The photo took long enough that I nearly closed the tab."

**Engineer shipping in 10 days.** "The verified label is the expensive one, because right now it is a string, and making it true means a document pipeline, a reviewer and a status field. The full-bleed photo above the fold also needs responsive art direction and a real image CDN."

**Skeptical PM.** "It will fail because a parent who does not know who verified the tutor will leave and ask a neighbour for a recommendation instead. Book Now reads like a vending machine, so the parent expects an instant confirmation and gets a pending request. And the price is shown per hour with no session total, so the parent does the maths themselves and abandons."

**My synthesis, in priority order.** (1) Replace the generic verified label with an explicit badge naming the document type; trust is the stated conversion lever. (2) Move the photo below the decision area; it costs the most on 3G and buys the least. (3) Rename "Book Now" to "Send Booking Request", so the copy matches what actually happens. (4) Show the session total in BDT, not just the hourly rate.

**What I would have missed.** On my own I would have caught the photo weight and stopped there, because it is the finding that looks like design work. The engineer perspective is what exposed that "verified" was a decoration with no system behind it, and the PM perspective is what caught the copy promising an instant booking the product cannot deliver. Neither is a visual problem, and both would have shipped.

---

## YOUR TURN

Answer each question in place. Paste Claude's real output, not a summary of it.

### Screen being critiqued

***Which screen, which version, and which brief did you generate it from? Paste a screenshot or describe it in two lines.***

### Perspective 1: confused user on a 3G phone

Run this prompt. Paste the response underneath it.

```
You are a first-time user, age 35, on a sub-15K taka Android, 3G
connection, in Bangladesh. You opened this screen because someone
sent you a link. Tell me in three sentences what you think this
screen is asking you to do, and where you got confused. Do not be
polite.
```

***Paste the response here.***

### Perspective 2: engineer who has to ship this in 10 days

```
You are an engineer who has to ship this in 10 days. List three
things in this design that will be expensive to build and explain
why, in code terms. Be specific about which CSS or interaction is
hard.
```

***Paste the response here.***

### Perspective 3: skeptical PM who has killed 20 launches

```
You are a skeptical PM who has killed 20 launches. Write three
reasons this design will fail in production. Each reason must
reference a real user behavior, not aesthetics.
```

***Paste the response here.***

### My synthesis, and what I would have missed

***What are you actually changing, in priority order, and why in that order? Then one paragraph: which finding would you not have caught on your own, and what does that tell you about your own blind spot?***

<!-- COURSE SCAFFOLDING: delete everything above YOUR TURN once you have filled it in. This becomes your real working file. -->
