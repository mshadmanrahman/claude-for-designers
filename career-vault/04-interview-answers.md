---
created: 2026-07-27
type: workbook
status: complete
tags: [ostad, batch-02, career-vault, class-08, interview]
---

# Interview Answer Bank

**What this file is for:** structured answers to the questions you will actually be asked, written down once so you are not improvising in the room.

**Why Claude needs it:** when you ask Claude to run a mock interview or tighten an answer, this file gives it your real material. Without it, it invents a career for you and you end up rehearsing someone else's.

**Class:** Class 8. First version in class, then updated after every interview you sit.

The structure is what you keep. The exact words should come out fresh. An answer you have memorized word for word sounds worse than one you have thought about, because the interviewer can hear the recital.

Every answer in this file is built on one idea: **name a decision, not a tool.** The interviewer is not trying to find out whether you used AI. They assume you did. They are trying to find out whether there is judgment behind the output. So every answer has you as the subject of the verb. I decided. I rejected. I cut. I was wrong about.

STAR is the format for the behavioral answers: situation, task, action, result. Two sentences per part, four parts, roughly sixty to ninety seconds spoken. Add a fifth line for what you learned, because that is the part interviewers actually score.

---

## The EduBridge example

This is the example, from the designer who built the Class 6 booking screen. Do not copy it. Your decisions were different, and the specificity is the whole point.

### The answer for "but didn't AI do this for you?"

You have about thirty seconds before the interviewer's opinion sets. Three beats.

Beat one, five seconds: accept the question without getting defensive.
Beat two, fifteen seconds: move the frame from outputs to decisions.
Beat three, ten seconds: land one specific example.

"Fair question, and worth asking. The way I work is that I direct the decisions and Claude makes the execution fast. On this project specifically: I decided the brief was wrong about who the user was and rewrote it around parents instead of students. I decided the screen had to load on 3G, which is why the photo sits below the fold. And I rejected the first three versions of the button copy, because 'Get Started' does not tell a parent what happens when they tap it. The HTML is the easy part. What you are hiring is the judgment that the brief was wrong."

Look at what is doing the work there. "Fair question" disarms. Three active verbs with three specific decisions attached. And the last sentence reframes what design is worth. The answer never denies AI use, because denying it would be both false and beside the point.

### STAR: "Tell me about a time you disagreed with a stakeholder"

Situation: "On the EduBridge project, the offshore client's brief said desktop-first. The local PM said mobile is the only thing that matters in this market."

Task: "I had three days before sprint kickoff and could not design both. Somebody had to resolve it, and I was the one holding the brief."

Action: "I wrote a one-page memo with three things in it: the device share for this market, the PM's own statement quoted directly, and the brief's stated success metric, which only made sense on mobile. I sent it and asked for a decision rather than arguing for one."

Result: "The client signed off on mobile-first inside 24 hours."

Learned: "Briefs are negotiable when you bring evidence instead of an opinion. The thing that moved them was their own success metric, not my preference."

### STAR: "Tell me about a time you failed"

The two traps here are picking something that is not a failure ("I care too much") and picking something disqualifying ("I missed a deadline and the client left"). What you want is a judgment call you made with the information you had, that turned out wrong, that you can explain.

Situation: "I assumed parents wanted document-level verification visible on the booking screen. NID, qualifications, background check, all as badges."

Task: "I needed to design the trust signal for the screen, and I treated my assumption as settled."

Action: "I designed three badge variants over two days. Then I tested with five parents."

Result: "Three of the five told me they would rather see a short introduction video from the tutor than a row of documents. Two days of work on the wrong solution."

Learned: "The mistake was not the badges. It was testing the assumption after the design instead of before it. Now I test the assumption first, even when I am confident, and especially when I am confident."

### STAR: "Tell me about a project you are proud of"

Use the five parts from `02-portfolio-story.md` in order: what the brief was, how you directed the work and what you built, what problem you actually solved, what you rejected, what the outcome was including what you got wrong. Under ninety seconds spoken. If it runs longer, you are describing screens instead of decisions.

### "Why do you want to work here?"

The lazy answer praises the company. The good answer connects their work to your positioning.

"I want to work somewhere that treats this market as its own thing rather than a translation of a Western product. From what I have seen, you made a specific choice about [the thing you noticed], which is the kind of decision I am trying to be in the room for. I am also at the stage where I learn fastest from people five to ten years ahead of me on this exact path, and your team has that."

If you cannot fill in the middle of that with something real about them, you should not be applying.

### Live case: "design a feature for X user under Y constraint"

You think out loud. Two rules.

Interrogate before you sketch. "Before I start, can I confirm five things: who the user is, what device they are on, what they are trying to get done, what success looks like, and what is explicitly out of scope." Then take notes on the answers. This is the same brief interrogation from Class 3, done verbally.

Make every trade-off audible. Not "I would design X." Instead: "I would design X because of Y, knowing that costs me Z." That sentence is the one that separates a designer from someone who produces screens.

If the interviewer cuts you off with "just design it," answer anyway, but note it. A team that does not want to hear the constraint question is telling you how they work.

### The process questions, which are a different genre

Everything above is incident-based: "tell me about a time". These five are not. They ask **how you operate**, and agency interviews lean on them heavily, because they are hiring someone who will be put in front of a client.

You already have the answers. Every one of them is a file in your workspace. That is the whole point of having done the course.

---

**"How do you work on a brief?"**

*Weak:* "I read it carefully, ask questions if anything is unclear, then start wireframing."

*Strong:* "I assume the brief is out of date before I open it, because it usually is. First pass I read every version I was sent together, not one at a time, because contradictions only show up side by side. Then I pick the questions only I can answer, the ones where two readings are both defensible, and I answer them with a confidence label attached. On the last project three of my answers were guesses and I marked them as guesses. The client corrected one of them in week one instead of week four."

*Why it works:* it describes a repeatable method with a specific outcome, and the confidence labelling is unusual enough to be remembered. **Source: `brief-interrogated.md`, which is `brief-v3-interrogated.md` if you worked on EduBridge.**

---

**"Your boss changes the brief halfway through. What do you do?"**

*Weak:* "I stay flexible and adapt. Change is part of the job."

*Strong:* "I check whether it is a revision or new scope, because they get handled differently. A revision I absorb. New scope gets a sentence: happy to take that on, it is roughly this many days, that puts it outside the current sprint, want me to quote it. That is not a refusal, it is a price. Last project video calling arrived after the budget was agreed. I said yes to it and quoted it separately, and it got approved as extra."

*Why it works:* it shows you can be accommodating without being exploited, which is exactly what they are checking. **Source: `engagement.md`.**

---

**"How do you negotiate?"**

*Weak:* "I try to find a win-win and keep the relationship positive."

*Strong:* "I try to have the scope written down before a number exists, because after the number everything is a negotiation instead of a definition. When I do have to push back I bring a count rather than an opinion. On the last project the client wanted one global checkout and had conversion data supporting it. I did not argue with the data. I counted the screens their flow was missing for this market, listed the five error states nobody had specified, and let the count make the argument. And I never discount without removing scope, because that teaches the client my first number was invented."

*Why it works:* three concrete principles and a real example, and the last line signals you have been burned and learned. **Source: `engagement.md` and `critique-notes.md`.**

---

**"How do you plan a piece of work?"**

*Weak:* "I break it into phases and set milestones."

*Strong:* "I break the brief into tasks before I design anything, and then I deliberately do only one of them first. The mistake I used to make was starting the whole product at once, so nothing was finishable and everything was eighty percent done. Now the first deliverable is one screen, complete, including the empty and error states, because that is what surfaces the questions the brief did not answer. The rest gets easier once one thing is genuinely finished."

*Why it works:* it names a mistake and the correction, which reads as experience rather than theory. **Source: `/brief-to-tasks`, Class 6.**

---

**"You have an idea and you want to pitch it to your boss. How?"**

*Weak:* "I'd put together a presentation and explain the benefits."

*Strong:* "I bring the alternative with it. An idea on its own asks them to do the work of comparing, and busy people say no to that. So I show what we do now, what I am proposing, the one thing that decided it for me, and what my option gives up. The last part matters most. If I pretend there is no downside they stop believing the rest. When I moved a verification badge above the tutor's name I could point at the finding that decided it and say plainly what the old layout did better."

*Why it works:* naming the tradeoff is what separates someone with opinions from someone with judgment. **Source: `critique-notes.md`, Class 4.**

---

### How to use these five

Do not memorise the strong versions. They are somebody else's project. Take each question, open the file named under it, and write your own from what is actually in there. If a file is thin, that is the honest signal about which part of your process needs work, not a reason to invent a better answer.

**Say all five out loud once.** Written answers that fall apart when spoken are not ready, and these are longer than the STAR answers, which makes them easier to ramble.

### Three questions you ask them

Always have three ready. What you ask reveals what you care about.

About the work: "What is a design decision the team made recently that somebody internally disagreed with, and how did that get settled?"

About growth: "What does junior to senior look like here in practice? Not the titles, the actual scope change."

About AI: "How does the team use AI today, and what is something you have deliberately chosen not to use it for?"

That third one matters. A team with no position on AI is either not paying attention or has not had to think about it yet. A team with explicit limits has done the thinking.

### Things not to say

- "I am a perfectionist." Reads as evasion.
- "I am a quick learner." Everyone says it, so it carries nothing.
- "I am passionate about design." Replace it with one specific thing you did that nobody asked you to do.
- "I can do anything you need." No, and claiming it makes your real strengths less believable.
- "I use AI for everything." Say you use it. Do not suggest you need it.

### Night before, morning of

Night before: read `01-positioning.md` once. Read the AI-objection answer twice. Read the story for whichever project you will be asked about. Use their product for ten minutes if it exists. Find one thing they shipped or wrote recently and form an opinion on it.

Morning of: eat something. Say your elevator pitch out loud once. Then stop reading these notes. The structure is in your head. Go in fresh.

---

## YOUR TURN

<!-- COURSE SCAFFOLDING: delete everything above YOUR TURN once you have filled it in. This becomes your real working file. -->

Write your own answers below, grounded in the work you actually did in Class 6. Not the EduBridge example. Yours.

The test for every answer: pull out the sentence that names the decision. If you cannot find one, or if the only concrete thing in the answer is a tool name, the answer is not finished. "I used Claude Code to build the screen" is not an answer to anything. "I decided the photo goes below the fold because the page has to load on 3G" is.

Use STAR for questions 2, 3, 4 and 5. Two sentences per part, plus one line on what you learned.

When the drafts are done, open Claude Code at the root of this workspace on the latest Sonnet at medium effort. Ask it to interview you: it asks the question, you answer from memory without looking, then it tells you which decision you failed to name. Do that round three times. Fits in one session.

### 1. What do you say when someone insinuates AI did your work?

Write it in three beats: accept the question, move the frame to decisions, land one specific example. Then name three decisions from your own project that you can list inside it. Not three things Claude produced. Three calls you made and could defend.

Decision one:

Decision two:

Decision three:

Your answer:

### 2. STAR: a time you disagreed with someone who outranked you

Real disagreement, real stakes, real resolution, including if the resolution went against you. A client, a PM, a senior designer, a teacher, a group project lead. What you brought to the disagreement is the answer, not who won.

Situation:

Task:

Action:

Result:

What I learned:

### 3. STAR: a time you were wrong

One judgment call you made and regret. The decision, what it cost, how you found out, what you changed. This should be the same failure you wrote in part 5 of `02-portfolio-story.md`, said out loud instead of written.

Situation:

Task:

Action:

Result:

What I learned:

### 4. STAR: the project you are proud of

The Class 6 screen. Compress the five parts of your portfolio story into STAR shape and time yourself saying it. If you go past ninety seconds, you are describing what the screens look like. Cut back to what you decided.

Situation:

Task:

Action:

Result:

What I learned:

### 5. STAR: a time you cut scope

A second decision from the same project is fine here. Pick the moment you said no to something, or moved it out of this round, and told the client why. `engagement.md` has the material. Vary the decision, not the project.

Situation:

Task:

Action:

Result:

What I learned:

### 6. Answer the five process questions

One paragraph each, in your own words, from your own files. Open the file named under each one first.

- How do you work on a brief? (`brief-interrogated.md`, or `brief-v3-interrogated.md` on EduBridge)
- Your boss changes the brief halfway through. What do you do? (`engagement.md`)
- How do you negotiate? (`engagement.md`, `critique-notes.md`)
- How do you plan a piece of work? (`/brief-to-tasks`)
- How do you pitch an idea? (`critique-notes.md`)

Then say each one out loud once. Fix whatever falls apart when spoken.

### 7. What three questions do you ask them?

One about the work, one about how you would grow there, one about how the team handles AI. Write your actual wording, not the categories.

1.
2.
3.
