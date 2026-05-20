---
name: prd-quick-draft
description: Use this skill when the user asks to "write a quick PRD", "10-minute PRD", "fast PRD", "rough PRD", "PRD draft", "draft a PRD quickly", "PRD skeleton", or wants a fast first-pass product requirements doc to break analysis paralysis. This skill produces a tight one-page PRD from a six-blank framework in about ten minutes. For a full production-ready PRD with acceptance criteria, edge cases, failure modes, and architecture, use prd-authoring instead.
version: 1.0.0
---

# Quick PRD Draft (10-Minute Framework)

You are helping the user produce a complete first-pass PRD fast — in roughly ten minutes — to break analysis paralysis and give the team something concrete to react to. A quick draft that ships beats a perfect draft that stalls.

This is a draft, not a final spec. The bar is: clear enough that the team understands what to build and why. For the full production PRD (acceptance criteria, edge cases, success metrics, architecture), use the `prd-authoring` skill.

Core principle: a PRD exists for one reason — you want the team to build something. Keep every line in service of that.

## Step 1 — Load Context

Read `memory/user-profile.md` for product context, personas, and the user's PRD format preference. Read any feature description, notes, or links the user provided. Do not block on missing context — this is a fast draft; infer and mark assumptions.

## Step 2 — Set the Frame

Remind the user once, briefly, of the rule that makes this fast:
- Time-box it to 10 minutes. Phone away, chat and email closed, notifications muted.
- The goal is a draft to react to, not a finished artifact.

## Step 3 — Fill the Six Blanks

Produce the PRD by completing these six statements. Each should be one to three sentences — specific, concrete, no hedging:

1. **Our users have this problem:** _____ — name the persona and the situation; quantify the pain if you can.
2. **To solve it, we should do this:** _____ — the core mechanic, in plain language.
3. **Then, our users will be better off, like this:** _____ — the user-visible outcome.
4. **This is good for business, because:** _____ — the revenue, retention, cost, or strategic reason.
5. **Here's how we'll know if it worked:** _____ — one or two measurable signals.
6. **Here are other things we considered:** _____ — alternatives weighed and why this one won.

If the user's input leaves a blank unanswerable, fill it with a clearly-marked assumption (`[ASSUMPTION: ...]`) rather than stopping. At most, ask ONE clarifying question — only if the core problem is genuinely unknowable.

## Step 4 — Title It

Create a short, catchy title that names the thing being built. Place it at the top, centered, with the word **PRD** in bold right after it. Example: `Smart Reorder **PRD**`.

## Step 5 — Output

Render the PRD as a single tidy page:
- Centered bold title with **PRD**
- The six filled statements as a clean list or short sections
- Any `[ASSUMPTION: ...]` markers left visible so the team can correct them

## Step 6 — Save & Next-Step Offer

Offer to:
1. Save to `outputs/prd-[feature-name]-[date].md`
2. Hand the draft to the `prd-authoring` skill to expand into a full production PRD once the team has reacted to it.
