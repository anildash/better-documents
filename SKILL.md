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
metadata:
  version: 1.1.0
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
| **full-review** | "review this doc," "look at this deck" | Run all five passes plus the reader test on an existing document, produce a structured report |
| **rewrite** | "fix this," "make this better" | Apply all passes, reader-test the result, return a revised version |
| **targeted** | "is the ask clear," "check the formatting" | Run only the relevant pass(es) |
| **quick** | "quick look," "does this work" | Run passes 1 and 2 only, flag the top 3 issues |

Default to **generate** when producing a new document from scratch. Default to
**full-review** when given an existing document with no other instruction.

---

## The Five Passes

Apply these in order. Each targets a different failure mode.

In review and rewrite modes, after completing each pass, briefly re-check that
the changes made in that pass did not compromise earlier passes — for example,
a reordering in Pass 2 must not reintroduce Pass 3 formatting problems. Fix any
regression before moving on.

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

If the audience is a board of directors, read `references/boardroom.md` before
reviewing or generating. It covers how board members actually read, how power
works in the room, and what the realistic goal of a board document is.

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
is emphasized, nothing is. This pass targets stacked emphasis, decorative
underlines, too many colors, heavy borders, filler visuals, and inconsistent
formatting that readers will mistake for meaning.

For the full checklist, see `references/formatting-restraint.md`.

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

## Reader Test

In full-review and rewrite modes, after the five passes, verify the document
works for its audience — not just for you, who know what the author meant.

1. **Predict reader questions.** Write 3–5 questions the audience will
   realistically ask when they read this: What are we deciding? What happens
   if we say no? What does it cost? When is the deadline?
2. **Test with a fresh reader.** If sub-agents are available, dispatch one
   with only the document content and the questions — no context from this
   conversation. If sub-agents are not available, skip this step and note in
   the report that the reader test was not run.
3. **Report failures.** Any question the fresh reader cannot answer from the
   document alone is a Pass 1 (audience) finding. Include it in the report,
   labeled "(reader test)," with the question that exposed it.

The point is to catch author blind spots: things that make sense to the person
who wrote the document but do not land on a cold read.

---

## Expert Panel

For high-stakes documents (board decks, client proposals, anything going to an
external audience), optionally assemble 3–5 expert personas relevant to the
document type — for example, a skeptical board member, a busy executive skimming
on a phone, or a first-time reader with no context. Each persona scores the
document 1–10 and gives specific critiques, not just scores.

Revise the lowest-scoring areas first, then re-score until all personas score 7+
with an average of 8+.

| Score | Meaning |
|---|---|
| 9–10 | Publish-ready; no meaningful improvements |
| 7–8 | Strong; minor tweaks only |
| 5–6 | Functional but has clear gaps; needs another pass |
| 3–4 | Significant issues; major revision needed |
| 1–2 | Fundamentally broken; rethink the approach |

**When to use:** always for high-stakes external documents, optional for internal
documents, skip in quick mode.

---

## AI Tells in Prose

Default LLM prose has recognizable tells (contrast reveals, stock openers,
placeholder adjectives, and similar) that make professional documents read as
machine-generated. In generate mode, avoid these. In review modes, flag them.

For the full list of tells, fixes, and what not to flag, see `references/ai-tells.md`.

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
- Write prose without AI tells: state points directly, no contrast reveals, no
  stock openers, no placeholder adjectives (see `references/ai-tells.md`)

**Check for a brand context file.** Before asking about brand constraints, look
for a `.better-documents/brand.md` file in the project root. If it exists, read
it and use its brand colors, fonts, and template rules. If the user provides new
brand information that differs from the file, update the file.

**Override default visual style.** Do not apply Claude's default document
aesthetic; it reads as AI-generated and is wrong for most professional contexts.
Before generating any document with visual styling, ask about brand or visual
constraints first, and default to neutral if there are none. For the full rule
and procedure, see `references/visual-style.md`.

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
[Reader-test failures go here, labeled "(reader test)"]

### Pass 2 — Structure and Sequencing [N issues]
[Same format]

### Pass 3 — Formatting Restraint [N issues]
[Same format]

### Pass 4 — Wayfinding and Density [N issues]
[Same format]

### Pass 5 — Naming and Versioning [N issues]
[Same format]

### What's Working Well
[2–3 specific things the document does right — what is clear, what is
effective, what is worth keeping. Calibrates the findings. Do not pad it.]

### Top 3 Changes
[The three revisions that would most improve this document's effectiveness,
ranked by impact]
```

### Rewrite mode

Apply all five passes and the AI-tell check, then reader-test the revised
version (if sub-agents are available) before returning it. Return the revised
document with a brief note after explaining what was changed in each pass and
why. Do not explain every small edit — only the structural decisions that
changed meaning or order.

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
