# Data Play Generation Context

Use this as the master handoff for a fresh authoring session.

## Purpose and destination

**Data Play exists to produce canonical source content for eventual transformation and insertion into the Oikonomia Demo application.**

Oikonomia is a church leadership planning/reporting platform. Data Play is not primarily an independent Bible-character writing project, devotional collection or fictional novel. It may intentionally have the richness of biblical reflection, leadership case study, connected character drama, occasional gentle comedy and Daily Bread-like reading, but the eventual destination is Oikonomia.

Generated material should therefore map naturally to Oikonomia's actual sections and product behavior: Weekly Calendar / Agenda, Monthly Calendar / Agenda, Meeting Notes, Ministry, Lifegroup, Reach-Out, Leadership Progress Report and Volunteer Forms / Documents, together with Goals, Attendance, People, Events, tasks/actions, Attention Required, comments/follow-ups, permissions, shared/personal workspaces, linked documents, completion and printable views.

Before generating an application artifact ask: **Where does this belong in Oikonomia, who owns it, who can see it, and what later activity can it affect?** Do not create a record merely because a biblical topic is interesting. Some history belongs in character/context material rather than an application record.

The content must simultaneously work as realistic application data and worthwhile human-readable material. It is not a collection of sterile fixtures and not a collection of prompts for future AI generation.

**Required:** every AI author or reviewer must also read `AI-GENERATION-GUARDRAILS.md` before substantial generation.

## Central fiction

All selected biblical characters are contemporaries and present today in the shared Oikonomia world.

**2026 is real. Biblical history is memory/background. Biblical personality is character. Oikonomia activity is present-day.**

Their biblical accounts are their actual lived past. Moses may remember the Red Sea. David may discuss Ziklag. Peter may remember his denial. Paul may refer to journeys, disagreements, imprisonment or churches he served. These memories are not fictionalized into having happened in 2026.

A current 2026 circumstance may naturally trigger a detailed reflection on a historical biblical event. Do not gimmickily reenact Scripture in modern Toronto or pretend ancient events happened in 2026.

Jesus generally remains the theological and historical center rather than an ordinary demo account receiving mundane overdue tasks.

## Timeline

- January 2026 through September 2026: populated current demo calendar and accumulated history.
- September 2026 through December 2027: future plans, schedules, goals and anticipated activity.
- A character's whole biblical life may be used as lived history regardless of where a 2026 record falls.

## Content objective

Author actual records: reports, meetings, schedules, goals, tasks, Lifegroup entries, ministry activity, prayers, testimony, personal development, mentorship, conversations/comments, attention items, follow-ups, operational reviews and related artifacts.

The transformer/importer should mostly map authored substance into Oikonomia records. It should not invent the character's story.

**AI writes canonical source content. A transformer maps it. Oikonomia validates and owns the resulting records.**

## Biblical literacy

**Do not assume biblical literacy.**

When an event matters, provide enough context to understand the people, situation, conflict, what happened, biblical truth and present application. Use short references when context already exists, medium retellings for meetings/Lifegroups, and full narrative reflections for testimony, development, hardship, prayer and mentoring.

Where useful add:

> **Biblical account:** Exodus 14:5–31  
> **Reflection theme:** Faith under pressure; knowing when to wait and when to move.

Never fabricate a quotation and attribute it to Scripture.

## Voice

Use contemporary leadership language, not archaic/KJV imitation. Preserve recognizable personality without reducing a person to a single trait. David is not merely worship. Thomas is not merely doubt. Martha is not merely hospitality. Jonah is not merely a joke.

## Interconnection

Characters share one organization. OT leaders, prophets, the Twelve and Acts/letter personalities may collaborate, mentor, disagree and attend shared activities. Cross-era relationships are allowed as 2026 fiction. Biblical relationships remain especially important where they exist.

Shared artifacts should have one canonical source and be referenced by participants rather than duplicated with divergent copies.

## Oikonomia product behavior

Data Play should exercise real product concepts: leader-created work, shared workspaces, personal workspaces, attention-required states, permissions, confidential/restricted reports, cumulative history, printable records, tasks from meetings, assignments, completion, attendance and linked follow-up.

Persona switching uses normal authorization. It does not create omniscient access. Admin/system access does not automatically expose confidential pastoral content.

Respect record boundaries. Calendar/activity records say what happened and when; meetings/gatherings record what happened within them; reports explain what mattered and what needs attention; tasks state concrete work and ownership. Do not repeat identical prose merely to populate multiple sections.

## Ministries

Use the canonical church ministries and responsibilities in `CHURCH-ROLES-AND-MINISTRIES.md`. Put work where it belongs. Example: manna/food provision belongs naturally in Victuals material even when Moses is historically central to the account.

Topics are perspectives, not exclusive ownership. Multiple characters may legitimately reflect on one biblical event, but their Oikonomia artifacts should represent genuinely different responsibilities or perspectives rather than duplicated content.

## Humor

Humor should arise from personality, administrative framing, modern workflow friction or harmless consequences of recognizable history. Main reports remain coherent. Freer banter belongs mainly in comments. Long comments are welcome when the setup makes the joke understandable.

A comment thread may intentionally remain unanswered when the unresolved state itself is funny or useful demo data.

**Explicit first, clever second.**

## Sensitivity

Grave sin, death, sexual violence, abuse, trauma and human suffering are not comedy material. Describe serious biblical failures plainly enough to preserve moral truth. Repentance does not erase consequences.

## Metadata

Write records in the human-readable format defined in `RECORD-FORMAT.md`: record headings, a few field lines (record type, date, visibility, status, tags), closing lines for attention, requests, related goals and biblical accounts, and comments.

Tags describe tone and emotional or spiritual state. The vocabulary is open, grows from the base set in `RECORD-FORMAT.md`, and describes the actual record, not merely the biblical story mentioned.

## Source architecture

Prefer stable semantic identities such as `person.david`, `ministry.psalmists`, `scenario.david.ziklag` rather than database IDs. Inside records, refer to people, ministries and groups by their roster or `/organization` names; the import script resolves them. Canonical source documents remain human-readable and semantically structured rather than imitating current SQLite tables or volatile implementation details.

Generated/import output is disposable and separate. Canonical source content must never be rewritten by a transformer.

## Required generation discipline

For substantial generation follow:

**READ → RESEARCH → CLASSIFY FACTS → PLAN → WRITE → CROSS-CHECK → COMMIT**

The complete factual, chronology, character, Oikonomia, permissions, humor, sensitivity and pre-commit rules are authoritative in `AI-GENERATION-GUARDRAILS.md`.

## Quality test

A strong Data Play record should still be worth reading if the reader temporarily forgets it is software test data. It should also remain structured and realistic enough that, when imported, it naturally belongs in Oikonomia and meaningfully exercises the product.

When biblical fidelity, Oikonomia usefulness and creative flourish compete, **biblical fidelity comes first, then coherent Oikonomia use, then creative flourish.**