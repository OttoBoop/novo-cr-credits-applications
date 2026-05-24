# Google Cloud Research Credits — Application draft

> Latest stable version. Iteration history in [`loop-log.md`](loop-log.md).
> The core artifact is the 250-word proposal (Google's strict limit). Supporting field content provided for the form's other fields.

---

## v3 (2026-05-24)

### Identification fields

| Form field | Value |
|---|---|
| First name | Valdemar |
| Last name | Pinho Neto |
| Email | (Valdemar's @fgv.br institutional address) |
| Country | Brazil |
| State | Rio de Janeiro |
| Job Title | **Faculty** |
| Organization Name | Fundação Getulio Vargas — Escola de Pós-Graduação em Economia (EPGE/FGV) |
| Institution Type | University |
| Department | EPGE — Graduate School of Economics |

### Project name

**NOVO CR: Longitudinal Educational AI Infrastructure**

### Project start date

[To be confirmed when submitting — proposal target: month following acceptance notification]

### Field of research

**Computer Science** (with applied research domain in education)

### Intended credit application

**Evaluation / Comparison** (multi-provider benchmark of Gemini against Anthropic and OpenAI models at each pipeline stage)

### External funding source status

No external funding currently. Submission planned to Brazilian CNPq Jovem Cientista Prize 2026 (Track 3: AI and Education), deadline July 31, 2026.

### Prior cloud infrastructure use / Prior Google Cloud use

The NOVO CR system runs on Render (hosting), Supabase (database), and E2B (code execution). Google Cloud is currently used only through Gemini API access (no direct GCP infrastructure beyond API). Prior Google Cloud credits: none.

### Post-expiration funding plan

After the 12-month grant period, project continuity is supported by: (a) pursuit of CNPq Jovem Cientista funding for 2027 research activities; (b) structural cost reductions achieved during the grant through prompt-caching benchmarks established with Gemini; (c) pilot deployment revenue paths through FGV's CTAE school (2027 target); (d) institutional support discussions with EPGE leadership.

### Expected costs (via pricing calculator)

[Pricing calculator URL to be generated when submitting — see REVIEW.md pendency.]

Rough internal estimate based on production measurements:
- Gemini 3 Flash full pipeline: ~$0.19 per student exam
- Anticipated grant-period usage: ~5,000–10,000 exam-equivalents across benchmarking and pilot deployment

---

## Proposal (≤ 250 words)

> The core artifact. Must include: research problem, GCP tools, project timeline, key milestones and outcomes, and how GCP can support the research in the future.

---

Educational data on a single student is fragmented across institutional silos: schools hold grades and attendance, child welfare councils hold reports, the juvenile justice system holds socio-educational measures. NOVO CR (https://ia-educacao-v2.onrender.com) is a longitudinal data infrastructure for AI-assisted educational assessment, running in production with 26 subjects, 100+ processed activities, and three providers (Anthropic, OpenAI, Google) integrated in parallel. A real 7-page cross-course report covering 9 disciplines across 4 years of one student's trajectory has already been produced as proof of concept.

GCP credits would fund production-scale evaluation of Gemini against alternatives at each of six pipeline stages. Current measurements show Gemini 3 Flash full pipeline at ~$0.19 per student exam; sustained API usage is needed to engineer per-stage selection rigorously and to build the missing batch pipeline for the cross-course longitudinal report (currently chat-only).

Timeline (12 months): months 1–3, provider benchmark per stage; months 4–6, batch pipeline for cross-course report; months 7–9, pilot deployment in FGV K–12 school (CTAE); months 10–12, municipal Rio de Janeiro network evaluation via SUBDEIS.

Outcomes: per-stage benchmark report, working batch longitudinal pipeline, FGV pilot deployment, submission to CNPq Jovem Cientista Prize 2026 (track 3, AI and Education). Continuity beyond the grant: pursuit of CNPq funding plus structural cost reductions from prompt-caching benchmarks established during the grant period.

---

**Word count (counted):** ~221 words. Under 250 limit. ✓

---

(v3 stabilized after self-critique. Stopping here pending Otavio's review and Valdemar's confirmation.)
