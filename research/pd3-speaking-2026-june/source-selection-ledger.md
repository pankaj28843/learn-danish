# Source Selection Ledger

Updated: 2026-05-25T13:14:58Z

## CDP Mode

The user requested headed CDP. Preflight was saved at `research/pd3-speaking-2026-june/cdp-headed-preflight.txt`.

Observed status:

- `cdp --help` succeeded.
- `cdp --browser-mode headed browser mode get --json` selected headed mode.
- `cdp --browser-mode headed daemon health --json` reported healthy.
- Headed SERP and extraction workflows were used.

## Query Set

Query file: `tmp/research-web-critical/pd3-speaking-2026-june/queries.txt`

Query families:

- Official format and dates.
- PD3 oral topics and learner experience.
- Danish language-school preparation material.
- Denmark/Danish/NewToDenmark Reddit threads.
- Danish and English search terms for "mundtlig", "speaking", "emner", and "experience".

## Search Engines

| Engine | Result | Evidence |
|---|---:|---|
| Google, headed | 160 candidates | `tmp/research-web-critical/pd3-speaking-2026-june/serp-google/candidates.json` |
| DuckDuckGo, headed | 114 candidates | `tmp/research-web-critical/pd3-speaking-2026-june/serp-duckduckgo/candidates.json` |
| Bing, headed | Degraded: only Microsoft privacy result | `tmp/research-web-critical/pd3-speaking-2026-june/serp-bing/candidates.json` |

## Extracted Sources

Primary extraction summary: `tmp/research-web-critical/pd3-speaking-2026-june/pages/extract-summary.json`

Additional Prøvebanken extraction summary: `tmp/research-web-critical/pd3-speaking-2026-june/proevebanken-pages/extract-summary.json`

PDF repair:

- `research/pd3-speaking-2026-june/sources/datoer-og-frister-s26.pdf`
- `research/pd3-speaking-2026-june/sources/datoer-og-frister-s26.txt`
- `research/pd3-speaking-2026-june/sources/mundtlig-pd3-instruktion-til-kursister.pdf`
- `research/pd3-speaking-2026-june/sources/mundtlig-pd3-instruktion-til-kursister.txt`

## High-Weight Sources

| Source | Why selected | Local artifact |
|---|---|---|
| Dansk og Prøver, PD3 content and level | Official SIRI/UIM description of format and official examples | `pages/002-danskogproever.../page.md` |
| Dansk og Prøver, 2026 deadline news | Official June 2026 date evidence | `pages/003-danskogproever.../page.md` |
| Dansk og Prøver dates PDF | Official detailed 2026 operational timeline | `sources/datoer-og-frister-s26.txt` |
| Studieskolen PD3 page | Exam-center confirmation of June 2026 oral period and logistics | `pages/005-www-studieskolen.../page.md` |
| UCplus PD3 page | Exam-center confirmation of June 2026 oral period and prep context | `pages/006-ucplusdansk.../page.md` |
| Clavis PD3 info | Concise timing breakdown: 15 min including grading, 2+3 min and 10 sec+4.5 min | `pages/007-www-clavis.../page.md` |
| Prøvebanken DAU3 | Official archive proves recent oral materials exist for 2024, 2023, 2022, but PDFs require UNI-login/copyright constraints | `pages/027-www-xn-prvebanken.../page.md` and `proevebanken-pages/` |

## Medium-Weight Sources

| Source | Why selected | Local artifact |
|---|---|---|
| Learn Danish oral review | Learner experience with concrete topics: alternative punishment and volunteer work | `pages/010-www-learn-danish...review.../page.md` |
| Life in Aalborg oral review | Learner experience and historical topic examples: alternative energy, tourism, drinking habits, environment, cycling culture | `pages/011-lifeinaalborg.../page.md` |
| Last Week in Denmark oral guide | 2026-facing course/blog guidance with topic examples: social media, youth finance, retirees, stress/workplace, changing jobs | `pages/012-lwid.../page.md` |
| Learn Danish Lab PD3 guide | Practice topic inventory around work, health, climate, education, integration, housing, technology | `pages/013-learndanishlab.../page.md` |
| Dit Dansk self-study and blog | Teacher/course marketing signal that PD3 prep is topic-heavy and society-topic driven | `pages/017-pd3-ditdansk.../page.md`, `pages/018-www-ditdansk.../page.md` |
| AB Danish PD3 page | Language-school framing of expected society topics: democracy, welfare, pensions, public/private sector | `pages/015-abdanish.../page.md` |

## Community Sources

| Source | Use | Local artifact |
|---|---|---|
| r/Danish PD3 Speaking | Preparation pain points: formal speaking, grammar, speaking groups | `pages/023-www-reddit...pd3-speaking/page.md` |
| r/Danish PD3 Modules/Exam | Success stories and timeline caveats | `pages/024-www-reddit...pd3-modulesexam/page.md` |
| r/NewToDenmark PD3 module requirement | Eligibility and value of module 5/class preparation | `pages/026-www-reddit...prove-i-dansk-3.../page.md` |
| r/Denmark PD3 examples 2004-2019 | Archive-seeking signal only, not content evidence | `pages/025-www-reddit...pd-3-examples.../page.md` |

## Rejected or Weak Sources

- Facebook group posts appeared in SERP, but extraction/auth is unreliable and not needed for core conclusions.
- YouTube titles were useful discovery signals, but transcript extraction was not run in this timebox. Titles are treated as weak corroboration only.
- Scribd documents appeared in SERP but were not used as evidence because access and copyright status are unclear.
- Prøvebanken material PDFs are behind UNI-login and carry explicit usage restrictions. The public archive page is used only to prove that official recent materials exist.
