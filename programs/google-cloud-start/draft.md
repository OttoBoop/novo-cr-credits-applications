# Google Cloud Start — Application draft

> Latest stable version. Iteration history in [`loop-log.md`](loop-log.md).
> **Status:** ready in content; not submittable until Otavio incorporates a legal entity. The blocker is operational (incorporation), not editorial.

---

## v3 (2026-05-24)

### Eligibility note (read first)

This program requires a registered company under 5 years old, pre–Series A funding, with a working website. **The Novo CR is currently a personal research project; an incorporated entity does not yet exist.** This draft documents what would be submitted *once* the company is registered. It is consistent with the strategic decision to incorporate that follows from either (a) FGV Ventures acceptance into batch 20 or (b) Otavio's standalone decision to commercialize.

### Identification fields (to be filled at incorporation)

| Form field | Value (placeholder) |
|---|---|
| Company name | TBD (e.g., "Novo CR Tecnologia em Educação Ltda." or MEI under Otavio's CPF) |
| CNPJ | TBD |
| Date of incorporation | TBD (target: 2026 H2 if path proceeds) |
| Country | Brazil |
| State | Rio de Janeiro |
| Industry | EdTech — AI-assisted educational assessment |
| Website | https://ia-educacao-v2.onrender.com (or a separate corporate site to be built) |
| Funding stage | Pre-funded / bootstrapped |
| Institutional VC funding received? | No |
| Prior Google Cloud credits? | None |
| Founder name | Otavio Bopp |
| Founder LinkedIn / email | TBD |

### Company description

The Novo CR is an early-stage Brazilian EdTech company developing longitudinal data infrastructure for AI-assisted educational assessment. The product, currently in alpha at https://ia-educacao-v2.onrender.com, runs a six-stage AI pipeline that turns each student exam into a narrative report — explaining what the student got wrong, what skill they demonstrated, and how they evolve across activities. The teacher keeps the final decision at every stage; the score becomes a byproduct, the report is the artifact.

The system has processed over 100 activities across 26 subjects, using three model providers (OpenAI, Anthropic, Google) in parallel. The bulk of real data comes from the founder's own four-year undergraduate degree at EPGE/FGV (18 disciplines, 2021–2025), with additional contributions from EMAp/FGV via prof. Moacyr Alvim. A 7-page cross-course longitudinal report has already been produced as proof of concept.

### Use of Google Cloud / Gemini

The system runs Gemini models alongside Anthropic Claude and GPT-5 family. Measured per-pipeline production costs:

- Gemini 3 Flash full pipeline (one student exam): ~$0.19
- Gemini 2.5 Flash full pipeline: ~$0.11
- Anthropic side total across 28 production runs: $0.99 / Google side: $0.49

Google Cloud credits would support:

1. **Gemini API benchmarking at scale.** Per-stage evaluation of Gemini against Claude and GPT-5 across the six pipeline stages, with statistically meaningful sample sizes.
2. **Vertex AI exploration.** Specifically for the cross-course longitudinal report (currently chat-only, no batch pipeline). Vertex's structured workflows may offer the missing automation layer.
3. **Pilot deployment infrastructure.** A FGV K–12 school pilot (2027 target with CTAE) would need standard GCP infrastructure for class-wide data processing.

### Founder credentials

Otavio Bopp — Founder and sole technical author. Alumni of EPGE/FGV (BSc Economics, 2025), advised by Valdemar Pinho Neto (coord. of EPGE's undergraduate program). Currently at SUBDEIS (Department of Economic Development, Innovation and Simplification, City of Rio de Janeiro). Built the Novo CR from late 2025; runs three model providers integrated in production.

Academic advisors:
- **Rubens Cysne** (director, EPGE/FGV) — encouraged the project's formal start in December 2025
- **Moacyr Alvim** (prof., EMAp/FGV) — contributed real student data, made the connection to CTAE
- **Mario Andrade** (pedagogical coordinator, CTAE/FGV) — pathway to a 2027 K–12 pilot

### Roadmap

| Phase | Period | Key activity |
|---|---|---|
| Incorporation | 2026 H2 | Register company + transition account ownership |
| Benchmark | 6 months post-incorporation | Per-stage Gemini benchmark report |
| Cross-course pipeline | 6–9 months | Batch automation of longitudinal report |
| FGV K–12 pilot | 2027 | Deploy in one CTAE school (active conversation) |
| Public network | 2027–2028 | Pilot in Rio de Janeiro municipal network via SUBDEIS access |

### What we'd ask for

The standard Start tier benefit: **$2,000 in Google Cloud credits + $200 in training credits for 12 months.** Used primarily for Gemini API and Vertex AI evaluation, plus essential pilot infrastructure.

### Why this tier (not Scale or AI tier)

The Scale and AI tiers require institutional VC funding (Series A or seed from recognized investors). Novo CR is bootstrapped. The Start tier is the appropriate entry point and would directly reduce friction at the company's earliest stage.

### Additional context

- **Live system:** https://ia-educacao-v2.onrender.com (alpha, public)
- **Production cost baseline:** 28 measured runs; total $1.48 across Anthropic + Google
- **Parallel applications:** Anthropic AI for Science and OpenAI Researcher Access (research-track) — Google Cloud Start credits target Gemini/Vertex specifically, with no overlap.
- **Companion academic submission:** CNPq Jovem Cientista Prize 2026, Track 3 (AI and Education), deadline July 31, 2026.
- **Accelerator track:** application in evaluation with FGV Ventures batch 20.

---

(v3 stabilized after self-critique. Operational status: ready in content; awaits incorporation to be submittable.)
