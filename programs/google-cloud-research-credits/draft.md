# Google Cloud Research Credits — Application draft

> Latest stable version (v4 with Computer Science field, Brazilian cost angle, "we already use Google API" emphasis). Iteration history in [`loop-log.md`](loop-log.md).
> **Valdemar Pinho Neto as Faculty applicant.** Credits go into FGV's GCP billing account.
> Pre-submission setup: GCP Billing Account ID at https://console.cloud.google.com/billing

---

## v4 (2026-05-24) — mapped to real form fields with corrections

### Identification fields

| Form field | Value |
|---|---|
| First name | **Valdemar** |
| Last name | **Pinho Neto** |
| Email | (Valdemar's @fgv.br institutional address — to fill) |
| Country | Brazil |
| State | Rio de Janeiro |
| Job Title | **Faculty** |
| Organization Name | Fundação Getulio Vargas — Escola de Pós-Graduação em Economia (EPGE/FGV) |
| Institution Type | University |
| Department | EPGE — Graduate School of Economics |

### Project name

**NOVO CR: Longitudinal Educational AI Infrastructure**

### Project start date

**December 2025** (Rubens Cysne, director of EPGE/FGV, encouraged formal start). The system has been ongoing in production since then; this grant supports the next 12 months of production-grade evaluation.

### Field of research

**Computer Science**

### Intended credit application

**Evaluation / Comparison** (multi-provider benchmark of Gemini against Anthropic Claude and OpenAI GPT-5 family at each pipeline stage)

### External funding source status

No external funding currently. Submission planned to the Brazilian CNPq Jovem Cientista Prize 2026 (Track 3: AI and Education), deadline July 31, 2026.

### Prior cloud infrastructure use / Prior Google Cloud use

**We already use Google's Gemini API in production.** Specifically, Gemini 3 Flash and Gemini 2.5 Flash are configured as one of three parallel providers in the NOVO CR's six-stage pipeline. Production cost measurements (2026-05-23 audit):

- Gemini 3 Flash full pipeline (one student exam): ~$0.19
- Gemini 3 Flash extract-only stage: ~$0.0012 (2,040 input / 507 output tokens)
- Google-side total across 28 production runs: $0.49

The NOVO CR system has not consumed prior Google Cloud research credits. We use Render for hosting, Supabase for database/storage, and E2B for code execution — Google Cloud usage is currently scoped to Gemini API access.

### Post-expiration funding plan

After the 12-month grant period, project continuity is supported by: (a) pursuit of CNPq Jovem Cientista funding for 2027 research activities; (b) structural cost reductions achieved during the grant through engineered prompt caching at the correction stage (~89% input-token reduction projected); (c) pilot deployment paths through FGV's CTAE school in 2027; (d) institutional support discussions with EPGE leadership.

### Expected costs (via pricing calculator)

[Pricing calculator URL to be generated at submission via https://cloud.google.com/products/calculator — see REVIEW.md pendency.]

Rough internal estimate based on production measurements:
- Per-pipeline Gemini Flash: ~$0.19 per student exam
- Anticipated grant-period usage: ~5,000–10,000 exam-equivalents across benchmarking and pilot deployment
- Range: ~$950–$2,000 in Gemini API spend, depending on per-stage configuration

### Google Cloud Billing Account ID

[Max 25 characters. To be obtained via EPGE/FGV institutional channels (TI or financial department), or via creating a new institutional billing account under Valdemar's representation. See REVIEW.md pendency.]

---

## Proposal (≤ 250 words)

> The core artifact. Must include: research problem, GCP tools, project timeline, key milestones and outcomes, and how GCP can support the research in the future.

---

Educational data on a single student is fragmented across institutional silos: schools hold grades and attendance, child welfare councils hold reports, the juvenile justice system holds socio-educational measures. NOVO CR (https://ia-educacao-v2.onrender.com), ongoing since December 2025, is a longitudinal data infrastructure for AI-assisted educational assessment, running in production with 26 subjects, 100+ processed activities, and three providers (Anthropic, OpenAI, Google) integrated in parallel. A real 7-page cross-course report covering 9 disciplines across 4 years of one student's trajectory has already been produced as proof of concept.

We already use Gemini in production: per-pipeline cost ~$0.19 with Gemini 3 Flash; Google-side total across 28 measured runs is $0.49. GCP credits would fund production-scale evaluation of Gemini against alternatives at each of six pipeline stages, plus build the missing batch pipeline for the cross-course longitudinal report (currently chat-only). Sustained API usage is needed to engineer per-stage selection rigorously and to validate prompt caching (~89% input-token reduction projected at the correction stage).

Timeline (12 months): months 1–3, provider benchmark per stage; months 4–6, batch pipeline for cross-course report; months 7–9, pilot deployment in FGV K–12 school (CTAE); months 10–12, municipal Rio de Janeiro network evaluation via SUBDEIS.

Outcomes: per-stage benchmark report, working batch longitudinal pipeline, FGV pilot deployment, submission to CNPq Jovem Cientista Prize 2026. Brazilian researchers face structural API cost disadvantages; the grant unblocks scientific rigor.

---

**Word count (counted):** ~245 words. Under 250 limit. ✓

---

(v4 stable — Computer Science field, Brazilian cost angle, "we already use Google" emphasis. Pre-submission pendencies: billing account institutional access + pricing calculator URL + Valdemar's institutional email.)
