# principles/

This folder holds what is true about **you**: how you work, your taste, what you refuse to ship, and who you design for by default. Three files. Claude reads all of them before it does anything substantive in this workspace.

This is the root layer. Nothing in here is about a client. If a fact would still be true on your next job, it belongs in this folder. If it is only true for this client, it belongs in `projects/{client}/` instead.

## The three files and when you fill them in

| File | Class | What it holds | You bring back |
|---|---|---|---|
| `claude-contract.md` | 2 | How you work, how Claude talks to you, what you will not delegate, and your defaults when a brief says nothing | Your contract, at root and in the project |
| `design-taste.md` | 4 | What good means to you, specifically enough to be arguable | Filled taste file, used by `/design-review` |
| `anti-ai-slop.md` | 4 | What you refuse to ship, and the fix for each pattern | Filled slop list, plus `critique-notes.md` in the project |

Class 1 adds no file here. It runs entirely in the chat window: the same prompt twice, once cold and once with six lines of context, and you compare the two. The repo opens in Class 2.

Classes 3, 5 and 6 do not add files here either. They work inside `projects/edubridge/`, using these three as the layer underneath.

## How each file is built

Every file in this folder ships as a workbook. Same shape each time:

1. What the file is for, one line.
2. Why Claude needs it, one line.
3. Which class it belongs to.
4. A filled example, under an `EXAMPLE` heading, written for the EduBridge project.
5. A `## YOUR TURN` section with the questions you answer in place.
6. A closing `COURSE SCAFFOLDING` comment telling you when to delete the rest.

Once your answers are in, delete everything above `YOUR TURN`. The scaffolding exists to get you started; leaving it in means Claude reads course furniture as if it were your working instructions. A contract file cluttered with exercise text is a weaker contract file.

## Why this folder matters more than the rest

These files are the difference between output you can ship and output that reads as generic AI work. That is not a motivational claim, it is the mechanism: Claude has no memory of you between sessions, so whatever is not written here gets replaced by an average drawn from everything it has seen. The average is generic by construction.

The two Class 4 files carry the most weight. If Sonnet keeps producing design you would not show a client, an empty `design-taste.md` and an empty `anti-ai-slop.md` are the reason, and filling them in is the fix. The latest Sonnet at medium effort works at the level of the taste you hand it.

## The contract lives in two places

`claude-contract.md` is the one file that gets copied. The root copy in this folder is the original, the one you keep refining. The copy inside `projects/{client}/` is the one Claude reads while you are doing that client's work, because Claude Code reads from the folder you opened.

Everything else in this folder stays at root only.
