# Skills

One file per slash command. Seven of them are Julian Oczkowski's design sequence, run in order. Two are extra critique passes. One is `/stuck`, which you run when your setup breaks rather than when the work moves forward.

Every class from Class 2 to Class 6 runs one or two of them. If you skip a step, the next step does that step's work badly.

## The seven, in sequence order

| Step | Command | What it does | Class | Where the output goes |
|---|---|---|---|---|
| 1 | `/grill-me` | Interrogates you until the brief has no soft spots left. | 2 | `principles/claude-contract.md` (C2), then `projects/<yours>/brief-v3-interrogated.md` (C3) |
| 2 | `/design-brief` | Turns the interrogation into one source of truth for the project. | 3 | `projects/<yours>/brief-v3-interrogated.md` |
| 3 | `/information-architecture` | The journey first, then every screen named against the step it serves, plus navigation and hierarchy. | 6 | Two files, both written for you: `projects/<yours>/ia-map.md` is the deliverable, `ia-map.html` beside it is the diagram |
| 4 | `/design-tokens` | Fixes color, type, spacing, radius and motion as named tokens. | 5 | `projects/<yours>/tokens.md` |
| 5 | `/brief-to-tasks` | Breaks the brief into tasks, each with a "done when" line. | 6 | `projects/<yours>/tasks.md` |
| 6 | `/frontend-design` | Builds the screen from the brief and the tokens, not from a guess. | 6 | `projects/<yours>/my-booking-screen.html` (never `booking-screen.html`, that one is read-only reference) |
| 7 | `/design-review` | Reviews the screen on layout, accessibility, responsiveness, dark mode, edge cases. | 4 | `projects/<yours>/critique-notes.md` |

## The two extras

| Command | What it does | Class | Where the output goes |
|---|---|---|---|
| `/heuristic-evaluation` | Audits against Nielsen's ten heuristics, evidence and a fix per finding. | 4 | `projects/<yours>/critique-notes.md` |
| `/persona-acid-test` | Reads the work three times: confused user, skeptical engineer, impatient PM. | 3 | `projects/<yours>/brief-v3-interrogated.md` (C3), then `critique-notes.md` when you rerun it on the built screen |

## The repair command

| Command | What it does | Class | Where the output goes |
|---|---|---|---|
| `/stuck` | Reads your folder, works out what is broken, and names one thing to fix. | any | No file. It answers in the session. |

Type `/stuck` on its own. Do not explain the problem, do not paste an error, do not say which step you are on. Claude looks at your folder, tells you which class it thinks you are on and which files are still blank, then names one blocker and one fix. When it fixes nothing, it writes the group-chat message for you so the ask is one line somebody can answer.

Use it at eleven at night when you are stuck on setup and the chat is quiet. It reaches the common faults: Claude Code opened one folder too deep, `.claude/skills/` missing so no command appears, work going into an `.example.md` answer key by mistake, a skill run before the files it reads were filled, and a hunt for a file that no skill ever creates.

### Why the class order is not the step order

Steps 1 to 7 are the order you run these on a real project, start to finish. The course order differs in one place: `/design-review` and `/heuristic-evaluation` arrive in Class 4, before information architecture and tokens in Class 5.

That is deliberate. Class 4 is where you learn to critique, using a throwaway screen generated from the confused brief. Critique is the skill everything after it depends on. No skill repeats the pass in Class 6, but the judgment does: you read the screen you actually ship the same way, this time with nobody prompting you.

## Where the output goes, and why that column matters most

**Most skills do not create a file.** They produce text in your session, and you paste that text into the file for that class. The tables above tell you which file.

Two of them are exceptions.

`/grill-me` in Class 2, run on a `claude-contract.md`. That run edits the contract in place, line by line, as you answer. Nothing to paste, and nothing new appears in the folder.

`/information-architecture` in Class 6 writes two files, and both are new. `ia-map.md` holds the four parts as text, and that is the file you hand in. `ia-map.html` beside it is the same mapping drawn, so the gaps are visible instead of buried in two bullet lists. Open the page in your browser and check it before you show it to anyone.

There is no `design-brief.md`. There is no `ia.md`, no `review.md`, no `grill-me-output.md`. Class 6 is the only class where a skill creates files from nothing, and it creates exactly three: `ia-map.md`, `ia-map.html` and `tasks.md`. Everywhere else the output goes into a file that already exists in your project folder, waiting for it. In the last batch a student ran `/grill-me`, got a clean Requirements Handshake, and then sat for hours asking the group chat whether it had become a new file. It had not.

Two rules on pasting:

- Paste the whole output, not a summary. The open questions and the assumptions sections are the parts the next skill reads.
- Keep the labels the skill gave you. `/grill-me` on a brief labels its output Requirements Handshake. `/design-review` labels its verdicts Pass, Needs work, Fail. Those labels are how Claude finds the right section next week. (Contract mode has no label to keep, because it writes into your headings directly.)

One more, from the two file-location rules: output about **you** goes at root, output about **the client** goes in the project folder. That is why `/grill-me` in Class 2 lands in `principles/claude-contract.md` and the same skill in Class 3 lands in the project.

## Installing these

You install them in Class 2, because Class 2 is the first class that runs one (`/grill-me`). Follow the install steps in the [top-level README](../README.md). After that, the slash command is all you type.

If the install has not worked yet, you are not blocked. Open the skill file, copy the whole thing into your Claude Code session, then name the file you want it run against. Same text, same behaviour. Bring the broken install to the class or the office hour.

Model: Sonnet 5 at medium effort, for every one of them. Each skill fits in one Claude session. Class 6 is the exception: `/brief-to-tasks` and then `/frontend-design` needs two sessions, because the build session has to hold your tokens file the whole way through.

## Running /grill-me without drowning

In the last batch a student answered roughly thirty questions from `/grill-me` and wrote in the group chat that he was dying. He was right to stop. That is a scoping failure, not a stamina problem, and you fix it in the invocation, not halfway through.

Cap it before you start. Paste this line right after the skill text:

> Four groups. Maximum three questions per group. One group at a time. After group four, stop asking and write the Requirements Handshake.

Twelve questions. Not thirty.

**That cap is for a brief, in Class 3 and later. Do not paste it in Class 2.** Run on a `claude-contract.md`, `/grill-me` asks one question at a time, hands you a suggested answer with each one, and rewrites the line you are looking at. Capping it into four groups puts brief mode back and you lose the rewrite.

Three rules that keep it moving once it starts:

1. **"I do not know. Assume X and move on" is a legitimate answer.** It is not a failure and it stalls nothing. It goes into the Assumptions being carried forward section of the handshake, which is exactly what that section exists for. An unknown you wrote down is worth more to the next step than a guess you dressed up as a fact.
2. **One line per answer.** No paragraphs. Claude expands whatever you give it, so long answers buy you longer follow-ups.
3. **Push back when it repeats itself.** "Answered in group one. Move on." It will.

Set a timer for twenty minutes. When it goes off: "Time is up. Write the handshake with what we have. Everything unanswered goes in open questions." A handshake with six open questions in it is a working document you can take to a client. Thirty answered questions you resented is not.

## How these pair with principles/

Skills are verbs. Principles are constraints. Every skill here assumes the files in `../principles/` are loaded. That is how Claude knows your voice, your taste rules, and the market you design for.

If a skill's output feels generic, the principles are probably not being read. Check the level you opened Claude Code at: the project folder for client work, the root for anything about how you work.

## Modifying skills

These are starting points. Tune them as you do real work. Edit the .md files directly; changes take effect in your next conversation.

Common edits:

- Add a project-specific question to `grill-me.md` if the same kind of brief keeps landing on you.
- Change the review dimensions in `design-review.md` if your domain has its own failure modes (medical, legal, financial).
- Rename the tokens in `design-tokens.md` to match what your developer already uses.
