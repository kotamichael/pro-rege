# Pro-Rege Project — Claude Code Context

This file is loaded automatically at the start of every Claude Code session in this repo. Keep it current — when the real style guide and bibliography exist, this file should be trimmed down to point at them rather than duplicating them.

## What this project is

A multi-article project defending a strict-1646-Westminster-Standards account of the relationship between the covenant of works and the covenant of grace across both Testaments — moral law, natural law, and grace under each administration — written in critical engagement with Klinean republication and its political-theological descendants. See `00-foundations/manifesto.md` for the full statement (once drafted — Phase 0.1 of the project TODO).

## Current state of foundational docs — check before assuming any of this is final

- `00-foundations/manifesto.md` — **not yet drafted**
- `00-foundations/outline.md` — draft skeleton exists in the project TODO; not yet finalized as its own file
- `00-foundations/bibliography.md` — **not yet drafted**; several contemporary authors listed in the TODO (Prakashpalan, Ruddell, Owen Anderson, Meyers, Smyth, Tomes, Weissman, Marino, Mattull) still need their specific published positions verified before they're cited — do not attribute claims to them from memory
- `00-foundations/style-guide.md` — **not yet drafted** — see provisional rules below

## Provisional house rules (supersede with `style-guide.md` once it exists)

- **Scripture quotation:** KJV by default, matching usage throughout the project's founding conversation. Confirm with the project owner before treating this as locked.
- **Confessional citation:** always cite the **1646** Westminster Confession / Larger Catechism / Shorter Catechism wording specifically. Where later American revisions differ (WCF 23 on the civil magistrate is the main case), state the difference explicitly rather than silently using the revised text.
- **Uncertainty discipline:** never assert a specific claim about a named living or recent author's published position without a verifiable source. If a claim can't be confirmed, say so plainly in the draft (e.g., an inline `[VERIFY: ...]` marker) rather than smoothing it into confident prose.
- **17th-century primary sources:** preserve original spelling/orthography in direct quotation (e.g., "stedfastly," "shew"); modernize only in paraphrase, and mark paraphrase as paraphrase.
- **Living authors** (Wolfe, Beers, Lynch, etc.) are engaged as Reformed brothers in a live intramural debate, not as opponents in the sense Kline's system is treated — charity and accurate representation are non-negotiable, especially in the `contemporary-interlocutor` lane.
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

- Not a general-audience apologetics site.
- Not a polemical takedown blog — the goal is precision that clarifies, not point-scoring.
- Not attempting to relitigate Owen/Ball/Petto as an in-house squabble; that precision is a tool aimed at a specific contemporary target (Klinean republication and its political-theological uses).
