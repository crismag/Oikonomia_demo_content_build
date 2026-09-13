# Data Play Generation Guide

This directory is the canonical entry point for generating Oikonomia Data Play content.

## Read order

1. `GENERATION-CONTEXT.md` — master handoff and non-negotiable principles.
2. `WORLD-AND-TIMELINE.md` — fiction, chronology, 2026 current/history window, future planning.
3. `CHURCH-ROLES-AND-MINISTRIES.md` — canonical church vocabulary, responsibilities and weekly rhythm.
4. `CONTENT-RULES.md` — biblical fidelity, explicitness, source-vs-record rules, metadata.
5. `CHARACTER-DEVELOPMENT-GUIDE.md` — how to turn a biblical person into a coherent Data Play identity.
6. `RECORD-TYPES.md` — what kinds of Oikonomia artifacts to author and how they differ.
7. `RELATIONSHIP-AND-SCENARIO-GUIDE.md` — continuity and cross-character story construction.
8. `HUMOR-AND-SENSITIVITY.md` — comedy boundaries and treatment of grave material.

Character-specific generation targets live separately under `/targets`. Generated canonical character material lives under `/characters`.

## Three-layer model

- `docs/generation/` = **how** Data Play must be generated.
- `targets/` = **what** still needs to be generated for each character.
- `characters/` = the **actual canonical authored content**.

Planning files are not finished content. Finished character content must not be reduced to prompts telling another AI what to write.

## Canonical principle

**AI writes the story. Oikonomia owns the records.**

This repository is a semantic authoring source. Oikonomia should import through its own domain/service layer rather than binding these documents to volatile database IDs or table layouts.

## Supersession

The older `docs/WORLD-RULES.md`, `docs/CHARACTER-PLAN.md`, and `docs/TIMELINE-PLAN.md` remain useful historical planning material, but this directory is authoritative where rules differ. In particular, the active populated window is January through September 2026; September 2026 through December 2027 is primarily future planning.