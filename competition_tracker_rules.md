# Competition Tracker — Editing Rules & Conventions

## Scope

This tracker covers **competitions, challenges, grand challenges, hackathons, and benchmark leaderboards** relevant to a PhD researcher in AI/ML (LLMs, VLMs, UQ, agents, robustness). It excludes undergraduate-only events, paper submission deadlines (use `conference_tracker.md`), and fellowship applications (use `fellowship_tracker.md`).

---

## Data Sources

- **Primary**: Official competition page (e.g., `arcprize.org`, `swebench.com`, `mlcommons.org`)
- **Fallback**: Organizer lab or conference page, Kaggle competition listing, Devpost
- **Truthfulness rule**: Use `~` prefix for approximate dates. Use `TBD` if dates are not yet announced. Never fabricate prize amounts — use a range (e.g., `$50–100K`) if only a range is published. Use `Varies` if inconsistent year-to-year
- **Discontinued events**: Mark `⚫ Inactive` in Notes; do not delete until confirmed gone 2+ years

---

## Category Definitions

| Category | Description |
|----------|-------------|
| **Research / Academic** | Competitions hosted or co-located with major AI conferences (NeurIPS, ICML, CVPR, ICLR, COLM, etc.). Primary value: research visibility, publication, academic prestige |
| **Industry / Engineering** | Standalone competitions from companies or industry bodies (ARC Prize, Kaggle, MLPerf, SWE-bench, AWS). Primary value: prize money, industry recognition, engineering depth |
| **Summit / Retreat / Hackathon** | In-person events combining talks, networking, and hands-on building. Value: exposure, community, real-time collaboration |
| **Leaderboard / Benchmark** | Continuous submission-based leaderboards (Open LLM, HAL, GAIA). Value: research visibility, publication anchor, ongoing community recognition |

---

## Formatting Rules

### Main Competition Tables

- **Column order**: `Competition | Organizer | ~Timing | Prize / Recognition | Format | Eligibility | Research Fit | Notes`
- **Sorted by**: Approximate annual deadline or event date (Jan → Dec) within each category section
- Competition names are **bold + linked**: `[**ARC Prize**](https://arcprize.org)`
- Dates prefixed with `~` (approximate recurrences) unless a confirmed date is listed
- Use `—` when a field is not applicable
- Use `TBD` when it applies but is not yet announced

### Research Fit Column

- Short comma-separated tags only: `ML, VLM, LLM, UQ, Agents, CV, Safety, Systems`
- Only include tags with genuine fit — don't pad

### Upcoming Section

- Show competitions with registration or submission deadlines within **60 days** of today
- Columns: `Competition | ~Deadline | ~Days Away | Action Needed`
- Recalculate on each update; remove rows as deadlines pass

### Relevance Map

- One row per competition
- Columns: `ML | VLM | LLM | UQ | Agents | CV | Systems`
- `✓✓` = primary/strong fit · `✓` = relevant · `—` = not a focus area

---

## Update Procedure

1. Set `Last updated` in the header to today's date (`YYYY-MM-DD`)
2. Recalculate **Upcoming Deadlines**: update days-away counts, remove past deadlines
3. Verify confirmed current-cycle dates and replace `~Month` with confirmed date if available
4. Check for new competitions announced at NeurIPS, ICML, CVPR, ICLR workshop tracks
5. Check industry labs (Anthropic, OpenAI, Google DeepMind, Meta AI) for new challenge announcements
6. Mark `⚫ Inactive` for events with no activity after 2+ years
7. For leaderboard entries: verify the leaderboard is still actively maintained

---

## Badge / Status Logic

| Badge | Meaning |
|-------|---------|
| 🟡 Upcoming | Deadline or event within ~60 days; dates confirmed |
| 🔵 Future | Announced but deadline/date not yet set |
| 🔴 Closed | Registration / submission deadline has passed |
| ♻️ Continuous | Ongoing leaderboard — no fixed deadline |
| ⚫ Inactive | No activity in 2+ years; possibly discontinued |

---

## Fields Reference

| Field | Rules |
|-------|-------|
| **Competition** | Bold + hyperlinked to official page |
| **Organizer** | Short name (NeurIPS, Google DeepMind, Kaggle, MLCommons, etc.) |
| **~Timing** | Annual date or event month; `~` prefix unless confirmed. Continuous for leaderboards |
| **Prize / Recognition** | Dollar value + academic credit. Use `~` for estimates. `Community prestige` for no-cash recognition |
| **Format** | `Remote`, `In-person ([City])`, or `Hybrid`. For in-person, always name the city |
| **Eligibility** | Key gates: open to all, PhD students welcome, team vs. individual, institution restrictions |
| **Research Fit** | Comma-separated tags from: `ML, VLM, LLM, UQ, Agents, CV, Safety, Systems` |
| **Notes** | Strategic framing: difficulty, past winners, relevance to research, special tracks, submission quirks |

---

## Eligibility Flags

Always note these explicitly in the Eligibility column:
- **Team vs. individual**: Note `Team of N` when team-based (e.g., `Team of 2–5`)
- **Institution restriction**: Note `[School] only` if restricted to specific universities
- **Graduation level**: Note `PhD/PostDoc only` or `Grad students welcome` as appropriate
- **Registration requirement**: Note if separate registration is needed before participation

---

## Strategic Notes (Standing)

- **ARC Prize**: Hardest recurring AI research challenge; leaderboard-friendly for publishing novel reasoning methods
- **NeurIPS/ICML/CVPR competition tracks**: Win = invitation to workshop, extended abstract, or full paper at a top venue — treat as mini-publications
- **Kaggle**: Grandmaster track is long-term career-signal, not a one-off win; useful for engineering credibility
- **MLPerf**: Not a competition for individuals — only relevant if participating via a lab/team with hardware
- **Berkeley Agentic AI Summit**: Primarily a networking/exposure event, not a traditional competition — attend for community presence
- **SWE-bench / HAL / GAIA leaderboards**: Submitting a new agent method here is equivalent to a benchmark-track publication anchor
- Always verify dates on official sites — timelines shift 1–4 weeks year to year
