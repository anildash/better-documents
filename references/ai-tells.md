# AI Tells in Prose

Reference for the better-documents skill (`SKILL.md`). The visual-style
override (`references/visual-style.md`) handles how a document looks. This
handles how it reads.

Default LLM prose has recognizable tells that make professional documents read
as machine-generated. In **generate** mode, avoid these. In **review** modes,
flag them. In **rewrite** mode, check for them alongside the five passes and
fix them in the revision.

| Tell | Example | Fix |
|---|---|---|
| Contrast reveal | "It's not a cost center, it's an investment." | State the point directly: "This is an investment, and here is why." |
| Negation list | "No meetings, no templates, no waiting." | Say what does happen; keep at most one negation if it carries meaning. |
| Self-answered question | "The result? 3x faster." | Delete the question; keep the answer as a sentence. |
| Colon reveal | "The best part: it learns." | Write a normal sentence. |
| Stock opener | "In today's fast-paced world…" / "Here's the thing:" | Cut it; open with the reader's problem or the fact. |
| Trailing pile-on | "…faster reporting, no exports, no spreadsheets, ensuring nothing slips." | End the sentence at the claim; give the benefit its own sentence. |
| Em-dash abuse | More than one em-dash per paragraph in a formal document | Use a period or comma; reserve the em-dash for one deliberate pause. |
| Placeholder adjectives | "robust," "seamless," "powerful," "leverage" | Replace with the fact it stands in for: the number, the step, the outcome. |

## Do not flag

- A genuine list of three when there really are three items
- A single "No credit card required"-style negation next to a call to action
- Questions in a FAQ
