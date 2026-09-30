---
created: 2026-07-27
type: reference
status: complete
class: 4
tags: [ostad, batch-02, workbook, principles, design-taste, student-editable]
---

# Design Taste

**What this file is for:** your taste, written down, so it applies to every screen instead of only the ones you are awake enough to catch.

**Why Claude needs it:** Claude will execute anything you ask. With nothing in the folder that says what good means, it falls back to the average of every screen on the internet, and the average is generic.

**Which class:** Class 4, Claude as Critic. It runs alongside `anti-ai-slop.md` and the `/design-review` skill.

**If Sonnet keeps handing you design you would not ship, this is the file that fixes it.** Not a bigger model. This file filled in, plus `anti-ai-slop.md`, plus `/design-review` run on the output. The latest Sonnet at medium effort produces work at the level of the taste you gave it. An empty taste file is the whole explanation.

<!--
COURSE NOTE for the student. This is not an instruction to Claude.

Everything under the EXAMPLE heading is the instructor's version. It is what a filled taste file looks like for BD-focused product work. Read it for shape and for how specific each principle gets, then write your own in YOUR TURN.

A principle that could apply to any designer anywhere is not taste. It is a platitude. Yours should be arguable.
-->

---

## EXAMPLE: the instructor's filled taste file (BD product work)

<!-- Read it, then replace it with your own answers from YOUR TURN. -->

### Hierarchy before decoration

Every screen has one thing the user is supposed to do. Before any color, type, or spacing decision, name that thing. The rest of the screen exists to make that one thing obvious.

A signal you got this right: if you cover everything except the primary action, the user knows where to click. If you have to squint at the screen to find the CTA, the hierarchy failed regardless of how pretty the buttons are.

When Claude generates a screen with five "important" cards of equal weight, that is a hierarchy failure. Push back: "Which of these is the actual decision the user is making? Make that one obviously primary, demote the rest."

### Restraint is the discipline most juniors skip

The temptation is to fill the canvas. Borders, shadows, gradients, icons, decorative shapes, three call-outs where one would do. Restraint is removing one of those until the screen stops fighting itself.

Test: after Claude generates a screen, ask "what could I remove without losing meaning?" If the answer is "nothing," the screen is over-designed and Claude has not pushed back hard enough. Half the time, removing the gradient or the third icon makes the work look more expensive, not less.

The mature instinct: when in doubt, leave it out. You can always add later. Removing is harder once the client has seen it.

### Type discipline beats type variety

Three weights of one well-chosen typeface beats five weights of three trendy ones. Pick a stack, stick to it, vary by size and weight, not family.

For BD work specifically: your stack must render Bangla and English in the same hierarchy. Most Latin-first fonts fall apart in Bangla. Check Noto Sans Bengali or SolaimanLipi as fallbacks. Do not let Claude propose a type stack without confirming it has working Bangla coverage.

What looks like type variety in good work is actually scale variety: 12, 14, 16, 20, 32. Same font, different sizes, ruthless about the gaps between them.

### Color discipline: tokens, not vibes

Define your palette as tokens with names that describe role, not appearance:

- `bg.surface`, `bg.subtle`, `bg.inverse`
- `text.primary`, `text.secondary`, `text.muted`
- `border.default`, `border.strong`
- `accent.primary`, `accent.danger`, `accent.success`

When you ask Claude for a screen, give it the tokens, not "use a blue and yellow." Tokens mean the same color shows up in the right places across screens. Vibes mean every screen invents its own palette and the product looks like five products.

For BD trust contexts: green carries trust because of bKash. Use it deliberately. Random green for "make it feel friendly" is not deliberate.

### Motion budget

Animations under 150ms feel responsive. Animations over 300ms feel laggy on common BD devices, even when they render smoothly on your MacBook. There is no middle ground that works for both.

Default: 150ms ease-out for everything except critical feedback (button press, error appear). Critical feedback can be 80-100ms. Decorative motion (hero wipes, scroll reveals) does not belong on a Slow 3G product at all.

When Claude proposes "a smooth 400ms fade," push back. Ask for the same effect in 150ms or none at all.

### What "professional" actually means in design

Junior designers chase "professional" by adding shadows, gradients, glass effects, and tiny serifs in headers. Senior designers chase "professional" by removing decisions until the work cannot be misread.

Heuristic: if you handed your screen to a senior designer with their phone on Slow 3G, what is the first thing they would change? Make that change yourself before you ship. Claude will not catch it. Your taste has to.

### When to override these principles

Principles are heuristics, not rules. If the work calls for breaking one of them, break it consciously, not accidentally.

Conscious break: "I am using a 400ms transition here because the user is mid-payment and a slower confirmation reduces anxiety. This is worth the cost on 3G."

Accidental break: Claude added a 400ms transition because the default was 400ms and you did not notice.

The difference is whether you can defend the choice. That defensibility is the taste you are building.

---

## YOUR TURN

<!-- Answer each question in the space under it. Work from a real screen Claude generated for you, not from memory. Every answer here is one fewer bad screen you have to reject later. -->

**1. Open the last screen Claude generated for you. Name the one thing the user is supposed to do on it.** If you cannot name it, write the sentence you should have sent back instead of accepting the screen.


**2. What do you delete on sight?** Name three decorations you now remove without discussing them: the gradient, the third icon, the fifth equal-weight card, whatever yours are.


**3. Write your type stack and your scale.** Exact font names, exact sizes, and a line confirming Bangla coverage. Leave this blank and Claude will invent a stack for you every single time.


**4. Write your motion budget as one number,** plus the single exception you allow and why it is worth the cost on a slow connection.


**5. Name the senior designer whose judgment you trust.** What is the first thing they would change about your last screen? Write it as a rule so Claude applies it before you have to notice it.


<!-- COURSE SCAFFOLDING: delete everything above YOUR TURN once you have filled it in. This becomes your real working file. -->
