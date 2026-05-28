---
name: better-documents
description: >
  Apply communication best practices when generating or reviewing any document,
  presentation, report, memo, slide deck, proposal, or email. Use this skill when
  asked to write, create, draft, or generate a document or presentation — apply
  the principles at generation time, not as an afterthought. Also use when asked
  to "review my doc," "look at this deck," "does this make sense," "is this clear,"
  "improve this proposal," "check this before I send it," "make this more effective,"
  or any request to evaluate whether a document will land with its audience. Use
  this skill even when the request seems minor — a "quick look" or a "short memo"
  is exactly when these principles matter most.
---

# Document Review

Apply communication best practices when generating or reviewing any business
document — whether the right message reaches the right audience in the right order.

This skill applies the principles from Anil Dash's [Make better documents](https://www.anildash.com/2024/03/10/make-better-documents/).

## Scope

This skill covers **business documents**: presentations, slide decks, proposals,
reports, memos, briefs, one-pagers, and emails. It does not cover UI, web
components, or frontend applications — use the `frontend-design` skill for those.

The design principles here differ from frontend design in important ways:

- **Restraint over expression.** UI benefits from bold aesthetic commitment and
  distinctive visual personality. Business documents benefit from getting out of
  the way of the content. Most people reading a board deck or a client proposal
  are not there to appreciate the typography.
- **The audience can't interact.** A web interface rewards exploration. A
  document gets one read, often skimmed, often on a small screen or printed.
  Every design choice that draws attention to itself is attention stolen from
  the message.
- **Non-designers are both authors and audiences.** UI is built and consumed
  with design context nearby. Business documents are built by operators, analysts,
  executives, and founders — and read by the same. Complexity that a designer
  handles intuitively becomes noise for everyone else.

## Modes

| Mode | When to use | What you do |
|---|---|---|
| **generate** | "write me a proposal," "create a deck," "draft a memo" | Apply all five principles while producing the document; no separate report needed |
| **full-review** | "review this doc," "look at this deck" | Run all five passes on an existing document, produce a structured report |
| **rewrite** | "fix this," "make this better" | Apply all passes and return a revised version |
| **targeted** | "is the ask clear," "check the formatting" | Run only the relevant pass(es) |
| **quick** | "quick look," "does this work" | Run passes 1 and 2 only, flag the top 3 issues |

Default to **generate** when producing a new document from scratch. Default to
**full-review** when given an existing document with no other instruction.

---

## The Five Passes

Apply these in order. Each targets a different failure mode.

### Pass 1 — Audience and Purpose

The most common reason documents fail: they were written for the author, not the reader.

Check for:

- **Missing context**: Does the document assume knowledge the audience may not have?
  Flag any jargon, backstory, or acronyms that aren't explained.
- **Buried ask**: Is there a request, decision, or action needed? If so, is it
  stated clearly in the first third of the document — not saved for the end?
- **Author-centered opening**: Does the document open with the author's anxieties,
  backstory, or credentials rather than shared context? Flag and suggest reordering
  to start from common ground.
- **Missing deadline or stakes**: If a decision or response is needed, is the
  timeline stated? Is the reason for that timeline explained from the *audience's*
  perspective, not just the author's?

Severity guide:
- **CRITICAL** — The core ask or decision is absent or appears only at the end
- **MAJOR** — The audience is unclear; the document would read differently to
  different readers
- **MINOR** — Context gaps that could be filled with a sentence

---

### Pass 2 — Structure and Sequencing

Order signals importance. Audiences assume the first thing is the most important.
If it isn't, they'll be confused or dismissive before they reach the part that matters.

Check for:

- **Creation-order sequencing**: Is the document structured in the order it was
  *written* (background → analysis → conclusion) rather than the order the
  audience needs (conclusion → supporting logic → call to action)?
- **Murder mystery structure**: Does the document build to a reveal rather than
  stating the point upfront? Flag any document where the key conclusion or request
  appears in the second half.
- **Unannounced ordering**: If the document is ordered chronologically, by category,
  or by any logic other than importance, is that explicitly stated? If not, the
  audience will hunt for meaning in the sequence.
- **Key information in the wrong channel**: Is anything critical only in speaker
  notes, appendices, or footnotes? Central points belong in the main body.

Severity guide:
- **CRITICAL** — The document's conclusion or core request is in the second half
- **MAJOR** — Ordering is non-obvious and unexplained
- **MINOR** — Supporting points could be reordered for better flow

---

### Pass 3 — Formatting Restraint

Over-formatting is the most visible symptom of unclear thinking. When everything
is emphasized, nothing is.

Check for:

- **Emphasis overload**: Are bold, italic, underline, and color being combined
  on the same text? Flag any instance of two or more emphasis types on a single
  element.
- **Underlines on non-links**: Flag every underline that isn't a hyperlink.
  Underlines exist to signal clickability; using them decoratively confuses readers.
- **Color proliferation**: Count distinct colors in use (excluding images). More
  than two is almost always a problem. More than three is always a problem.
- **Border clutter**: Flag tables and sections with heavy borders. White space
  separates content more clearly than lines.
- **Filler visuals**: Flag images, icons, or clip art that aren't specific to
  the content's message. A blank space is better than a stock photo.
- **Formatting inconsistency**: Do headings, titles, or labels vary in size,
  weight, or color across the document without clear reason? Flag inconsistencies
  that will read as meaningful to an audience even if they weren't intentional.

Severity guide:
- **CRITICAL** — Formatting inconsistencies that will be read as semantic signals
  (e.g., random font changes mid-document)
- **MAJOR** — Overuse of emphasis that makes it impossible to identify what's
  actually important
- **MINOR** — Minor decoration that adds noise without adding meaning

---

### Pass 4 — Wayfinding and Density

Audiences need to know where they are in the story, and how far they have to go.

Check for:

- **No orientation**: Is there any indication of structure — a brief outline,
  section headers, or progress markers — for documents longer than one page or
  five slides? If not, flag.
- **Unsummarized data**: Does any chart, table, or data display appear without
  a title or caption that states what it shows? Readers shouldn't have to interpret
  data cold. Flag every chart or table whose title doesn't answer "what does this show?"
- **Unanswerable questions**: Are there open-ended questions in the document
  (as headers or prompts) that can't actually be answered with a choice? Flag
  any question that could lead to a philosophical discussion instead of a decision.
  Good: "Do we go with Option A or Option B?" Bad: "How do we improve?"
- **Dense, unbroken prose**: Are there paragraphs longer than ~6 lines where
  bullet points would make the content more skimmable without losing meaning?

Severity guide:
- **CRITICAL** — Data presented without any interpretive framing
- **MAJOR** — Long documents with no structural signposts
- **MINOR** — Questions that could be made more answerable

---

### Pass 5 — Naming and Versioning

The title is information. Most document names throw it away.

Check for:

- **Generic or auto-generated title**: Does the document have a title like
  "Untitled," "Draft," "Meeting Notes," or the name of the person it's addressed
  to? Flag and suggest a title that includes: topic, date, and context/owner.
- **Recipient-first naming**: If the document is *for* someone at another
  organization, is it named after *them* rather than the author or topic?
  They'll search for it by *your* name, not theirs.
- **Version ambiguity**: Does the filename or title use `_v2`, `_final`,
  `_final_final`, or sequential numbers without dates? Flag and suggest
  date-based versioning.
- **Meeting invites named after participants**: If the document is tied to a
  meeting, flag any invite titled "Meeting with [Name]" — it tells the recipient
  nothing about what the conversation is for.

Severity guide:
- **CRITICAL** — Untitled or generic title on a document intended for external sharing
- **MAJOR** — Version ambiguity on any document with multiple drafts
- **MINOR** — Suboptimal naming that could make retrieval difficult later

---

## Output Format

### Generate mode

Produce the document applying all five principles as first-order constraints —
not as a post-hoc checklist. Specifically:

- State the conclusion or ask in the opening, not the closing
- Order content by importance to the audience, not by how it was assembled
- Use the minimum formatting necessary: one emphasis type at a time, no decorative
  underlines, no more than two colors, white space over borders
- Include structural signposts if the document is longer than one page or five slides
- Give the document a title that includes topic, date, and relevant context

**Override default visual style.** Claude's default document aesthetic — warm
cream backgrounds, serif display type (Georgia, Fraunces, Playfair), terracotta
or amber accents, and a "small all-caps label over a body copy block" slide
layout — is recognizable as AI-generated and inappropriate for most professional
contexts. Do not apply it.

Instead, before generating any document with visual styling:

1. **Ask about brand or visual constraints first.** Does the user have brand
   colors, a template, or a font they use? If so, follow those exactly.
2. **If no brand guidance is given**, default to neutral: black text on white,
   one sans-serif typeface throughout, no decorative color. The content should
   do the work, not the palette.
3. **If the user explicitly wants visual styling**, offer 2–3 distinct directions
   in one sentence each (e.g. "neutral/minimal," "bold/high-contrast," "warm/
   editorial") and let them choose before proceeding. Do not pick for them.

No review report is needed in generate mode. The principles are baked in.

---

### Full-review and targeted mode

```
## Document Review: [Title or description]

### Summary
[2–3 sentences: what the document is trying to do, how well it's set up to succeed,
the one or two changes that would most improve it]

### Pass 1 — Audience and Purpose [N issues]
[Each issue: location → what the problem is → suggested fix → severity]

### Pass 2 — Structure and Sequencing [N issues]
[Same format]

### Pass 3 — Formatting Restraint [N issues]
[Same format]

### Pass 4 — Wayfinding and Density [N issues]
[Same format]

### Pass 5 — Naming and Versioning [N issues]
[Same format]

### Top 3 Changes
[The three revisions that would most improve this document's effectiveness,
ranked by impact]
```

### Rewrite mode

Return the revised document with a brief note after explaining what was changed
in each pass and why. Do not explain every small edit — only the structural
decisions that changed meaning or order.

### Quick mode

Return only the top 3 issues found across passes 1 and 2, with a one-line
suggested fix for each. No full report.

---

## Constraints

- **Don't alter the author's voice.** In review and rewrite modes, improve
  structure and clarity, not style. If a sentence is clear and effective, leave it.
- **Don't invent content.** If information is missing (a deadline, a decision
  option, context for the audience), flag the gap — don't fill it in.
- **Ask before generating if the audience is unclear.** In generate mode, if the
  request doesn't specify who will read the document or what decision it needs to
  drive, ask before writing. A document built for the wrong audience fails
  regardless of how well it's structured.
- **Be specific.** Every finding must reference the actual text or location.
  Never say "consider clarifying" without showing where and how.
- **Respect intentional choices.** If the document is explicitly a narrative
  or a mystery-format pitch, flag the structural convention as a risk rather
  than a violation.

---

*Based on [Make better documents](https://www.anildash.com/2024/03/10/make-better-documents/) by Anil Dash.*
