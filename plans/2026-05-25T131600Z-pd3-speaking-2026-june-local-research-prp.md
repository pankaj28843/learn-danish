# PD3 Speaking June 2026 Local Research PRP

## Plan Operator Contract ("Do next steps")

When the user says **"Do next steps"**:

1. Always open/re-check **this plan file** first.
2. "Next steps" = the next incomplete checkbox items in **Implementation Blueprint**, starting from the earliest incomplete phase.
3. If unsure what to do next, recheck `## What else remains?` and resume from the topmost unfinished item.
4. After each chunk of work, update this plan:
   - Add/refresh a Status Snapshot entry, newest first.
   - Update checkboxes.
   - Update blockers/risks and `## What else remains?`.
5. If all items are complete, run the validation loop and record results.

## Status Snapshot (2026-05-25T13:18:30Z)

- Current phase/step: Phase 4 complete; validation finished.
- Repo reconciliation: `/Users/pankaj/Personal/Code/learn-danish` is not a git repo; artifacts are local files.
- Ralph-loop result: `COMPLETE`.
- Iterations run:
  - Iteration 1: initialized local rules and research scaffold.
  - Iteration 2: ran headed CDP web research and PDF text repair.
  - Iteration 3: wrote source ledger, synthesis, topic inventory, and June 2026 prediction.
  - Iteration 4: wrote five chapterwise study pages and validated artifact coverage.
- Commands/evidence run:
  - `find research study plans -maxdepth 3 -type f | sort` listed the expected research, study, and plan files.
  - `rg -n "headed|DuckDuckGo|Google|10.*23.*juni|10-23 June|June 2026|not public|probability|probabilistic|not an official list" research study plans` found required source and uncertainty markers.
  - `jq -r '.failures|length' tmp/research-web-critical/pd3-speaking-2026-june/pages/extract-summary.json` returned `0`.
  - `jq -r '.failures|length' tmp/research-web-critical/pd3-speaking-2026-june/proevebanken-pages/extract-summary.json` returned `0`.
  - `find study -mindepth 2 -name README.md | sort | wc -l` returned `5`.
- Files changed since last snapshot: final research files, study chapters, and this PRP update.
- Blockers: none.
- Exact next action: optional future enrichment only, such as YouTube transcript extraction or authenticated Facebook group review if the user wants more evidence.

## Status Snapshot (2026-05-25T13:14:58Z)

- Current phase/step: Phase 3 complete; final validation pending.
- Repo reconciliation: `/Users/pankaj/Personal/Code/learn-danish` is not a git repo; artifacts are local files.
- Files changed since last snapshot: `AGENTS.md`, `research/pd3-speaking-2026-june/*`, `study/*/README.md`, this plan, grill handoff.
- Commands/evidence run:
  - `cdp --help` and headed CDP preflight saved to `research/pd3-speaking-2026-june/cdp-headed-preflight.txt`.
  - Headed Google SERP: 160 candidates.
  - Headed DuckDuckGo SERP: 114 candidates.
  - Headed Bing SERP degraded: one Microsoft privacy result.
  - Headed extraction: 27 selected pages, zero failures, PDF text repaired through local venv and `pypdf`.
  - Prøvebanken detail extraction: 5 pages, zero failures.
- Blockers: none. Limitation: exact June 2026 topics are not public; prediction is probabilistic.
- Exact next action: run validation checks over file existence and key text markers.

## Goal / Why / Success Metrics

- **Goal**: Build a local, source-backed PD3 speaking-test research package for June 2026 with topic inventory, predictions, and study chapters.
- **Why**: The user needs practical preparation guidance grounded in official format and real learner/school experience.
- **Success metrics**:
  - [x] Initialize project `AGENTS.md`.
  - [x] Use headed CDP and save `cdp --help` evidence.
  - [x] Save raw search/extraction artifacts locally.
  - [x] Produce grill handoff before PRP.
  - [x] Produce PRP/living plan in local folder.
  - [x] Produce chapterwise study folder.
  - [x] Run final validation and update this plan if anything is missing.

## Current State

- Existing behavior: empty workspace at start, no git repo.
- Key files:
  - `AGENTS.md`
  - `research/pd3-speaking-2026-june/source-selection-ledger.md`
  - `research/pd3-speaking-2026-june/synthesis.md`
  - `research/pd3-speaking-2026-june/topic-inventory.md`
  - `research/pd3-speaking-2026-june/prediction-june-2026.md`
  - `study/README.md`
- Constraints:
  - Local-only output.
  - No GitHub/HN.
  - Use headed CDP.
  - Do not bypass protected material.
- Risks:
  - Exact unreleased topics cannot be known.
  - Some community/social sources are noisy.

## Engineering Principles Pass

| Pattern | Where | Why | Verification |
|---|---|---|---|
| Source ledger first | `source-selection-ledger.md` | Keeps prediction traceable | File exists and names raw artifacts |
| Separate evidence from prediction | `topic-inventory.md`, `prediction-june-2026.md` | Prevents false certainty | Prediction file contains caveat |
| Chapterwise study material | `study/*/README.md` | Makes output usable for learning | `find study -name README.md` |

| Anti-pattern | Signal | Why it hurts | Safer move |
|---|---|---|---|
| Claiming leaked topics | "will definitely appear" | Misleads learner | Use probability/risk labels |
| Copying protected PDFs | Prøvebanken logged-in material | Copyright and access problem | Use public metadata only |
| Snippet-only research | SERP titles with no extraction | Weak evidence | Cite extracted pages and local artifacts |

## Formal Methods / Contracts Pass

| Property / invariant | Scope | How to check | Counterexample to guard against |
|---|---|---|---|
| Every prediction category traces to evidence | `prediction-june-2026.md` | Manual review against source ledger | A prediction appears with no source rationale |
| Exact topics are not presented as guaranteed | All synthesis/prediction files | `rg -n "guaranteed|leaked|definitely"` | User treats forecast as official list |
| Local-only output | Workspace files | `find . -maxdepth 3 -type f` | Artifacts saved outside this folder except temporary venv |

## Evidence-to-Change Matrix

| Proposed change | Local evidence | External evidence | Rejected alternative | Validation |
|---|---|---|---|---|
| Create local research package | Empty initial workspace | User objective | Save only chat answer | `find research study plans` |
| Use headed CDP | `cdp-headed-preflight.txt` | User follow-up | Headless CDP | Check preflight file |
| Predict topic families | Extracted pages and PDFs | Official/SIRI, schools, blogs, Reddit | Claim exact unreleased topics | `prediction-june-2026.md` caveats |

## Implementation Blueprint

### Phase 0 - Recon / alignment

- [x] Step 0.1 - Inspect workspace and project rules.
  - Files: `AGENTS.md`
  - Validation: `ls -la`

### Phase 1 - Research collection

- [x] Step 1.1 - Run headed CDP preflight and save help/health output.
  - Files: `research/pd3-speaking-2026-june/cdp-headed-preflight.txt`
  - Validation: file exists and mentions headed.
- [x] Step 1.2 - Run headed SERP sampling.
  - Files: `tmp/research-web-critical/pd3-speaking-2026-june/serp-*`
  - Validation: Google and DuckDuckGo candidate files exist.
- [x] Step 1.3 - Extract selected pages and PDFs.
  - Files: `tmp/research-web-critical/pd3-speaking-2026-june/pages/`, `research/pd3-speaking-2026-june/sources/`
  - Validation: extraction summaries report zero failures.

### Phase 2 - Synthesis

- [x] Step 2.1 - Write source ledger.
  - Files: `source-selection-ledger.md`
  - Validation: contains Google, DuckDuckGo, Bing, and PDF repair.
- [x] Step 2.2 - Write topic inventory.
  - Files: `topic-inventory.md`
  - Validation: contains official, historical, school/course topic families.
- [x] Step 2.3 - Write June 2026 prediction.
  - Files: `prediction-june-2026.md`
  - Validation: contains caveat and ranked categories.

### Phase 3 - Study package

- [x] Step 3.1 - Create chapterwise study index and chapters.
  - Files: `study/README.md`, `study/*/README.md`
  - Validation: five chapter folders exist.

### Phase 4 - Validation and handoff

- [x] Step 4.1 - Run final filesystem/text validation.
  - Files: all artifacts.
  - Validation: `find`, `rg`, and summary checks.
- [x] Step 4.2 - Update final status snapshot and handoff.
  - Files: this plan.
  - Validation: `## What else remains?` synced.

## Validation Loop

| Level | What | Command | Expected |
|---|---|---|---|
| 1 | Artifact existence | `find research study plans -maxdepth 3 -type f | sort` | Key files listed |
| 2 | Source markers | `rg -n "headed|DuckDuckGo|Google|10.*23.*juni|June 2026|not public|probability" research study plans` | Markers found |
| 3 | Extraction summary | `jq -r '.failures|length' tmp/research-web-critical/pd3-speaking-2026-june/pages/extract-summary.json` | `0` |
| 4 | Study chapters | `find study -mindepth 2 -name README.md | wc -l` | `5` |

## Open Questions & Risks

- Exact June 2026 topics are not public. Treat predictions as preparation priorities.
- If the user wants more depth, next research should target YouTube transcript extraction and Facebook group posts where accessible.

## Plan Watchers

- **Status cadence**: update after every research run, synthesis change, or validation failure.
- **Current blockers**: none.
- **Decision log**:
  - 2026-05-25T13:14:58Z - Use headed CDP, local-only artifacts, no GitHub/HN.

## What else remains?

- [x] Step 4.1 - Run final filesystem/text validation.
- [x] Step 4.2 - Update final status snapshot and handoff.
