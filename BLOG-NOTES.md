# Blog post notes: promoting the better-documents skill

## The key insight / lede

There is **no Anthropic guidance anywhere** — not in system prompts, not in
the skills library, not in the cookbook, not in the prompting docs — that covers
the design of business documents Claude generates on behalf of users.

The `frontend-design` skill (293K+ installs, #2 on skills.sh) exists specifically
to stop Claude from producing "AI slop" UIs. It is explicitly scoped to web
components and applications.

Nobody has done this for documents.

Claude Opus 4.7 has a documented default house style — cream backgrounds, serif
display type, terracotta accents — that Anthropic's own docs note "appears in
slide decks as well as web UIs" and "will feel off for dashboards, dev tools,
fintech, healthcare, or enterprise apps." The recommended fix in Anthropic's
docs is to specify a concrete alternative or ask the model to propose options.
This skill does both, automatically.

So: there is a 293K-install skill that stops Claude from making ugly websites.
There is nothing that stops Claude from making ugly (or just eerily identical)
board decks, client proposals, and status reports. Until now.

---

## Angles / framings to explore

**The symmetry angle**
The `frontend-design` skill for devs, the `better-documents` skill for everyone
else. Devs already know to install skills for this kind of thing. Business users
don't. This is the version that reaches them — via LinkedIn, not GitHub.

**The "you can already tell" angle**
People are starting to recognize Claude-generated documents the same way they
recognize AI-generated images. The cream background, the Playfair headline, the
tiny all-caps kicker above the body copy block. It's a tell. This skill fixes
the tell — but more importantly, it fixes the underlying communication problems
that make AI-generated documents feel thin even when they look fine.

**The original post angle**
Link back to "Make better documents" (March 2024) as the source material — now
translated into something a coding agent can actually act on. The post was about
human authors; the skill is about AI authors. Same principles, different actor.

**The gap-in-the-ecosystem angle**
The agent skills ecosystem is massive and growing fast — 90K+ skills on
skills.sh, official repos from Vercel, Anthropic, Microsoft, Stripe. It has
deep coverage of code, UI, deployment, marketing copy. Business document
communication is almost entirely absent. The only adjacent things are
`sciwrite` (academic manuscripts) and some marketing copy skills. Nothing for
the documents most knowledge workers produce every day.

---

## Key points to make in the post

1. The skills ecosystem solves a real problem — you no longer have to re-explain
   your preferences to your AI every session. But the catalog reflects what
   developers built, not what knowledge workers need.

2. Business document design has different rules from UI design. Restraint beats
   expression. The audience can't interact. Non-designers are in the loop at
   every stage. These aren't obvious things and Claude doesn't know them by
   default.

3. Anthropic's own docs document the Opus 4.7 default style as a known problem
   for non-editorial, non-hospitality contexts — and note it shows up in slide
   decks. No skill addresses this for documents.

4. The skill doesn't just fix aesthetics. The communication principles (audience
   first, conclusion up top, no murder mysteries, answerable questions) are the
   more important half. The visual stuff is just the most visible symptom.

5. This is installable in one command and works across Claude Code, Cursor,
   Codex, and every other SKILL.md-compatible agent.

---

## Distribution notes

- Primary channel: LinkedIn (business productivity audience, not devs)
- Secondary: link from the original "Make better documents" post
- Potential: mention in a Claude.ai conversation or project instructions for
  people who don't use Claude Code
- The skill itself should link back to the blog post; the blog post should
  link to the GitHub repo and the original 2024 post

---

## Things to verify before publishing

- [ ] Test the skill against a few real document generation prompts to confirm
      the visual style override actually fires
- [ ] Check whether skills.sh has a "business documents" or "productivity"
      category to file under
- [ ] Confirm the `npx skills add` install command path once the repo is live
- [ ] Decide whether to publish under anildash.com GitHub or a new repo
