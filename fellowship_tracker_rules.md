# Fellowship & Award Tracker — Editing Rules & Conventions

## Data Sources

- **Primary**: Official fellowship/program page (e.g., nsfgrfp.org, research.google, amazon.science)
- **Deadline**: Program's "important dates" or "how to apply" page — deadlines shift annually by 1–4 weeks
- **Value/stipend**: Current program year announcement — amounts update annually
- **Truthfulness rule**: Use `~` prefix for approximate values and deadlines. Use `Varies` if genuinely inconsistent year-to-year. Use a range (e.g., `$30–50K`) if only a range is published. Never fabricate exact numbers.
- **Discontinued programs**: Mark as `⚫ Inactive` in Notes; do not delete until confirmed gone for 2+ years

---

## Formatting Rules

### Main Fellowship Tables

- **Column order**: `Fellowship | Provider | ~Deadline | Value | Duration | Nomination? | Eligibility | Research Fit | Notes`
- **Sorted by**: Approximate annual deadline month (Jan → Dec) within each category section
- Fellowship names are **bold + linked**: `[**NSF GRFP**](https://www.nsfgrfp.org)`
- All deadlines prefixed with `~` (all are approximate recurrences)
- Deadline format: month-based (e.g., `~Mid-Oct`, `~Late Aug`) — write specific dates only if confirmed for current cycle
- Use `—` when a field is not applicable

### Research Fit Column

- Short comma-separated tags only: `ML, VLM, LLM, UQ, Agents, CV, Safety`
- Only include tags with genuine fit — don't pad

### Upcoming Deadlines Section

- Show fellowships with deadlines within **90 days** of today
- Columns: `Fellowship | ~Deadline | ~Days Away | Action Needed`
- Recalculate on each update; remove rows as deadlines pass

### Relevance Map

- One row per fellowship (industry + federal + foundation; omit conference awards)
- Columns: `ML | VLM | LLM | UQ | Agents | CV`
- `✓✓` = primary/strong fit · `✓` = relevant · `—` = not a focus area

---

## Update Procedure

1. Set `Last updated` in the header to today's date (`YYYY-MM-DD`)
2. Recalculate **Upcoming Deadlines**: update days-away counts, remove past deadlines
3. Verify announced current-cycle deadlines and replace `~Month` with confirmed date if available
4. Update **Value** fields after new cohort announcements (stipends adjust with inflation)
5. Check for **new programs** — major AI labs (Anthropic, OpenAI, DeepMind) occasionally launch fellowship programs; add if relevant
6. Mark `⚫ Inactive` for programs with no activity after 2+ years; note in update comment

---

## Category Definitions

| Category | Description |
|----------|-------------|
| **Industry / Big Tech** | Company-funded fellowships (Google, Meta, Microsoft, etc.); typically include mentorship or internship |
| **Federal / Government** | US federal agency programs (NSF, DOE, DoD); most require US citizenship or PR |
| **Foundation / Independent** | Non-profit and private foundation programs (Hertz, Open Phil, Jane Street); academic-freedom-oriented |

---

## Fields Reference

| Field | Rules |
|-------|-------|
| **Fellowship** | Bold + hyperlinked to official program page |
| **Provider** | Short sponsor name (Google, NSF, Hertz Foundation, etc.) |
| **~Deadline** | Approximate annual deadline. Always prefix `~`. Two cycles → list both (e.g., `~May, ~Nov`) |
| **Value** | Stipend + key extras. Format: `$XK/yr stipend + tuition + [internship/travel/etc]`. Use `~` for estimates |
| **Duration** | How long support lasts (e.g., `2 yrs`, `Up to 5 yrs`) |
| **Nomination?** | Either `Self-apply` or `[Who] nominates [limit]` (e.g., `University nominates ≤3`) |
| **Eligibility** | Key gates: citizenship requirement, PhD year range, institution restrictions |
| **Research Fit** | Comma-separated tags from: `ML, VLM, LLM, UQ, Agents, CV, Safety` |
| **Notes** | Strategic context: competitiveness, research fit framing, special variants, process notes |

---

## Eligibility Flags

Always note these explicitly in the Eligibility column:

- **Citizenship**: Write `US citizen/PR` when required. Write `Open to all nationalities` when explicitly confirmed
- **PhD year restriction**: Note if there is an upper or lower year bound (e.g., `PhD years 2–3`, `PhD year 1–2 only`)
- **Institution-specific**: Write `[School] students only` for programs locked to specific universities (Stanford HAI, Harvard Kempner, CMU GAANN, Berkeley EECS Amazon, UW Allen School) — these do not apply while at UF
- **Team vs. individual**: Note `Team of 2 PhD students` in Nomination column when team-based (e.g., Qualcomm)

---

## NSF GRFP Special Rule

NSF GRFP has a strict eligibility window that must be tracked carefully:
- PhD students can apply **at most twice total** (once as a senior undergrad + once in PhD year 1 or year 2)
- After PhD year 2, permanently ineligible
- This makes it the **highest-priority early-PhD application** — flag prominently and track whether it has been applied to

---

## Special Program Notes

- **Open application fellowships** (no nomination barrier): Meta PhD Fellowship, NVIDIA Graduate Fellowship, NSF GRFP, DOE CSGF, NDSEG, SMART, Hertz, Open Phil, Two Sigma, Jane Street — these should be noted as `Self-apply` in the Nomination column
- **DOE CSGF practicum**: Mandatory 3-month DOE lab stay is non-negotiable; ensure applicant is prepared for that commitment
- **Open Philanthropy framing**: Their priority is "potential risks from advanced AI" — robustness, hallucination, reliability, and uncertainty-aware systems should be framed in those terms for applications
