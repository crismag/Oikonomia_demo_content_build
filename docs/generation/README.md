# Data Play Generation Guide

This directory is the canonical entry point for generating Oikonomia Data Play content.

## Destination

**Everything authored here is ultimately intended for transformation and insertion into the Oikonomia Demo.** Data Play may also read as biblical reflection, leadership case study, connected drama and occasional gentle comedy, but those are qualities of the content rather than a different destination.

Generation should therefore respect Oikonomia's actual sections, record types, ownership, ministries, permissions, relationships, workflows and continuity. Do not generate an application record merely because a biblical topic is interesting; determine where it naturally belongs in Oikonomia and what product behavior it exercises.

## Required read order

1. `GENERATION-CONTEXT.md` — master handoff and non-negotiable principles.
2. `AI-GENERATION-GUARDRAILS.md` — **required operating contract for Claude and every other AI author/reviewer.**
3. `WORLD-AND-TIMELINE.md` — fiction, chronology, 2026 current/history window, future planning.
4. `CHURCH-ROLES-AND-MINISTRIES.md` — canonical church vocabulary, responsibilities and weekly rhythm.
5. `CONTENT-RULES.md` — biblical fidelity, explicitness, source-vs-record rules, metadata.
6. `CHARACTER-DEVELOPMENT-GUIDE.md` — how to turn a biblical person into a coherent Data Play identity.
7. `RECORD-TYPES.md` — what kinds of Oikonomia artifacts to author and how they differ.
8. `RECORD-FORMAT.md` — **required writing format** for finished records, character identities and tags, so the import script can read them.
9. `RELATIONSHIP-AND-SCENARIO-GUIDE.md` — continuity and cross-character story construction.
10. `HUMOR-AND-SENSITIVITY.md` — comedy boundaries and treatment of grave material.
11. `STYLE-REFERENCE-REPORTS.md` — approved examples of report tone and style.

An AI should not begin substantial character generation after reading only a target file. It must use the generation context and guardrails, then inspect the character's existing workspace and relevant biblical source material.

Character-specific generation targets live separately under `/targets`. Canonical character material lives under `/characters`. The shared church structure lives under `/organization`.

## Layer model

- `docs/generation/` = **how** Data Play must be generated.
- `targets/` = **what** still needs to be generated for each character.
- `organization/` = the **shared church structure**: campus, ministries, leadership groups and venues.
- `characters/` = the **actual canonical authored content**.

Planning files are not finished content. Finished character content must not be reduced to prompts telling another AI what to write.

## Generation protocol

For substantial generation use:

**READ → RESEARCH → CLASSIFY FACTS → PLAN → WRITE → CROSS-CHECK → COMMIT**

The detailed protocol and required pre-commit audit are in `AI-GENERATION-GUARDRAILS.md`.

## Canonical principle

**AI writes canonical source content. A transformer maps it. Oikonomia validates and owns the resulting records.**

This repository is a semantic authoring source. Keep it independent of volatile database IDs, SQLite/table layouts and temporary UI implementation details. Records stay human-readable Markdown; `RECORD-FORMAT.md` fixes only the headings, field lines and closing lines an import script needs. The script produces a separate, disposable Oikonomia demo baseline and never rewrites this repository.

## Supersession

The older `docs/WORLD-RULES.md`, `docs/CHARACTER-PLAN.md`, and `docs/TIMELINE-PLAN.md` remain useful historical planning material, but this directory is authoritative where rules differ. In particular, the active populated window is January through September 2026; September 2026 through December 2027 is primarily future planning.