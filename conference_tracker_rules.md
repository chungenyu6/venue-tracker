# Conference Tracker — Editing Rules & Conventions

## Data Sources

- **Primary**: Search the official conference website directly (e.g., `neurips.cc`, `icml.cc`, `eccv.ecva.net`)
- **Fallback**: Web search for "[Conference Name] 2026 important dates" or "[Conference Name] 2026 call for papers"
- **Truthfulness rule**: Only enter a date if it was found online. Use `TBD` if the date is genuinely not announced yet. Never fabricate or estimate a specific date for the main table (approximate `~` dates are allowed only in the Workshop Table).
- Always check the **official site** — third-party trackers can lag or be wrong

---

## Formatting Rules

### Main Conference Table
- **Column order**: `Est. Month | Status | Conference | Abstract | Full Paper | Conf Date | Location | Tier | Notes`
- **Sorted by**: Historical abstract deadline month (Jan → Dec), ascending
- Conference names are **bold + linked**: `[**NeurIPS 2026**](https://neurips.cc/Conferences/2026)`
- Use `—` (em dash) when a field is not applicable (e.g., no abstract deadline, no edition this year)
- Use `TBD` when the field applies but the date has not been announced yet

### Workshop Table
- **Column order**: `Est. Month | Status | Workshop @ | Full Paper | Workshop Date | Location | Notes`
- **No** Abstract, Notification, or Tier columns
- **One row per host conference** — do not list individual workshops
- Use `~` prefix for approximate dates (e.g., `~Apr 24, 2026`) since workshop deadlines vary by ±1–2 weeks
- **Sorted by**: Est. Month (Jan → Dec), same as main table

### Upcoming Section
- **Next 3 Submission Deadlines — Main Conferences**: top 3 upcoming abstract/full-paper deadlines from the main table, with days-left count relative to today
- **Next 3 Submission Deadlines — Workshops**: top 3 upcoming workshop paper deadlines, same format
- **Conferences Happening Soon**: top 3 closest conference start dates pulled directly from the main table; recalculate days-left each update

---

## Update Procedure

1. Set `Last updated` in the header to today's date (`YYYY-MM-DD`)
2. Re-check status badges for all rows (deadlines pass, new announcements go up)
3. Recalculate "Days Left" in the Upcoming section based on today's date
4. Recalculate "Conferences Happening Soon" — always the 3 nearest `Conf Date` values from the main table
5. For any `TBD` entry, search the official site to see if dates have been announced
6. When adding a new conference, also add a row to the **Relevance Map**

---

## Badge / Status Logic

| Badge | Meaning | When to use |
|-------|---------|-------------|
| 🟡 Upcoming | Submission deadline within ~60 days; official dates confirmed | Deadline is close and confirmed |
| 🔵 Future | Conference website exists but submission dates not yet announced | Website up, no dates yet |
| 🔴 Closed | Submission deadline has passed | Past the full-paper deadline |
| ⚫ No Edition | Conference not held this cycle (biennial / alternating) | e.g., ICCV in even years, ECCV in odd years |

- Do **not** use a 🟢 Open badge — it was removed
- Do **not** use `*` suffix markers — they were removed in favor of explicit Tier column

---

## Fields per Conference

### Main Table Fields

| Field | Rules |
|-------|-------|
| **Est. Month** | Historical month when abstract deadline typically falls; used for sort order |
| **Status** | One of the four badges above |
| **Conference** | Bold + hyperlinked name; include year |
| **Abstract** | Official abstract deadline date, or `—` if no abstract deadline, or `TBD` if not announced |
| **Full Paper** | Official full paper deadline, or `TBD` |
| **Conf Date** | Conference start–end date range, or `TBD` |
| **Location** | City, Country/State abbreviation |
| **Tier** | CORE 2023 rank: `A*`, `A`, `B`, or `—` if not ranked (new/systems conf) |
| **Notes** | Special info: ARR submission system, biennial pattern, tracks, dual cycles, etc. |

### Workshop Table Fields

| Field | Rules |
|-------|-------|
| **Est. Month** | Month when workshop paper deadline typically falls |
| **Status** | Same badge logic as main table |
| **Workshop @** | Linked as `[HostConf Workshops](url)` |
| **Full Paper** | Approximate deadline with `~` prefix; `TBD` if unknown |
| **Workshop Date** | Approximate date with `~` prefix if not confirmed |
| **Location** | Same as host conference |
| **Notes** | e.g., "Suggested deadline", deadline variation notes |

### Relevance Map
- One row per conference
- Columns: `Vision | NLP/LLM | UQ | Robotics | General ML | ML Systems`
- `✓✓` = primary venue, `✓` = relevant track, `—` = not a focus area
- Every conference in the main table must have a corresponding row here

---

## Conference Tier Reference (CORE 2023)

| Tier | Examples |
|------|---------|
| A* | NeurIPS, ICML, ICLR, CVPR, ECCV, AAAI, IJCAI, ACL, EMNLP, NAACL, KDD, ICRA |
| A | UAI, AISTATS, IROS, ECML-PKDD, AAMAS, CoRL |
| B | WACV, BMVC |
| — | COLM (new, est. 2024), MLSys (systems, not in CORE AI/ML), MILCOM (IEEE defense) |

## Special Conference Notes

- **ECCV**: even years only; **ICCV**: odd years only → use ⚫ No Edition for off-years
- **ACL / EMNLP / NAACL**: use ACL Rolling Review (ARR) system — note in the Notes column
- **KDD**: two submission cycles per year (Cycle 1 ~Jul, Cycle 2 ~Feb)
- **WACV**: two rounds per year (~Jul and ~Sep)
- **MILCOM**: IEEE Comms/Defense conference; has classified and unclassified paper tracks
- **COLM**: new conference (est. 2024), LLM-specific, not yet in CORE rankings
