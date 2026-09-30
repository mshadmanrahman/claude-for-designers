# EduBridge Bangladesh: the course project

This is the project you carry from Class 3 to Class 6. By the end it is also the folder you show someone when they ask what your design process looks like.

EduBridge is what your instructor demos on every class, because its brief has contradictions planted in it on purpose.

Whether *your* assignments run on EduBridge or on your own client was decided in Class 1, and it does not change after Class 2. A case study built half from EduBridge and half from another product is weaker than one built from either. If you chose your own client, the file structure here is identical to the one in your folder, so read this as the answer key.

## Read this first: which level do you open?

Two rules. Getting them wrong is how you end up with generic output, and last batch someone spent four weeks unsure which one to open.

1. **Root versus project.** The root of the repo holds what is true about **you**: how you work, your taste, your voice, your reusable skills. This project folder holds what is true about **this client**: their brief, their users, their constraints. The test is one question. Would it still be true on your next job? Then it goes at root.
2. **Select a Folder is a decision.** Open Claude Code at the **root** when the work spans projects: writing your working contract, building a skill. Open Claude Code at **this folder** when you are doing EduBridge work: the brief, the critique, the tokens, the screen. Opening at the wrong level gives you generic output, or context bleeding from one client into another.

So: your contract and your taste rules live at root, in `principles/`. Everything in this folder is EduBridge and only EduBridge.

## What is reference, and what is yours to fill in

Seven files in here are yours. The rest is context you read.

**Yours to fill in.** The six markdown files each carry their own instructions at the top, a filled example, and a `## YOUR TURN` section. Delete the scaffolding once your answers are in. The seventh, `my-booking-screen.html`, does not exist yet; you create it in Class 6.

If EduBridge is your project, these are your files. If you brought your own client, fill the same files in your own folder and read these for the standard.

| File | Class | What you produce |
|---|---|---|
| `context.md` | 1 | Who this client's users actually are, the device and connection they are on, and what they can afford. Everything downstream reads it |
| `claude-contract.md` | 2 | What is true about this client only: who they are, who their users are, their constraints, what they will not accept. The root `principles/claude-contract.md` is the other half, and it holds what is true about you |
| `brief-v3-interrogated.md` | 3 | Your decisions on every place the client brief and the PM thread contradict each other |
| `engagement.md` | 3 | What the job actually is: scope, what is out, revisions, who signs off. Write it before you quote a price |
| `critique-notes.md` | 4 | What was actually wrong with your first-pass screen, and what you changed |
| `tokens.md` | 5 | Your color, type, spacing, radius and motion tokens, named |
| `ia-map.md` | 6 | The journey first, then every screen named against the step it serves. `/information-architecture` writes it, and `ia-map.html` beside it is the same thing drawn |
| `tasks.md` | 6 | The build broken into tasks, each with a done-when line. `/brief-to-tasks` writes it |
| `my-booking-screen.html` | 6 | Your own booking screen, built from your brief, critique and tokens. You create this file; `booking-screen.html` beside it stays as reference |
| `build-notes.md` | 6 | Three states nobody asked for, and the brief line each one answers |

**Reference, do not edit.**

| File | What it is |
|---|---|
| `brief-v1-client.md` | The client brief as sent. Polished, confident, wrong in several places |
| `brief-v2-pm-thread.md` | The same brief as it really arrives: WhatsApp and email fragments that contradict the document in seven places |
| `context.example.md` | The instructor's filled user context for EduBridge. Open it after you have written your own, not before |
| `engagement.example.md` | The instructor's filled engagement. Open it after you have written your own, not before |
| `brief-v3-interrogated.example.md` | The instructor's fully worked interrogated brief. Open it after you have written your own, not before |
| `PRODUCT.md` | Standing product context: users, purpose, brand, design principles. Claude reads this on every task in this folder |
| `DESIGN.md` | The finished design system behind the built screen. The Class 5 answer key |
| `ia-map.example.md` | The instructor's worked IA for the booking flow. The Class 6 answer key. Open it after you have written your own |
| `ia-map.example.html` | The same IA drawn as a page. Open it in a browser to see what a gap looks like |
| `booking-screen.html` | The instructor's built screen, read-only. See below |

## `booking-screen.html`, and what Class 6 does with it

This is a real, working, single-file HTML screen: the parent-facing tutor booking request for EduBridge BD. It was built in one Claude Code session from the interrogated brief plus the tokens, and it is the shape of the thing you are working toward from Class 3 onward.

It is deliberately imperfect. The gaps are real gaps, and they are there so there is something to find.

You do not edit this file. In Class 6 you build your own version of the same screen, in a new file beside it called `my-booking-screen.html`, and then you audit that. Keeping the two files separate is what lets you diff your screen against the instructor's afterwards, and it means a bad session never destroys your reference.

Then:

1. Point Claude Code at this folder and run `/brief-to-tasks` on your `brief-v3-interrogated.md`. You get a task list, time-boxed.
2. Run `/frontend-design` with your brief, your `critique-notes.md` synthesis and your `tokens.md` in context, and have it write to `my-booking-screen.html`. That is the whole point of the previous three weeks: the quality of the screen is the quality of those three files.
3. Open `my-booking-screen.html` in a browser on a phone-width viewport and look at it. Then audit it, and fix what the audit finds.

The latest Sonnet at medium effort. Building the screen fits in one session. Building it and then auditing and fixing it needs two, so do not start the build twenty minutes before you have to leave.

Claude Code writes the HTML. You decide what the screen is for, who it is for, and whether what came back is good enough to send. Nobody who has not done Classes 3 to 5 can make those calls, which is the answer to whether this replaces you.

## Progressive disclosure: the reference repo has everything, your assignment does not

The files you write ship blank, and the worked version sits beside each one. The assignment only ever asks you to touch the current week's file, so ignore the rest until its class arrives.

Across the whole workspace:

- **Class 1**: no file. It runs in a chat window, and the repo opens in Class 2.
- **Class 2**: adds `principles/claude-contract.md` at root and `claude-contract.md` here in the project. `context.md` sits beside the project contract for this client's users. The skills already ship inside the repo, so nothing gets installed; Class 2 is just the first class that runs one (`/grill-me`).
- **Class 3**: the brief chain here, `brief-v1` to `brief-v2` to `brief-v3-interrogated.md`, plus `engagement.md` for the commercial half.
- **Class 4**: adds `critique-notes.md`.
- **Class 5**: adds `tokens.md`.
- **Class 6**: `ia-map.md` and its diagram `ia-map.html`, then `tasks.md`, then your own screen as `my-booking-screen.html`, then `build-notes.md`.
- **Class 7**: `career-vault/` opens for the first time.
- **Class 8**: the rest of `career-vault/`.

## The arc

Confused brief, interrogated brief, critique, system, built screen. Five steps, nothing handwaved, nothing missing. A reviewer can open this folder and see exactly how you think, which is worth more than a dribbble shot of the final screen.

## When you start your own project

Do not duplicate this folder. Duplicate `projects/_new-client/` instead: right-click it, Duplicate, rename the copy, or ask Claude Code to do it for you. This folder is filled in as the answer key, so copying it drags EduBridge's users, tokens and decisions into your client's folder.

Then, in your own folder, work through the same sequence. Replace `brief-v2-pm-thread.md` with your real PM thread, or delete it. Rewrite `PRODUCT.md` first, because everything downstream reads it. Then run the same sequence from interrogation to build.

The folder is the process, not just an output of it.
