---
created: 2026-07-27
type: reference
status: template
tags: [edubridge, class-5, workbook, design-tokens]
project: EduBridge Bangladesh
---

# EduBridge BD: Design Tokens

**What this file is for:** the named values your design is made of, written once so you stop retyping hex codes into every prompt and every Figma layer.

**Why Claude needs it:** without it, "use a nice green" produces a different green every session. With it, Claude writes `#00A651` because you told it what `accent.primary` means, and your Figma variables and your built screen finally agree.

**Which class:** Class 5. Class 6 pastes this file into the prompt that builds the screen.

<!--
COURSE NOTE for the student. This is not an instruction to Claude.

Everything between here and `## YOUR TURN` is teaching material. Delete it once your own answers are in.
-->

## How you produce it

You write the set first, and the skill checks it afterwards. That order is deliberate: a token
you did not choose is a token you cannot defend when a developer asks why it exists.

1. List the raw values you actually used on your Class 4 screen. Colours, type sizes, spacing, radii, motion. Do not name them yet.
2. Give each value a role. Rename it by what it does, so a developer knows when to reach for it without seeing the colour.
3. Write them into the tables below, with the use for each one. Delete any row you cannot fill.
4. Apply the same names in Figma as variables, exactly, character for character.
5. Run `/design-tokens` last, as a check. Ask it to compare your file against your frame. Treat the result as a diagnostic, not an answer key.

The names are the contract. Values change all the way to launch; names should not.

## Example: the token set behind `booking-screen.html`

Labelled as the example. This is the real system behind the Class 6 screen, written up in full in `DESIGN.md`. It is deliberately small: eleven colors, five type steps, one accent that means one thing.

**Color.** `navy-ink` #0A2540 (header, avatar, headlines, price). `confirm-green` #00A651 (verified badge, input focus, primary CTA, and nothing else). `confirm-green-pressed` #007A3D (CTA `:active` only). `bkash-pink` #E2136E (used exactly once, as the payment-method prefix). `screen-surface` #FFFFFF. `page-surround` #F3F4F6. `border-default` #E5E7EB. `text-tertiary` #374151. `text-secondary` #6B7280. `text-muted` #9CA3AF. `placeholder` #D1D5DB.

**Type.** System stack, no webfont, because it renders instantly on 3G with no font-loading flash and it looks like the parent's own phone. `display` 22px/700 (the session price, the number being decided on). `headline` 18px/700 (tutor name). `title` 17px/600 (header title, CTA label). `body` 15px/400 (detail rows). `label` 12px/600, 0.05em tracking (section labels, verified badge). Inputs sit at 16px on purpose, larger than body, because anything smaller makes iOS zoom on focus.

**Spacing.** `xs` 8px, `sm` 12px, `md` 16px, `lg` 20px. Multiples of four, nothing off the scale.

**Radius.** `sm` 8px (inputs), `md` 12px (buttons), `full` 100px (the verified pill).

**Motion.** Nothing over 220ms, and the CTA press feedback is 80ms. On a slow device a long transition reads as a hang, not as polish.

**The named rule.** The One Confirm Color Rule. Green appears in exactly three places: the verified badge, the input focus ring, the CTA. If a new element wants to stand out, it does not get a new color. It earns green only if it means the same thing, trust confirmed or action ready. That rule is why the badge still means something on the fourth screen.

---

## YOUR TURN

Answer each question in place. Fill the tables with your own values, from your own critique.

### Color

***Which colors does your screen actually need, and what does each one mean? Give every token a use, and delete any row you cannot fill in. Keep the names; change the values.***

| Token | Value | Use for |
|---|---|---|
| `--surface` |  |  |
| `--surface-inverse` |  |  |
| `--text-primary` |  |  |
| `--text-secondary` |  |  |
| `--text-muted` |  |  |
| `--action` |  |  |
| `--destructive` |  |  |
| `--border` |  |  |

### Type

***Which font family, and which five steps? For each step, what is the one thing on screen that uses it? A step with no user is not a step.***

| Token | Size | Weight | Line height | Use for |
|---|---|---|---|---|
| `--text-display` |  |  |  |  |
| `--text-heading` |  |  |  |  |
| `--text-body` |  |  |  |  |
| `--text-body-small` |  |  |  |  |
| `--text-label` |  |  |  |  |

### Spacing and radius

***What is your base unit, and what is the full scale? Then your radius set. If a value in your Figma file is not on this scale, either the value is wrong or the scale is.***

| Token | Value |
|---|---|
| `--space-1` |  |
| `--space-2` |  |
| `--space-3` |  |
| `--space-4` |  |
| `--space-6` |  |
| `--space-8` |  |
| `--radius-sm` |  |
| `--radius-md` |  |
| `--radius-full` |  |

### Motion

***What are your three durations, and what is your ceiling? Justify the ceiling against the device your user is actually holding.***

| Token | Duration | Easing | Use for |
|---|---|---|---|
| `--motion-fast` |  |  |  |
| `--motion-default` |  |  |  |
| `--motion-slow` |  |  |  |

### The one rule your system has to enforce

***Write the single rule that keeps this system honest, in the shape "X appears only when it means Y." Name it. A rule with a name gets followed; a preference gets argued with.***

<!-- COURSE SCAFFOLDING: delete everything above YOUR TURN once you have filled it in. This becomes your real working file. -->
