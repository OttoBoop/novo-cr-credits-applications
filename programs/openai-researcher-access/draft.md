# OpenAI Researcher Access — Application draft

> Latest stable version (v4 mapped to actual form fields). Iteration history in [`loop-log.md`](loop-log.md).
> **Valdemar Pinho Neto signs as main author** (OpenAI requires "active affiliation"; alumni alone does not satisfy).
> Pre-submission setup: Org-ID at https://platform.openai.com/account/organization (set up if not done).

---

## v4 (2026-05-24) — mapped to real form fields

### Contact

| Form field | Value |
|---|---|
| First Name | **Valdemar** |
| Last Name | **Pinho Neto** |
| Institutional Email Address | (Valdemar's @fgv.br institutional email — to fill at submission) |
| Email associated with OpenAI API account | (account-holder email — likely Valdemar's after setup; alternatively a project account email) |
| Institution or organization | Fundação Getulio Vargas — Escola de Pós-Graduação em Economia (EPGE/FGV) |
| Professional profile links | https://www.linkedin.com/in/valdemar-pinho-neto-9359a0204/ · plus Otavio's LinkedIn for co-investigator |
| Country | Brazil |
| Educational Stage | Faculty |
| Gender Identity | (Valdemar's preference) |

### Research Areas

Select (in order of fit):
- ☑ **Societal impact**
- ☑ **Interdisciplinary research**
- ☑ **Interpretability / transparency**

Rationale: the project's strongest alignment is with three of OpenAI's named priority areas. Societal impact captures the longitudinal-data infrastructure with applications in child protection and socio-educational measurement. Interdisciplinary research captures economics + applied mathematics + pedagogy + production AI engineering. Interpretability/transparency captures the architecture choice of producing a visible, editable document at every pipeline stage.

### Project Description

#### Research question

How can transparent, multi-provider AI-assisted assessment produce longitudinal educational data of clinical quality — narrative reports per exam, plus cross-time/cross-discipline aggregation — and how can GPT models contribute optimally to specific stages of that pipeline when compared rigorously against alternatives? The project has been ongoing since December 2025 (formally encouraged by Rubens Cysne, director of EPGE/FGV) and runs in production at https://ia-educacao-v2.onrender.com.

#### Research design

NOVO CR runs a six-stage AI pipeline per student exam: extract questions, extract answer key, extract student responses, correct by comparison (pure classification, not generation), analyze demonstrated skills, generate narrative report. The architecture is provider-agnostic by design: OpenAI GPT-5 family, Anthropic Claude 4.5 family, and Google Gemini 3 family are configured per stage. Every step stores a visible, editable document; no black box.

With this grant, the design extends to systematic per-stage benchmarking of GPT models against alternatives. The codebase already has durable token-usage persistence (Supabase migration applied 2026-05-23, `record_count=20` over 187 priced production runs); the missing layer is sustained sample-size sufficient for statistical confidence at each stage. We hypothesize GPT-5.4 Mini and Nano variants will dominate cost-efficiency at extraction stages, while comparison against Claude Sonnet at the correction stage is the open empirical question we want to settle.

#### Expected outcomes

A per-stage benchmark report comparing GPT-5 family models against Claude and Gemini, with measured cost ($), measured quality (rubric-graded by independent reviewers), and engineering recommendations for per-stage provider selection. Public methodology contribution to the cross-provider AI-for-education research conversation; production deployment documentation; and the foundation for the FGV K–12 school pilot in 2027 (CTAE conversations under way).

### Timeline

12 months. Months 1–3: integration of GPT models at production scale and per-stage benchmark design. Months 4–9: rigorous comparative measurement at sample sizes yielding statistical confidence. Months 10–12: benchmark report, methodology paper preparation, and pilot integration with FGV K–12 school in 2027.

### Budget

Up to **$1,000 USD** (the maximum under this program) in OpenAI API credits.

Measured GPT family per-pipeline production costs (2026-05-23 audit):
- GPT-5 Nano full pipeline: ~$0.017 per student exam
- GPT-5.4 Mini full pipeline: ~$0.079 per student exam
- GPT-4.1 full pipeline: ~$0.54 per student exam
- GPT-5 (premium) full pipeline: ~$1.05 per student exam

$1,000 supports approximately:
- ~10,000 nano-tier exam runs for high-volume benchmarking
- ~12,500 GPT-5.4 Mini exam runs at the cost-efficient tier
- ~1,000 full GPT-5 premium runs at the high-quality end

For a Brazilian researcher operating without institutional research funding, this grant is meaningful at this scale. Brazilian researchers building production AI infrastructure in education face a structural cost disadvantage relative to peers in North America and Europe; OpenAI's stated interest in supporting researchers with limited resources aligns directly with our circumstances.

### Org-ID

[To be filled from https://platform.openai.com/account/organization. Pre-submission action: ensure the OpenAI organization for this research is set up. The credits will be applied here if accepted.]

### Additional collaborators (up to 6 investigators)

| Role | Name | Email | Notes |
|---|---|---|---|
| Investigator | Otavio Bopp | (to fill) | Co-investigator, system builder, alumni EPGE/FGV |
| Investigator | Rubens Penha Cysne | rubens.cysne@fgv.br | Director EPGE; encouraged project start (Dec 2025) |
| Investigator | Moacyr Alvim H. B. da Silva | (institutional email) | Professor EMAp/FGV; data contributor |
| Investigator | (optional) | — | — |
| Investigator | (optional) | — | — |
| Investigator | (optional) | — | — |

### Past research

To be filled by Valdemar (primary applicant). Suggested submissions:
- Otavio's TCC (undergraduate thesis advised by Valdemar) — TBD if relevant
- Valdemar's published economics papers (most relevant to the analytical/quantitative aspects)
- Any prior FGV publications on educational data or analytics

### Any other comments

The project has been ongoing since December 2025, when Rubens Cysne (director of EPGE/FGV) encouraged its formal start. Production system in alpha at https://ia-educacao-v2.onrender.com with 26 subjects and over 100 processed activities; a 7-page real cross-course longitudinal report covering 9 disciplines across 4 years has already been generated as a working proof of concept.

Parallel applications: Anthropic AI for Science Program (up to $50K, complementary — Anthropic-specific optimizations) and Google Cloud Research Credits (Gemini-specific evaluation, complementary). OpenAI credits target GPT-specific per-stage evaluation, with no overlap in API spend.

Companion academic submission: CNPq Jovem Cientista Prize 2026, Track 3 (AI and Education), deadline July 31, 2026.

The principal investigator (Valdemar Pinho Neto) is currently coordinator of the EPGE/FGV undergraduate program and Otavio's former TCC advisor. His active institutional affiliation satisfies the program's eligibility criterion (alumni status alone would not qualify the co-investigator independently).

---

(v4 mapped to actual form fields. Critical pre-submission setup: OpenAI Org-ID + Valdemar's institutional emails. See [`REVIEW.md`](../../REVIEW.md).)
