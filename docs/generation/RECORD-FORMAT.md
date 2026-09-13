# Record Format

This is the recommended writing format for finished character content. It is written for people first. An import script later reads these files and creates Oikonomia Demo records, so a few things are written the same way every time: record headings, the field lines under them, and closing lines.

The reference is David's newer content. Moses and Joshua predate this format and will be aligned to it.

**Rule of thumb:** a record should read naturally when printed. If a field line would not help a human reader, and the script does not need it, leave it out.

---

## 1. Files and records

A content file holds one or more related records.

```markdown
# David — Relationship and Leadership Reports: Saul

**Oikonomia section:** Leadership Report

> Optional preamble for the reader: source boundary, context, series notes.
> Nothing before the first record heading is imported.

---

## Saul Was the First King I Served Closely

**Record type:** Leadership Reflection
**Date:** 2026-02-15
**Visibility:** Leadership
**Status:** Complete
**Tags:** #reflective #serious #gratitude #grief

Body text…

**Biblical account:** 1 Samuel 16:14–23; 1 Samuel 18:5–16.

---

## Next record title
```

- `#` is the file title, and there is only one.
- `**Oikonomia section:**` under the file title says where the file's records belong in Oikonomia (see §3). A record may override it with its own `**Oikonomia section:**` line.
- `##` starts a record, and `---` separates records.
- `###` and deeper headings are sections inside a record's body.
- Field lines come directly under the record heading, one per line, as `**Name:** value`. End each field line that is followed by another with two spaces, so the lines render on separate rows. Examples in this document omit the spaces. They end at the first blank line followed by body text.
- Closing lines (§6) come at the end of the body, before any `### Comments`.

### Record titles

Use a plain, meaningful title. A date may lead the title when the file is a dated series:

```markdown
## 2026-01-15 — What Happened Before Goliath
```

A date in the heading counts as the record's date. Use ISO dates (`2026-01-15`) everywhere, including in headings.

---

## 2. Field lines

Only the fields that apply to a record need to be written.

| Field | Needed | Write | Notes |
|---|---|---|---|
| **Record type** | Reports | Free wording, e.g. `Field / Leadership Assessment` | Shown to readers as the report type. Keep it under 80 characters. Use `Family / Specific` when it helps. |
| **Date** | Always, unless the heading carries the date | `2026-03-15` | Every imported record needs a 2026 date. Weekly reports use the Sunday of that week. |
| **Owner** | Only when not the folder's character | A name from the roster, e.g. `Aaron` | Exactly one person. Name collaborators under **Shared with**, not as co-owners. |
| **Visibility** | Reports, Lifegroup entries | See §4 | |
| **Shared with** | When visibility names people | `Moses, Joshua` | Roster names separated by commas. |
| **Status** | Usually | Words for people, e.g. `Complete`, `Follow-up Required`, `Threat Resolved` | See §5. |
| **Tags** | Usually | `#serious #gratitude` | Tone first, then emotion or spiritual state. An open vocabulary, see §7. |

Use one spelling for each field. Do not use `Type:`, `Biblical foundation:` or `2026 goal link:`; use the names in this document.

**Names** are written as people read them: `Moses`, `James son of Zebedee`, `Philip the Evangelist`. The script matches them against the character roster, so use the roster spelling for anyone with a shared name. Where the person is not yet decided, `<Ministry> lead` (for example `Production lead`) refers to whoever heads that ministry in `/organization`.

---

## 3. Oikonomia sections

Choose the section by asking the question in `GENERATION-CONTEXT.md`: *where does this belong in Oikonomia, who owns it, who can see it?*

| Section | Use for | Record shape |
|---|---|---|
| **Leadership Report** | Weekly leadership reports, ministry reports, special or after-action reports, relationship, family and personal development reports, equipment or replacement requests, song submissions, testimony written as a report | §8.1 |
| **Lifegroup Gathering** | A Lifegroup report: how the gathering went, how it was carried out, its members, testimonies shared, what was discussed, prayer and follow-up | §8.2 |
| **Personal Reflection** | A private reflection that is not a report on any gathering, meeting or ministry work | §8.1 with `Visibility: Only me` or `Named people` |
| **Meeting Notes** | Meeting minutes or a personal meeting note, with decisions and action items | §8.3 |
| **Goals** | Annual or quarterly goals and their progress | §8.4 |
| **Calendar** | Recurring rhythm and dated events | §8.5 |
| **Agenda** | A leader's weekly to-do items: follow-ups, preparation, calls, commitments made in other records | §8.6 |
| **Reach-Out** | Outreach contact reports | §8.1 without visibility, status or tags |
| **Form** | Checklists or structured forms that genuinely need fields, such as a volunteer form | Discuss before authoring |

Every character is a leader. When a character attends a Lifegroup and writes its report, that character is one of the gathering's leaders, which is what lets them record the report in Oikonomia.

---

## 4. Visibility

Use the words Oikonomia shows its users.

| Write | Who can read it |
|---|---|
| `Only me` | The owner alone. For confession, pastoral matters and sensitive development. |
| `Named people` | The owner plus everyone listed under **Shared with**. **Shared with** is required. |
| `Leadership` | The owner, members of the church leadership body, and anyone under **Shared with**. |
| `Shared` | Intended for ordinary organizational reading. Add **Shared with** to guarantee specific readers. |

For **Lifegroup Gathering** entries such as a prayer request or follow-up:

| Write | Who can read it |
|---|---|
| `Lifegroup leaders` | Every Lifegroup leader. |
| `This gathering's leaders` | Leaders assigned to that gathering. |
| `Named people` | People under **Shared with**. |
| `Only me` | The author alone. |

Older content uses other words. Convert them when aligning:

| Old | New |
|---|---|
| `Shared` | `Shared` |
| `Leadership` | `Leadership` |
| `Restricted` | `Named people` with **Shared with** |
| `Highly Restricted` | `Only me`, or `Named people` naming one or two people |
| `Lifegroup` | Remove from a gathering report header (gathering reports have no visibility). On a gathering entry, use `Lifegroup leaders`. |

Visibility is part of the story. Do not widen it to make a scene easier to write. Cris is not omniscient.

---

## 5. Status

Write status for a person reading the record, e.g. `Complete`, `Follow-up Required`, `Alternative Equipment Selected`, `Threat Resolved`.

The import script only needs to know whether a record is finished:

- `Draft` → an unfinished draft the owner is still writing.
- Anything else → a finished record. The wording is kept for readers.

Goals use their own four statuses (§8.4). Unresolved work does not belong in Status. Write it as an **Attention** or **Action requested** line (§6).

---

## 6. Closing lines

These go at the end of a record body, in this order, when they apply.

```markdown
**Attention:** Watch for emerging leaders who read nervousness as disqualification.
**Attention to:** Moses
**Action requested:** Confirm the final instrument list before Production cutoff — from Production lead, by 2026-03-19
**Approval requested:** Replacement stone tablets — from Moses
**Related goal:** Goal 1 — Delegate without disappearing
**Biblical account:** Exodus 3–4.
```

| Line | Meaning | Notes |
|---|---|---|
| **Attention** | Something leaders should notice | Omit it, or write `None`, when there is nothing. A `### Attention` section with the same meaning is also accepted. |
| **Attention to** | Who should notice | A roster name, or one of: `Reporting leader`, `Ministry head`, `Campus leadership`, `Church leadership`. Default: `Reporting leader`. |
| **Action requested** | A concrete request someone must act on | `<request> — from <name or position>, by <date>`. The date is optional. |
| **Approval requested** | A decision someone must approve or decline | `<request> — from <name or position>` |
| **Related goal** | The owner's goal this record advances | Use the goal heading as written in `2026-goals.md`. |
| **Biblical account** | Scripture the record draws on | Every record whose content depends on a biblical event. Plain references; never invented quotations. |
| **Reflection theme** | Optional one-line truth or lesson | For reflective records where it helps the reader. |

---

## 7. Tags

Tags describe the **tone** of the record and the author's **emotional or spiritual state**. List tone first.

The vocabulary is open. Start from the base set below. Add a new tag when none fits, after checking there isn't already a near-synonym (`#reflective`, not `#reflection`).

- **Tone:** `#serious` `#administrative` `#reflective` `#devotional` `#dramatic` `#pastoral` `#celebratory` `#light` `#funny` `#cringe`
- **Emotion:** `#joy` `#gratitude` `#hope` `#peace` `#relief` `#awe` `#fear` `#anxiety` `#grief` `#regret` `#anger` `#frustration` `#exhaustion` `#confusion` `#uncertainty` `#distress` `#resentment` `#jealousy`
- **Spiritual stance:** `#conviction` `#courage` `#faith` `#humility` `#repentance` `#restraint` `#accountability` `#discernment` `#lament` `#compassion` `#confidence` `#obedience`

Do not use tags for things that have their own place: ministry (`#production`), record kind (`#equipment`, `#assessment`) or topic (`#leadership`). Tag the record, not the biblical story it mentions.

Up to 30 tags per record, each under 40 characters; 3–6 is normal.

---

## 8. Record shapes

### 8.1 Leadership Report

````markdown
## Victory / After-Action Report — Goliath

**Record type:** After-Action / Victory Report
**Date:** 2026-02-22
**Visibility:** Shared
**Status:** Threat Resolved
**Tags:** #dramatic #serious #courage #faith

### Situation

…

### Outcome

…

**Attention:** None.
**Biblical account:** 1 Samuel 17:38–54.

### Comments

**Cris:** Logged. Please do not attach the sling to the equipment register.
**David:** It was returned to the bag.
````

Body sections are free. Use the headings the record needs: Situation, Outcome, Leadership lesson, Next week and so on.

**Comments** go under `### Comments` as one `**Name:** text` paragraph per comment, in order. Comments are imported for **Leadership Reports** and **Reach-Out** only. Oikonomia comments are a flat list; a reply is simply the next comment.

### 8.2 Lifegroup Gathering

```markdown
## 2026-01-15 — What Happened Before Goliath

**Led by:** David, Samuel
**Venue:** Fellowship hall
**Attendance:** Samuel, Solomon, Miriam (first-time visitor: Dan R.)
**Tags:** #reflective #devotional #courage

How the gathering went: what was shared, how members responded, testimonies, what was discussed…

### Discussion

What responsibilities are forming us now that nobody considers impressive?

### Prayer

**Visibility:** Lifegroup leaders

Pray for …

**Biblical account:** 1 Samuel 16–17.
```

- A Lifegroup Gathering record is the **gathering report**: how the group went, how it was carried out, its members, testimonies shared and what was discussed. It is written in the reporting leader's own voice.
- **Led by** defaults to the folder's character, who is always one of the gathering's leaders. List co-leaders with commas.
- **Venue** and **Attendance** are optional. A non-roster attendee can be named in plain words.
- The heading title is the gathering's topic. The body before the first `###` section is the report. **Biblical account** is the Scripture the gathering centred on. Keep the report under about 600 words.
- `### Discussion`, `### Prayer`, `### Testimony`, `### Follow-up` and `### Attention` become entries on the gathering. Each may carry its own **Visibility** line; the default is `Lifegroup leaders`. Use `Only me` or `Named people` for a member's sensitive prayer request or a private follow-up.
- A gathering record needs no Record type, Visibility or Status line; it is a completed gathering unless its Status says `Cancelled`.
- A gathering has no comments.

### 8.3 Meeting Notes

```markdown
## 2026-03-10 — Psalmists / Production Input List Review

**Kind:** Minutes
**Meeting type:** Ministry
**Facilitator:** David
**Note taker:** Miriam
**Participants:** David, Miriam, Production lead
**Absent:** Solomon
**Tags:** #administrative #light

### Discussion

…

### Decisions

- Late instrument additions require confirmation before soundcheck.

### Action items

- [ ] Send final instrument list to Production — David, due 2026-03-12
- [x] Update channel assignments — Production lead
```

- **Kind** is `Minutes`, which participants can read, or `Personal note`, which only the owner and note taker can read.
- **Meeting type** is `Leaders`, `Ministry`, `Lifegroup`, `Planning`, `Coaching`, `Campus` or `Other`.
- Action items are checklist lines, `- [ ] Task — Assignee, due YYYY-MM-DD`. `[x]` marks one done.
- A shared meeting has **one** canonical file. Other characters' records refer to it; they don't copy it.

### 8.4 Goals

```markdown
## Goal 1 — Receive correction before defending myself

**Status:** Active
**Ministry:** Psalmists
**Target:** 2026-12
**Tags:** #serious #conviction #humility

### Why this matters

…

### 2026 actions

- …

### Progress

- 2026-03-01 — Restated Nathan's concern before explaining myself in the Psalmists review.
- 2026-06-14 — …

**Biblical account:** 2 Samuel 11–12; Psalm 51.
```

- **Status** is `Active`, `Completed`, `On hold` or `Carried forward`.
- **Ministry** is optional. When it is set, that ministry's team can edit the goal.
- **Target** is a month (`2026-12`) or date (`2026-12-20`).
- *Why this matters* and *2026 actions* together become the goal description. Keep them under about 300 words.
- Each dated `### Progress` bullet becomes a progress update on that date.

### 8.5 Calendar

```markdown
## Mentorship Night

**Repeats:** Weekly on Tuesday
**Time:** 19:00–21:00
**From:** 2026-01-06
**Until:** 2027-12-28
**Category:** Mentorship
**Ministry:** Mentorship
**Location:** Main hall

Short note for the calendar entry.
```

Or for a one-off event, `**Date:** 2026-04-05` instead of `Repeats` / `From` / `Until`.

- **Repeats** is `Daily`, `Weekly on <day>`, `Fortnightly on <day>`, `Monthly` or `Yearly`.
- **Category** is fixed by Oikonomia: `Prayer & Fasting`, `CHAT`, `Lifegroup`, `Potbless`, `Victuals`, `SEED`, `Mentorship`, `Ministry meeting`, `Service`, `Celebration` or `Other`. Psalmists practice, Production and Greeters use `Ministry meeting` or `Service`.

---

### 8.6 Agenda

```markdown
# Peter — Weekly Agenda — August to September 2026

**Oikonomia section:** Agenda

---

## Week of 2026-08-31

- [x] Call the Riverside family before the follow-up visit — due 2026-09-02 — Field Ministry
- [ ] Brief four remaining Lifegroup leaders on in-person handoffs — due 2026-09-06
- [x] Coffee with John — Thursday
- [ ] Ask Tunde about co-leading from October — for Marisol
```

- One file per person; one `## Week of YYYY-MM-DD` record per week. The date is the **Monday** of that week.
- Each item is one checklist line. `[x]` is done, `[ ]` is open.
- After the text, optional parts separated by ` — `, in any order:
  - `due YYYY-MM-DD`, or a weekday (`Thursday`) meaning that day of the week;
  - a ministry name from `organization/ministries.md`;
  - `for <Name>` when the item is done on behalf of, or assigned to, another roster person.
- Items should come from somewhere real: a meeting action, a follow-up, a commitment in a report, a calendar occasion. Agendas are not a place to invent new storylines.
- Keep item text short and concrete. Pastoral details stay out; "Call L.K." or "Hospital visit (see restricted note)" is enough.
- Agendas are private working lists: they have no visibility, status or tags lines, and no comments.

## 9. Writing inside a record

The body converts cleanly into Oikonomia when it uses:

- paragraphs,
- `###`/`####` headings,
- bullet and numbered lists (one level),
- checklists,
- block quotes,
- **bold**, *italic* and links.

Avoid tables, images, code blocks and nested lists inside record bodies. File preambles and profiles may use them freely, because they are not imported.

---

## 10. Characters as people

Every character is also a person in the demo organization. The top of `profile.md` carries an **Oikonomia identity** block, written in the same field-line style:

```markdown
## Oikonomia identity

**Name:** David
**Title:** Senior Leader · Psalmists
**Access:** Leader
**Campus:** Main campus
**Reports to:** Moses
**Ministries:** Psalmists — head; Mentorship — member
**Groups:** Leadership Council — member
**Leads Lifegroups:** Yes
**Demo persona:** Featured
```

- **Title** is the church title shown beside the name, under 120 characters.
- **Access** is `Leader`, `Ministry Head`, `Bishop` or `Admin`. Access is not rank: a ministry head's rights come from leading the ministry, and a leadership body's reach comes from the group.
- **Ministries** and **Groups** are `Name — function`, where function is `head`, `leader`, `coordinator`, `member` or `service-worker`. Use `— sees only` for someone who can see a ministry's work without being on its team.
- **Leads Lifegroups** is `Yes` when the character writes Lifegroup Gathering reports. Every character is a leader, so this only records whether they take part in Lifegroup reporting.
- **Demo persona** is `Featured` (offered in the demo chooser), `Available` (offered, lower in the list) or `No` (present as a colleague only).

Ministries, leadership groups, campuses and venues are defined once in `/organization`, in the same readable style, and referred to by name everywhere else.

---

## Appendix — How the import script reads this

For script maintainers. Authors do not need this section.

| Written | Becomes in Oikonomia |
|---|---|
| Leadership Report record | `leadership_report`: title, `report_type` ← Record type, `reporting_period` ← "Week of <Date>", `tags`, `visibility` + `audience_ids`, blocks ← body, status `published` (or `draft`), `published_at` ← Date |
| Personal Reflection | `leadership_report` with visibility `private` / `restricted` |
| Comments | `comment` rows on the report, in order, timestamps spaced after Date |
| Attention / Action requested / Approval requested | `escalation` of type attention / action / approval, source = the report, `requested_from_role` or `requested_from_person` |
| Related goal, Biblical account, Reflection theme | Final paragraph block of the body; Biblical account also in `related_text` |
| Lifegroup Gathering | `gathering` (date, `assigned_leaders` ← owner + Led by, `primary_leader_id` ← owner, venue, status `completed`), `report_summary` ← body, `exhortation_topic` ← title, `exhortation_scripture` ← Biblical account, `gathering_attendance`, `lifegroup_entry` per Discussion / Prayer / Testimony / Follow-up / Attention section. Reports by several characters on the same date and venue belong to one gathering. |
| Meeting Notes | `meeting_note` (`note_type`, `meeting_type`, facilitator, note taker, participants, absentees, blocks, tags) + `meeting_task` per action item |
| Goal | `goal` (year 2026, status, ministry, owner, target, description) + `goal_update` per Progress bullet |
| Calendar | `schedule_entry` (single date or recurrence, category, ministry, organizer ← owner) |
| Agenda | `agenda_item` per checklist line: `text`, `week_of` ← week Monday (or `date` when a weekday or due date is given), `completed` ← `[x]`, `due_at` ← due date, `ministry_id`, `assignee_id` ← `for <Name>` or owner |
| Oikonomia identity | `person`, `account` (active), `onboarding_state` (complete), `ministry_member` / `responsibility_group_member` (confirmed), `demo_identity` for Featured / Available |
| Status word | `Draft` → draft; anything else → finished; original wording kept in the body header |
| Tag spelling | Lowercased, `#` stripped |
| Names | Resolved against the character roster; an unresolved name fails the import |
| Record identity | Derived from file path + record heading; renaming a heading creates a new record on the next baseline build |

Open decisions on the Oikonomia side:

- Report visibility `shared` currently reaches only the named audience. Either Oikonomia makes `shared` organization-wide, or the script expands `Shared` to a default audience.
- Imported history needs real 2026 timestamps. Services stamp the current time, so the baseline builder must write `created_at` / `published_at` directly.
- Oikonomia has no report→goal link. **Related goal** is kept as text until one exists.
- Lifegroup entry categories are hard-coded, and `updateGathering` drops `notes`. Both are Oikonomia defects to fix, not reasons to change this format.
