# Organization

The shared church structure of the Data Play demo. Records and character profiles refer to these by name; the import script turns them into Oikonomia campuses, ministries, responsibility groups and venues.

- `campus.md` — the campus.
- `ministries.md` — every ministry, its purpose and its lead.
- `groups.md` — leadership bodies and other responsibility groups.

Write entries in the field-line style of `docs/generation/RECORD-FORMAT.md`. Ministry responsibilities and weekly rhythm are canonical in `docs/generation/CHURCH-ROLES-AND-MINISTRIES.md`; this folder only adds who leads and who belongs.

Assign a lead or member only when the character's canonical content supports it. `Not yet assigned` is a valid state until that character is generated.

Venues are added here when a record first needs one.

## Where organization-level records live

- **Ministry goals:** `characters/<head>/content/ministry-goals/2026-<ministry>.md`, owned by each ministry head. Gifts and Arrows has no head yet; its Council goal is in Moses' folder.
- **Weekly church schedule and dated events:** `characters/cris/content/calendar/`, maintained by Cris as coordinator.
- **Meeting minutes:** in the folder of the person who owned the meeting, e.g. Leadership Council minutes in Peter's and Esther's folders.
