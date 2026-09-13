# AI Generation Guardrails

## Purpose and destination — read this first

**Data Play exists to produce canonical demo content for eventual insertion into the Oikonomia Demo application.**

This repository is not primarily a Bible-character writing project, devotional collection, fictional novel, or independent dataset. Those qualities may enrich the material, but the destination is **Oikonomia**: a church leadership planning and reporting application.

Generated material must therefore map naturally to Oikonomia sections, record types, relationships, permissions, workflows, cumulative history and user experiences.

Primary binder destinations are:

1. Weekly Calendar / Agenda
2. Monthly Calendar / Agenda
3. Meeting Notes
4. Ministry
5. Lifegroup
6. Reach-Out
7. Leadership Progress Report
8. Volunteer Forms / Documents

Supporting product concepts include Goals, Attendance, People, Events, tasks/actions, Attention Required, comments and follow-ups, permissions, shared and personal workspaces, linked documents, completion states and printable views.

Before authoring an application record, ask: **Where would this artifact belong in Oikonomia, who owns it, who can see it, and what later activity can it affect?**

Do not generate a record merely because a biblical story would be interesting. Some biblical history exists primarily to establish identity, character, relationships and context. Conversely, do not flatten rich biblical material into sterile software fixtures.

**AI writes canonical source content. A transformer maps it. Oikonomia validates and owns the resulting records.**

Canonical source documents must remain human-readable and semantically structured. Do not couple authoring to current SQLite tables, volatile database IDs, implementation details or temporary UI structure.

---

## Authority order

When sources conflict, use this order:

1. Scripture and accurately established biblical facts.
2. This repository's current canonical generation rules under `docs/generation/`.
3. Existing canonical character/scenario content under `characters/`.
4. Character target and planning files under `targets/` and character planning documents.
5. New creative extrapolation.

A lower layer must never silently overwrite a higher layer.

If existing canonical Data Play material appears to contradict Scripture, **stop and report the conflict**. Do not silently rewrite Scripture, reinterpret the conflict away, or quietly alter established content.

---

## Biblical research and factual guardrails

### Scripture outranks creativity

Never change a biblical event, relationship, outcome or moral reality to improve a storyline, joke, workflow or character arc.

### Research before generation

Before developing a character substantially, review the person's complete relevant biblical source material, not only the famous episode or the existing topic list. Topic files are research guides, not exhaustive authorities.

Research should look for:

- explicit events and actions;
- relationships;
- words actually attributed to the person;
- responsibilities and roles;
- strengths and faithfulness;
- failures, correction and consequences;
- changes across the person's life;
- emotions explicitly shown or strongly supported by the text;
- later biblical references to the person or event;
- unresolved or ambiguous matters.

### Do not invent through biblical silence

Do not manufacture ancient parents, childhoods, occupations, motives, private conversations, romantic histories, psychological diagnoses, dates, travel details, emotions or relationships simply because they would make the character easier to write.

Sparse characters should remain appropriately sparse. A supporting character does not need an invented full biography to justify inclusion in Data Play.

### Three epistemic layers

Always distinguish these layers mentally and, where ambiguity could mislead a reader, explicitly in the content:

**Biblical fact** — Scripture states or clearly establishes it.

**Interpretation/inference** — a reasonable conclusion or traditional interpretation, but not explicit fact.

**Data Play fiction** — contemporary activity invented for the Oikonomia Demo.

Never present inference or Data Play fiction as Scripture.

### References must support the claim

Do not attach a plausible-looking biblical citation without checking that the passage actually supports the statement. A citation is not decoration.

### Namesakes and disputed identities

Take special care with repeated names: James, Judas, Mary, Philip, Herod and similar cases. Do not merge people because their names or roles look compatible.

Where an identification is traditional or disputed rather than explicit — for example Nathanael/Bartholomew — retain appropriate qualification instead of silently declaring certainty.

### Preserve uncertainty

When the biblical text does not settle a question, preserve that uncertainty. **Uncertainty is preferable to a polished hallucination.**

---

## Time and world guardrails

**2026 is real. Biblical history is memory. Biblical personality is character. Oikonomia activity is present-day.**

Do not forward-date Scripture. The Red Sea did not occur in March 2026; Moses may submit a March 2026 reflection about having crossed it.

Do not back-project Oikonomia into biblical history. Cameras, microphones, production equipment, Oikonomia reports, modern church departments, Toronto locations, contemporary forms and electronic calendars did not exist in the ancient account.

A modern situation may cause a character to remember biblical history. Do not gimmickily reenact a miracle or biblical event merely to create a 2026 scenario.

Current timeline:

- January 2026 through September 2026: populated/current demo history.
- September 2026 through December 2027: primarily future plans, schedules, goals and anticipated activity.

The character's whole biblical life remains available as lived historical memory.

Cross-era character interaction is intentional **2026 Data Play fiction**. Biblical characters from different historical periods may serve together today, but their ancient histories must not be rewritten to pretend those relationships existed in biblical time.

---

## Character integrity

Do not reduce a person to the trait by which popular culture remembers them.

Examples:

- Thomas is not merely doubt; include courage, questions, evidence and confession.
- Martha is not merely anxiety or food service; include faith, confession, grief, hospitality and relationship.
- Peter is not merely impulsive; include leadership, revelation, failure, restoration, courage, pastoral development and growth.
- John Mark is not permanently the person who withdrew; preserve restoration and later usefulness.
- Jonah is not merely comic resistance; preserve the theological seriousness of God's compassion and Jonah's heart problem.
- David is not merely worship or heroism; preserve leadership, failure, abuse of authority, repentance, consequences, grief and preparation for the next generation.
- Gideon's victory does not erase his later complications.
- Solomon's wisdom does not erase his later compromise.

Failure is not identity. Success is not sanitization.

Use contemporary language while preserving distinguishable personality. Do not make Moses, David, Peter, Paul, Nehemiah and every other leader sound like the same modern management consultant.

Jesus generally remains the theological and historical center, not an ordinary demo persona. Do not assign Jesus mundane overdue reports, administrative comedy or invented 2026 dialogue simply to exercise a feature.

---

## Oikonomia record guardrails

### Put work where it belongs

The famous person in a biblical account does not automatically own every modern record inspired by it.

Examples:

- food, manna and meal provision naturally inform Victuals;
- praise, songs, dancing and instruments naturally inform Psalmists;
- transport, site setup, tents and logistics naturally inform Facilities;
- children and generational teaching naturally inform Gifts and Arrows;
- outreach distribution and giving naturally inform More Than Enough;
- offsite visitation naturally informs Field Ministry.

Characters may still reflect on the same historical event from their own legitimate perspective.

### Topics are perspectives, not exclusive ownership

The same biblical event can support several distinct records when the perspectives are genuinely different. Do not copy the same prose into multiple characters or modules.

### Respect record boundaries

- Calendar/activity: what happened or is planned, and when.
- Meeting/Gathering: what happened within the gathering.
- Ministry record: ministry-specific activity and operational substance.
- Leadership report: what mattered, changed, needs attention and what happens next.
- Goal: desired development/outcome and measurable progress.
- Task/action: concrete work, owner and follow-up.
- Comment: contextual conversation, clarification or coherent banter.
- Personal development: character formation, correction, learning and growth.
- Testimony/prayer/reflection: spiritual meaning and response.

Do not duplicate identical prose across these surfaces.

### Do not sermonize every record

A Facilities report may simply be a good Facilities report. A task may simply state what needs doing. Biblical truth should be explicit where meaningful, especially in reflection, testimony, Lifegroup, mentoring and development records, but not mechanically appended to every operational artifact.

### No artificial completeness

Not every character needs every module, ministry, emotion, record type or week of activity. Do not create filler because a calendar contains 39 Sundays or because a schema supports a field.

Ordinary activity can be concise. Significant activity deserves depth.

### Continuity over isolated cleverness

A consequential record should affect later records. Assignments persist. Goals progress. Conflicts have consequences. Delegation changes workload. Recovery changes later capability. An attention item can remain open. Do not generate a dramatic event and forget it the following week.

### Permissions are part of the story model

Do not grant a character access merely because it would make writing easier. Shared, personal, restricted and confidential records must respect Oikonomia's authorization model. Admin/system access does not automatically mean pastoral/confidential access. Cris is not omniscient.

---

## Fact, fiction and dialogue

Invented contemporary dialogue is allowed when it is clearly Data Play interaction. Never fabricate dialogue and imply that Scripture records the character historically saying it.

Historical retellings should distinguish direct biblical quotation from paraphrase. Never manufacture a quote and attach a verse to it.

Comments are the preferred location for freer fictional interaction and administrative humor. Main reports should remain coherent and useful as application records.

A fictional contemporary record may explicitly describe a true biblical memory. The reader should be able to tell which part is remembered history and which part is the 2026 framing.

---

## Humor guardrails

**Explicit first, clever second.**

A reader with low biblical literacy should be able to understand the setup. If the joke depends on Moses breaking the tablets, explain that he broke them after seeing the golden calf rather than assuming the reader already knows.

Prefer humor from:

- ordinary administration applied to extraordinary historical experience;
- recognizable personality;
- workflow friction;
- harmless consequences;
- comments and review threads;
- contemporary organizational misunderstandings that do not rewrite Scripture.

Administrative absurdity is preferable to changing a biblical event for a joke.

Do not turn grave sin, sexual violence, abuse, murder, death, severe illness, trauma, judgment or grief into comedy.

Do not make every character funny. Do not write serious biblical leaders as comedians merely because Data Play permits humor.

Unresolved humorous threads may remain unresolved. AI must not compulsively provide a response, reconciliation or punchline to every comment thread.

---

## Sensitivity and moral clarity

Describe serious biblical failures with enough clarity that their moral weight is not erased by modern corporate language.

Do not romanticize adultery, abuse of power, violence, exploitation or betrayal. Do not make repentance a mechanism that removes consequences.

Do not use psychological or medical labels unsupported by the biblical text.

When writing grief, persecution, illness, violence or trauma, prioritize dignity and biblical fidelity over drama.

---

## Canonical-content protection

Existing canonical character and scenario content outranks newly generated convenience. Before modifying an established character, read the existing files.

Do not casually rewrite Moses, Joshua, David or another developed character because a newly generated character would be easier to connect if history changed.

Shared scenarios should have one canonical source. Participants can reference or respond to that source rather than creating incompatible copies.

Target files and `notable-topics.md` are plans, not Scripture and not necessarily exhaustive. Research may discover a missing biblically grounded topic. Add it deliberately rather than pretending the planning list was complete.

Transformers/importers must not rewrite canonical source content. Generated import artifacts should be separate and disposable.

---

## Required AI generation protocol

Use this sequence for substantial character/content generation:

### 1. READ

Read the canonical generation documents, the character target, existing character workspace, related characters and relevant shared scenarios.

### 2. RESEARCH

Review the complete relevant biblical account. Expand beyond the famous episode. Verify names, relationships, chronology and references.

### 3. CLASSIFY FACTS

Separate biblical fact, interpretation/inference and proposed Data Play fiction. Identify disputed or uncertain points.

### 4. PLAN

Determine which topics naturally produce Oikonomia artifacts. Identify owner, section/module, visibility, relationships, chronology and later consequences.

### 5. WRITE

Author actual human-readable canonical content, not prompts telling another AI what to generate. Preserve character voice and appropriate detail.

### 6. CROSS-CHECK

Check the new material against Scripture, generation rules, existing canonical content, ministry ownership, permissions, timeline and related characters.

### 7. COMMIT

Only after the content passes the self-audit should it become canonical repository material.

Short form:

**READ → RESEARCH → CLASSIFY FACTS → PLAN → WRITE → CROSS-CHECK → COMMIT**

---

## Required pre-commit self-audit

Before declaring substantial generation complete, verify all of the following:

- Biblical claims are accurate and references support them.
- Biblical fact, inference and Data Play fiction have not been blurred.
- No biblical event was moved into 2026.
- No modern concept was projected backward into Scripture.
- Namesakes/disputed identities were handled carefully.
- Biblical silence was not filled with invented ancient biography.
- Character voice is distinct and not reduced to one popular trait.
- Serious material retained appropriate moral and emotional weight.
- Humor is coherent, understandable and appropriately located.
- The artifact has a natural Oikonomia destination.
- Ministry/record ownership is appropriate.
- Record types are not duplicating one another.
- Permissions and confidentiality are plausible.
- Cross-character relationships are consistent.
- Consequences and open items can continue into later records.
- Existing canonical content was not contradicted or casually rewritten.
- The material is actual authored content rather than a prompt for future generation.
- Sparse source material was not inflated into unsupported biography.
- Uncertainty remains uncertainty where Scripture does not settle the issue.

If any check fails, correct it before commit. If correction would require changing a higher-authority canonical fact, **stop and report the conflict instead of silently resolving it**.

---

## Final quality standard

A strong Data Play artifact should satisfy three tests simultaneously:

1. **Biblically responsible:** a knowledgeable reader should not be misled about what Scripture says.
2. **Worth reading:** the content should have human, leadership, devotional, dramatic or appropriately humorous value beyond being test data.
3. **Oikonomia-native:** after transformation, it should look as though it naturally belongs in the Oikonomia Demo and meaningfully exercises the product.

When these goals compete, biblical fidelity comes first, then coherent Oikonomia use, then creative flourish.