---
created: 2026-07-27
type: workbook
status: complete
tags: [ostad, batch-02, career-vault, class-07, portfolio]
---

# Portfolio Story

**What this file is for:** one project, one structured story, so that when someone says "tell me about a project" you do not improvise.

**Why Claude needs it:** this is the file Claude reads when you ask it to draft a case study page, a LinkedIn post, or an interview answer about your work. It only knows what you decided if you wrote it down.

**Class:** Class 7. You write the EduBridge story in class. After that, one story per real project, forever.

One project gets one story. Five parts, in order. The parts are chosen so the story is about your judgment, not about the tool. A story that says "I used AI to build a booking screen" is worth nothing. A story that says "the brief was wrong about who the user was, here is how I found out, here is what I cut" is worth an interview.

When you start a new project's story, copy this file:

Ask Claude Code: *"make a copy of career-vault/02-portfolio-story.md inside a new career-vault/portfolio-stories/ folder, named after this project."* One story per project, so this file stays the template.

---

## The EduBridge example

This is the example. It is the story of the booking screen built in Class 6, written the way it should be written. Do not copy it. Your project had different problems.

### Part 1. What was the brief

"An offshore client asked us to localize their existing UK and AU tutoring marketplace for Bangladesh. The brief was polished. Three-week sprint, MVP scope, desktop-first, Stripe for payment, students as the primary user."

### Part 2. How I directed AI, and what I built

"I ran brief interrogation before anything got drawn, which is what surfaced the contradictions in part 3. I wrote the design tokens before a single screen existed, so the system was locked before Claude could invent its own spacing scale. Then I used Claude Code to write the HTML and CSS for one screen.

The split was this. Claude wrote the markup. I chose the screen, the layout order, the fold position, the copy on the button, and the motion budget. I tested the result on a sub-15K taka Android on throttled 3G, which is where two of the rejections in part 4 came from.

What I built: the tutor booking request screen. Parent-facing, mobile, max-width 400px. Tutor name, photo below the fold to save bandwidth, verified-document badges for NID and qualifications, price in BDT, and exactly one call to action."

### Part 3. What problem did I solve

"The brief and the reality were two different projects, and nobody had said so out loud.

The brief said desktop-first. The local PM said mobile is the only thing that matters here. The brief assumed one global card checkout, which converts at 19% in the UK and would have stalled here; most of these users pay with bKash or Nagad, and that is a different flow shape, not a different button. The brief put students as the primary user, but parents hold the phone, the money, and the veto.

So the problem I actually solved was not 'design a booking screen.' It was 'this brief will produce a product nobody here can use, and someone has to say that in week one instead of week three.' I rewrote the brief: parent-first, mobile-first, bKash and Nagad, Bangla as a requirement and not a phase two, trust signals ahead of aesthetics. Three weeks meant one screen only, so search and onboarding went out of scope on purpose."

### Part 4. What did I reject, and why

"Claude's first booking screen had a large tutor photo above the fold and a 400ms fade-in on load. I cut both. The photo pushes the booking button below the fold and costs bandwidth on a connection that cannot spare it. The fade-in reads as a broken page on the devices these parents actually hold.

I also rejected the first three versions of the button copy. Claude kept writing 'Get Started,' which tells a parent nothing about what happens when they tap. It became 'Send Booking Request,' which says who is doing what.

None of this reached a reviewer. It got cut before the screen was shown to anyone."

### Part 5. What was the outcome, including what I got wrong

"Outcome: a class project, so it did not ship to real users. It was reviewed by a senior product designer, who found two things I had missed. There is no error state when a bKash payment fails, and the verified badges have no offline fallback. Both are on my followup list with a fix written for each.

What I got wrong: I assumed parents wanted document-level verification visible on the screen, and I designed three badge variants before I tested that assumption with anyone. When I finally tested with five parents, three of them said they would rather see a short introduction video from the tutor than a row of document badges. I had spent two days on the wrong solution. The mistake was not the badges. It was testing the assumption after the design instead of before it."

Do not leave this part out and do not soften it. An honest failure in a portfolio story is the single fastest way to read as someone who has done real work. Every experienced designer in the room has a story like this. The juniors are the ones who claim they do not.

### The sixty-second version

Compressed, for a recruiter call.

"I rebuilt the booking screen of a tutoring marketplace for the Bangladesh market. The client brief said desktop-first and English-only; the real users are parents on entry-level Android phones switching between Bangla and English. I redirected the brief to parent-first and mobile-first, then built one screen end to end including the HTML: verified-tutor signal, bKash payment path, loads on 3G. Reviewed by a senior designer, who found two gaps I had missed."

---

## YOUR TURN

<!-- COURSE SCAFFOLDING: delete everything above YOUR TURN once you have filled it in. This becomes your real working file. -->

Write the story of the screen you built in Class 6. Answer each part in place, in order. Full sentences, first person, past tense.

Two rules while you write. Every sentence in parts 2 through 5 should have you as the subject of the verb, not Claude. And no part is optional, including part 5.

When the five parts are drafted, open Claude Code at the root of this workspace on the latest Sonnet at medium effort and ask it to find every sentence where the tool is the subject instead of you, and every claim you have not backed with something specific. Then fix them yourself. Do not let it rewrite the story; it will make it sound like everyone else's. Fits in one session.

### 1. What was the brief?

One paragraph, in plain language. What you were asked to do, including the parts of the ask that turned out to be wrong. Write it as the client wrote it, not as you wish they had.

### 2. How did you direct AI, and what did you build?

Two paragraphs. First: what you kept and what you handed over. Be exact. Which decisions were yours, which keystrokes were Claude's, and what you did to check the result. Second: the one screen or flow you actually built, described specifically enough that someone could picture it.

### 3. What problem did you solve?

One or two paragraphs. Not the task you were given. The problem underneath it. What was contradictory, missing, or wrong in the brief, how you found it, and what you changed as a result. This is the part most designers skip, and it is the part that gets you hired.

### 4. What did you reject, and why?

At least two things Claude produced that you said no to, with the reason for each. The reason matters more than the rejection. "It looked bad" is not a reason. "It pushes the primary action below the fold on the device our users hold" is a reason.

### 5. What was the outcome, and what did you get wrong?

Two parts, both required.

Outcome first: if it shipped, what happened. If it did not ship, who reviewed it and what they found. Be honest that a class project is a class project. Nobody is fooled and nobody minds.

Then the failure: one specific judgment call you regret, what happened because of it, and what you now do differently. Not "I worked too hard." Not "I missed a deadline." A decision you made with the information you had, that turned out to be wrong.

Then compress the whole story into three sentences you can say out loud on a call. Say them out loud. If they do not sound like speech, rewrite them.
