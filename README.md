# Oikonomia Demo Content Build

This repository is the authoring source for **Data Play — Biblical Leadership Demo**, a fictional 2026 Oikonomia organization populated by biblical characters as contemporary leaders.

## Core fiction

- All demo characters are alive and serving together in **2026**.
- Biblical history is their lived background and memory; it is not re-dated as if ancient events literally happened in 2026.
- Their recognizable biblical personalities, relationships, strengths, failures, journeys, victories, hardships, prayers, and leadership lessons inform how they behave today.
- Their Oikonomia activity is contemporary: agendas, goals, meetings, lifegroups, ministries, reports, tasks, prayers, follow-ups, attendance, documents, and leadership concerns.
- The tone may be warm and occasionally funny, but should remain respectful and useful as realistic church-leadership demo content.
- Demo visitors may switch between leader personas. Each persona must see the same shared organization through normal ownership and permission rules rather than through special fake pages.
- System/application dates stay within the supported 2026 demo year. Ancient events may appear as historical context or personal memories inside content.

## Purpose

This repository does **not** directly seed a database. It develops the canonical people, relationships, organization, scenarios, timelines, and authored content for the Oikonomia Demo (https://oikosdemo.crishub.com). An import script reads this human-readable content and builds the demo's baseline database; each character becomes a leader who can be signed in as in the demo.

The content should ultimately exercise real product behavior: shared and private records, attention items, assignments, reports, goals, meeting notes, lifegroup activity, ministry work, follow-ups, confidentiality, delegation, and cross-persona visibility.

## Structure

- `docs/generation/` — how content is generated; start with its `README.md`. `RECORD-FORMAT.md` defines the writing format the import script reads.
- `organization/` — campus, ministries, leadership groups and venues.
- `targets/` — per-character generation backlog and queue.
- `characters/` — canonical character profiles and finished content.
- `docs/WORLD-RULES.md`, `docs/CHARACTER-PLAN.md`, `docs/TIMELINE-PLAN.md` — earlier planning material, superseded by `docs/generation/` where they differ.
