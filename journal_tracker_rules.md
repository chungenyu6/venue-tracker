# Journal Tracker — Editing Rules & Conventions

## Data Sources

- **Primary**: Official journal page (publisher site — Springer, Elsevier, IEEE, ACM, MIT Press)
- **Impact Factor**: Journal Citation Reports (JCR) — published annually in June by Clarivate; use the most recent JCR year
- **SJR**: SCImago Journal Rank — https://www.scimagojr.com/
- **CiteScore**: Scopus — https://www.scopus.com/sources
- **h5-index**: Google Scholar Metrics — https://scholar.google.com/citations?view_op=top_venues
- **APC (Article Processing Charge)**: Publisher's current "Author Services" or "Open Access" page — prices change annually
- **Indexing**: Verify on DOAJ, MathSciNet, Scopus, Web of Science (WoS/SCIE) directly
- **Truthfulness rule**: Only enter a metric if found from a primary source. Use `—` if not applicable, `TBD` if not yet announced, `~` prefix for estimates. Never fabricate.
- **New journals** (< 2 years old): IF and SJR will not exist yet — write `— *(new)*` instead of leaving blank

---

## Formatting Rules

### Main Journal Tables

- **Column order**: `Journal | Publisher | IF (year) | SJR | h5 | CiteScore | APC (USD) | Indexing | Notes`
- **Sorted by**: Impact Factor descending within each category section
- Journal names are **bold + linked**: `[**TPAMI**](https://computer.org/csdl/journal/tp)`
- Priority journals get a ⭐ suffix after the link: `[**JMLR**](https://jmlr.org) ⭐`
- Use `—` when a field is not applicable (e.g., no APC for Diamond OA journals → still write `$0` in APC column for clarity)
- Use `— *(new)*` for metrics unavailable due to journal being newly launched
- Use `~` prefix for estimated/approximate values (e.g., `~$3,900`)
- APC column always in USD; add `~` if converted from GBP/EUR

### Priority Journals Section

- List all ⭐-marked journals in the "Priority Journals at a Glance" table at the top
- Columns: `Journal | Category | IF (2024) | APC (USD)`
- Link the journal name to the official journal homepage using bold format (e.g., `[**JMLR**](https://jmlr.org)`)

### Relevance Map

- One row per journal — must match every journal in the full table
- Columns: `Vision/VLM | NLP/LLM | UQ | Robotics | General ML | Agents`
- `✓✓` = primary/top venue for that area · `✓` = relevant track · `—` = not a focus area

---

## Update Procedure

1. Set `Last updated` in the header to today's date (`YYYY-MM-DD`)
2. **Impact Factor**: JCR releases annually each June — update the IF year label and all values after each release
3. **APCs**: Check publisher pages annually; prices typically change Jan 1. Note the year if price is from a previous year
4. **SJR / CiteScore**: Update from Scimago and Scopus after their annual release (typically Q1)
5. **h5-index**: Google Scholar Metrics updates periodically — verify and refresh
6. **Indexing**: When a new journal gains SCIE or Scopus coverage, update the Indexing column and add a note
7. **New journals**: Add to the appropriate category section and to the Relevance Map. Mark metrics `— *(new)*` until indexed
8. **Priority mark (⭐)**: Only assigned manually based on personal research priorities — do not add or remove without user direction

---

## OA Model Definitions

| OA Model | Meaning | APC? | Free to Read? |
|----------|---------|------|---------------|
| Diamond | Free to publish AND free to read | $0 | Yes |
| Gold OA | APC required; paper freely readable | Yes | Yes |
| Hybrid | Subscription journal; optional Gold OA via APC | Optional | Only if APC paid |
| Subscription | Traditional subscription model; no OA option | $0 to publish | Institutional access only |

- For Hybrid journals: note whether Green OA (arXiv self-archiving) is allowed and any embargo period
- ACM journals transitioning to Gold OA Jan 2026 — update model accordingly

---

## Fields Reference

| Field | Rules |
|-------|-------|
| **Journal** | Bold + hyperlinked to official journal homepage. Add ⭐ after link for priority journals. |
| **Publisher** | Short publisher name (IEEE, Elsevier, Springer, ACM, MIT Press, SIAM/ASA, AI Access Foundation, MLR Press) |
| **IF (year)** | Impact Factor from JCR; include year in column header (e.g., `IF (2024)`). Use range (e.g., `4.0–5.9`) only if sources genuinely conflict. |
| **SJR** | SCImago Journal Rank score (not quartile — the numeric score). Q1/Q2 context in Notes if relevant. |
| **h5** | h5-index from Google Scholar Metrics (5-year h-index). |
| **CiteScore** | Scopus CiteScore (4-year average citations per document). |
| **APC (USD)** | Article Processing Charge in USD. `$0` for Diamond/Subscription. `~` if estimated. `Inst. covered` if typically paid by university subscription. |
| **Indexing** | List coverage: SCIE, Scopus, DBLP, DOAJ, ACM DL, MathSciNet. |
| **Notes** | Strategic context: scope, bar for acceptance, community, special model (e.g., ARR, conference-companion), review time if known. |

---

## Journal Tier Reference

Informal research-community tiers (no single official ranking like CORE for conferences):

| Tier | Journals |
|------|---------|
| Elite | Nature Machine Intelligence, TPAMI, JMLR |
| Top | TMLR, TACL, CL, IJCV, TIP, TNNLS, EAAI, ACM TIST |
| Strong | AIJ, JAAMAS, T-RO, JAIR, Neurocomputing, ACM TOPML |
| Solid | JUQ, IJAR, DMLR, Neural Computation, MLWA |

- These tiers reflect community perception for AI/ML/Vision/NLP — not formal rankings
- Do not add this tier column to the main table; use for internal guidance only

---

## Special Journal Notes

- **TACL + CL**: Both published by MIT Press / ACL. TACL has a hybrid journal+conference model (accepted papers present at ACL/EMNLP). CL is traditional journal format.
- **TMLR**: Uses OpenReview with transparent review. Cannot reject for "lack of novelty" — only correctness and soundness matter. No volume/issue constraints.
- **JMLR family**: JMLR, TMLR, DMLR all use MLR Press / Microtome. All Diamond OA, all $0 APC.
- **ACM journals (TOPML, TIST)**: ACM transitioning to 100% Gold OA by Jan 2026. Waivers available for 1,800+ participating institutions and low-income countries — always check before assuming out-of-pocket cost.
- **IEEE Hybrid journals (TPAMI, TIP, TNNLS, T-RO)**: Free to publish under subscription model; OA version costs the APC. Green OA via arXiv generally permitted.
- **Elsevier journals (AIJ, EAAI, IJAR, Neurocomputing, MLWA)**: Green OA allowed via author's accepted manuscript on arXiv, typically after 12-month embargo.
- **Nature Machine Intelligence**: Extremely high APC (~$12,850 USD). Check if your institution has a Springer Nature Transformative Agreement (many universities have this — reduces or eliminates APC).
- **DMLR**: Purpose-built for data contributions. Treats datasets, benchmarks, and data governance as first-class scientific contributions.
- **JUQ**: SIAM journals are typically covered by institutional library subscriptions — no out-of-pocket APC expected.
- **JAIR**: One of the few journals that publicly discloses acceptance rates (~11% overall). Non-profit, Diamond OA since 1993.
