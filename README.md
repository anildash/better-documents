# document-review

A skill for Claude Code, Cursor, and any SKILL.md-compatible agent that applies communication best practices when generating or reviewing business documents.

## The problem

There's a 290K-install skill that stops Claude from making ugly websites. Nothing equivalent exists for business documents — until now.

Claude has a documented default visual style (cream backgrounds, Playfair headlines, terracotta accents) that Anthropic's own docs flag as inappropriate for most professional contexts, and note bleeds into slide decks. But the more important problem is structural: buried asks, author-centered openings, conclusions saved for the end, formatting used as a substitute for clarity. These are the patterns that make AI-generated documents feel thin even when they look fine.

The agent skills ecosystem has deep coverage of code, UI, and deployment. Business document communication is almost entirely absent. This skill fills that gap.

## What it does

Two modes:

**Generate** — fires when you ask Claude to write a deck, memo, proposal, or report. Applies five communication principles at creation time, not as an afterthought. Also overrides Claude's default visual style and asks about your brand before touching anything visual.

**Review** — fires when you ask Claude to review or improve an existing document. Runs five named passes and produces a structured report with severity levels (CRITICAL / MAJOR / MINOR) and specific suggested fixes.

### The five passes

1. **Audience and Purpose** — buried ask, author-centered opening, missing stakes
2. **Structure and Sequencing** — creation-order docs, murder mystery structure, key info in speaker notes
3. **Formatting Restraint** — emphasis overload, decorative underlines, color proliferation, filler visuals
4. **Wayfinding and Density** — no orientation, unsummarized data, unanswerable questions, dense prose
5. **Naming and Versioning** — generic titles, recipient-first naming, `_final_final`

## Install

```bash
npx skills add github:anildash/document-review
```

Or copy `SKILL.md` into your project root.

## Usage

Once installed, the skill fires automatically on relevant requests:

```
Write a proposal for migrating our analytics stack to BigQuery.
```

```
Review this deck before I send it to the board.
```

```
Quick look — does this memo make sense?
```

No extra prompting needed. The skill's description is written to trigger on generation requests ("write," "create," "draft") and review requests ("review," "look at this," "does this work").

## Scope

This skill covers **business documents**: presentations, slide decks, proposals, reports, memos, briefs, one-pagers, and emails.

It does not cover UI, web components, or frontend applications — use the [`frontend-design`](https://github.com/anthropics/anthropic-quickstarts) skill for those. Document design has different rules: restraint over expression, one read not interactive, non-designers in the loop at every stage.

## Source

Based on [Make better documents](https://www.anildash.com/2024/03/10/make-better-documents/) by Anil Dash (March 2024) — translated from advice for human authors into instructions an AI agent can follow.

## Files

- `SKILL.md` — the skill itself
- `document-design.md` — the source guidelines in distilled form, useful as standalone reference
- `BLOG-NOTES.md` — notes on the thinking behind this skill
