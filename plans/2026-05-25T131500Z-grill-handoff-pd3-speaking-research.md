# PRP Grilling Handoff: PD3 Speaking June 2026 Research Package

## One-sentence goal

Create a local, evidence-backed PD3 speaking-test research package with topic inventory, June 2026 prediction, PRP/living plan, and chapterwise study material.

## Decisions made

| Decision | Answer | Source |
|---|---|---|
| Research source type | Web-first, no GitHub/HN, include Danish subreddits, blogs, schools, official pages | User objective |
| Browser mode | Use headed CDP | User follow-up and `research/pd3-speaking-2026-june/cdp-headed-preflight.txt` |
| Output location | Keep everything in this workspace | User objective |
| Exact-topic claims | Do not claim unreleased June 2026 topics are public; produce a probability-ranked preparation map | Evidence audit |
| Study structure | Five chapter folders: format, inventory, prediction, playbook, practice bank | User asked chapterwise folder, "think study-enrich" |

## Assumptions to validate

| Assumption | Validation gate | Counterexample |
|---|---|---|
| Exact June 2026 topics are not publicly available | Search/extraction ledger includes official and community sources but no public exact list | A newly published official/public source contains exact topics |
| Official format is stable for June 2026 | Dansk og Prøver and exam-center pages agree on 2026 dates and format | SIRI changes oral format before 10 June 2026 |
| Topic prediction should favor recurring societal topic families | Topic inventory traces each cluster to at least one source | A source shows June 2026 is specialized around a narrow theme |

## Non-goals

- Do not bypass Prøvebanken login or protected material restrictions.
- Do not use GitHub or Hacker News.
- Do not present predictions as leaked or guaranteed topics.
- Do not commit or push anything; this is not a git repo.

## Acceptance criteria

- [x] Local `AGENTS.md` exists.
- [x] Headed CDP preflight and `cdp --help` output are saved.
- [x] Source ledger records search engines, extracted pages, and limitations.
- [x] Topic inventory lists official, historical, school-prep, and community-derived topic families.
- [x] June 2026 prediction ranks topics by likelihood and labels uncertainty.
- [x] PRP/living plan exists with "Do next steps" and "What else remains".
- [x] Chapterwise study folder exists with meaningful learner-facing material.

## Risks and mitigations

| Risk | Mitigation | Evidence needed |
|---|---|---|
| Overstating predictions | Use probability labels and caveats | `prediction-june-2026.md` |
| Weak community evidence | Treat Reddit as preparation sentiment, not official topic proof | Source ledger |
| Protected material | Use Prøvebanken page metadata only; do not scrape logged-in PDFs | Prøvebanken extraction |
| Stale source data | Timestamp every artifact and keep raw extraction paths | Source ledger and PRP snapshot |

## Recommended /plan-prp input

Build and maintain a local PD3 speaking research and study package for the June 2026 exam period. Use headed CDP web research only, no GitHub/HN. Produce source-backed topic inventory, probability-ranked prediction, and chapterwise study material in this folder. Preserve uncertainty around unreleased exact topics and keep the living PRP synced with artifacts.

## Readiness

Ready for `/plan-prp`.
