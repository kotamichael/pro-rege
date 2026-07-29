# Pro-Rege Project — Claude Code Context

This file is loaded automatically at the start of every Claude Code session in this repo. Keep it current — when the real style guide and bibliography exist, this file should be trimmed down to point at them rather than duplicating them.

## What this project is

**Primarily constructive, not polemical.** This project reconstructs and states clearly the classical Reformed orthodox position on natural and moral law, philosophy, epistemology, and apologetics — and how they properly relate to special revelation — across the whole of a Christian's life, so believers can recalibrate their foundations with a clear view of how special revelation bears on every area of life, not just a compartmentalized "spiritual" sphere. The vehicle for that reconstruction is a strict-1646-Westminster-Standards account of the covenant of works and the covenant of grace across both Testaments — moral law, natural law, and grace under each administration.

Historical debates (the antinomian and neonomian controversies, the Owen/Ball/Petto/Cameron dispute over Sinai, the Marrow Controversy) are read closely because they are where the historic consensus got forced into precision, not as ammunition-hunting. Contemporary departures — Klinean republication and its political-theological descendants (VanDrunen, R2K) — are engaged for the same reason: a live pressure-test that clarifies the constructive account, not the project's actual reason for existing. Keep this ordering straight in every article and every reading note: state the positive doctrine on its own terms first; bring in the debate because it clarifies, not because defeating it is the point.

See `00-foundations/manifesto.md` for the full statement.

## Current state of foundational docs — check before assuming any of this is final

- `00-foundations/manifesto.md` — **drafted, in progress, updated through 2026-07-29.** Purpose, Thesis, confessional anchor, historical method (Vos as a confirmed middle term between Owen and Kline), scope, non-goals, and a "Relation to Existing Treatments" section are all in place — the latter now covers six distinct contemporary angles (Myers/Belcher/McGraw, Wolfe, Garris, and Marino/Tomes as living voices running genuinely parallel arguments, credited for convergence rather than treated as competition). The natural-law/natural-theology/political-theology synthesis in `research/natural-law-synthesis-reading-map.md` is still deliberately not folded into the manifesto's main argument — the project owner is reading his way to it, and that reading map has grown substantially: a real internal Reformed fork in Strand 3 (Gillespie/Gib vs. Symington on whether Christ's civil authority is mediatorial or general/essential — see the reading map for the working answer), a sharpened natural-law hypothesis (universal operation vs. autonomous/neutral authority — two claims that were being run together as one), a new Clark-Van Til analogy/univocity subsection in Strand 4, and real academic secondary literature (Muller, Seung-Joo Lee on Junius) that was previously absent entirely.
- `00-foundations/outline.md` — draft skeleton exists in the project TODO; not yet finalized as its own file
- `00-foundations/bibliography.md` — **not yet drafted, and this is now a real gap given how much verified bibliographic material exists.** Two full audit rounds (2026-07-28/29) resolved nearly all of the previously-unverified TODO list and added substantial new academic literature — full detail in `research/contemporary-interlocutors-map.md` (the actual raw material this file should draw from) and the `contemporary_author_audit`/`project_constructive_purpose` memories. This is now closer to a "consolidate what already exists" task than a research task.
- `00-foundations/style-guide.md` — **not yet drafted** — see provisional rules below

## How the project owner wants to work

The project owner wants to do the primary theological reading and reasoning himself — Claude Code's job is scaffolding (reading maps, source location, summarizing, structuring, light drafting when explicitly asked), not authoring the constructive theological argument. Current production workflow: read a primary source → write a short micro-article reading note in `research/reading-notes/<strand>/` (template: `research/reading-notes/_template.md`) → once a strand has enough notes to show a pattern, synthesize → graduate mature material into a full `series-*` article through the six-lane pipeline below. Keep output visible at every stage rather than banking everything on one long reading project before anything gets written.

## Provisional house rules (supersede with `style-guide.md` once it exists)

- **Scripture quotation:** KJV by default, matching usage throughout the project's founding conversation. Confirm with the project owner before treating this as locked.
- **Confessional citation:** always cite the **1646** Westminster Confession / Larger Catechism / Shorter Catechism wording specifically. Where later American revisions differ (WCF 23 on the civil magistrate is the main case), state the difference explicitly rather than silently using the revised text.
- **Uncertainty discipline:** never assert a specific claim about a named living or recent author's published position without a verifiable source. If a claim can't be confirmed, say so plainly in the draft (e.g., an inline `[VERIFY: ...]` marker) rather than smoothing it into confident prose.
- **17th-century primary sources:** preserve original spelling/orthography in direct quotation (e.g., "stedfastly," "shew"); modernize only in paraphrase, and mark paraphrase as paraphrase.
- **Living authors** (Wolfe, Garris, Marino, Tomes, Beers, Lynch, etc.) are engaged as Reformed brothers in a live intramural debate, not as opponents in the sense Kline's system is treated — charity and accurate representation are non-negotiable, especially in the `contemporary-interlocutor` lane. Marino and Tomes in particular are running genuinely parallel natural-law/mediatorial-kingship arguments independent of this project (see `research/contemporary-interlocutors-map.md`) — credit convergence, don't imply priority.
- **Register:** technical precision is in service of doxology, not a substitute for it. Where an article's subject allows it, end on a pastoral or devotional note rather than a purely scholastic one.

## The six editorial lanes

This project divides labor across six Claude Code subagents in `.claude/agents/`. **Auto-invocation is unreliable in practice** — Claude often just does the work in the main session instead of delegating, even when a matching subagent exists. Invoke explicitly: *"Use the exegete subagent to draft the biblical-theological section of III.1"* rather than assuming Claude will route there on its own.

| Lane | File | Job |
|---|---|---|
| A | `historical-researcher.md` | Primary-source accuracy: Scholastics, Assembly minutes, 18th–19th c. controversies |
| B | `exegete.md` | Biblical-theological spine every systematic claim answers to |
| C | `confessional-reviewer.md` | Checks drafts against 1646 WCF/LC/SC text specifically |
| D | `contemporary-interlocutor.md` | Fair, sourced representation of Kline/VanDrunen/Federal Vision/Wolfe et al. |
| E | `pastoral-political.md` | The "so what" — pastoral, civil, and lay-practical implications |
| F | `editor-style.md` | House style enforcement and final read-through |

Default handoff order for a new article: **B + A** (gather exegetical and historical material) → **C** (check against confessional text) → **D** (only for articles engaging contemporary positions) → **E** (application) → **F** (final pass). Revise this per-article as needed; it's a default, not a rule.

## Repo structure

```
pro-rege/
├── CLAUDE.md
├── 00-foundations/        (manifesto, outline, bibliography, style-guide)
├── series-I-foundations/
├── series-II-ot-covenants/
├── series-III-nt-continuity/
├── series-IV-historical-debates/
├── series-V-implications/
├── .claude/agents/        (the six lane files)
└── research/              (scratch notes, source PDFs, quote-hunting — not for publication)
```

## Non-goals

- **Not fundamentally an anti-Kline, anti-VanDrunen, anti-R2K, or anti-Van-Til project.** It's a constructive reconstruction of the classical Reformed position on natural law, moral law, and their relation to special revelation, for ordinary Christians recalibrating their own foundations. The debates sharpen that reconstruction; they aren't its point. If a draft's critical engagement outweighs its constructive statement of positive doctrine, that's drift, not depth.
- Not a general-audience apologetics site.
- Not a polemical takedown blog — the goal is precision that clarifies, not point-scoring.
- Not attempting to relitigate Owen/Ball/Petto as an in-house squabble; that precision serves the constructive account first, and only secondarily sharpens the contemporary engagement with Klinean republication and its political-theological uses.
