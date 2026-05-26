# Anthropic AI for Science — Application draft

> Latest stable version (v4 mapped to actual form fields). Iteration history in [`loop-log.md`](loop-log.md).
> Form: Anthropic AI for Science Application Form (link via support article).
> Pre-submission setup: create/locate Anthropic Organization ID at https://console.anthropic.com/settings/organization

---

## v4 (2026-05-24) — mapped to real form fields

### Contact information

| Form field | Value |
|---|---|
| E-mail | (institutional FGV email — to fill at submission) |
| Name of primary contact | **Otavio Bopp** (or Valdemar Pinho Neto as co-applicant, depending on the position field interpretation — see REVIEW.md) |
| Name of organization/research institution | Fundação Getulio Vargas — Escola de Pós-Graduação em Economia (EPGE/FGV) |
| Position/title at organization | Alumni and research collaborator; institutional supervision by Valdemar Pinho Neto (Coordinator of EPGE Undergraduate Program) |
| Website / Google Scholar / GitHub | https://ia-educacao-v2.onrender.com (live system) · GitHub of the project (to be made public for the application) |
| Where did you hear about this program? | Direct discovery via the Anthropic Help Center |

### Project information

**Project title:**
> NOVO CR: Longitudinal Data Infrastructure for AI-Assisted Educational Assessment

**Scientific field(s) (select all that apply):**
- ☑ Computer Science
- ☑ Other: **Education / Learning Sciences**

**Organization ID:**
[To be filled from https://console.anthropic.com/settings/organization. Pre-submission action: create the org if not already done; record the ID — looks like `1bc14c5d-6442-4fa9-bgjj-c1ejei29aef01v`.]

### Research Team (<300 words)

Otavio Bopp is principal investigator and sole technical author of the NOVO CR system. He holds a BSc in Economics from EPGE/FGV (2025), where Valdemar Pinho Neto advised his undergraduate thesis. He currently serves at SUBDEIS (Department of Economic Development, Innovation and Simplification, City of Rio de Janeiro); previously, he worked in the office of city councilman Flávio Valle. He built and operates NOVO CR in production, integrating three model providers (OpenAI, Anthropic, Google) since late 2025.

The project has been formally ongoing since December 2025, when Rubens Penha Cysne (director, EPGE/FGV) encouraged its formal start. Institutional supervision sits with Valdemar Pinho Neto (Coordinator of EPGE/FGV's undergraduate program). Moacyr Alvim H. B. da Silva (professor, EMAp/FGV) contributed real master's-level discipline data and connected the project to FGV's pedagogical coordination at CTAE via Mario Andrade (pedagogical coordinator, 13 years in the role).

Combined expertise spans economics and quantitative methods (EPGE), applied mathematics (EMAp), K–12 pedagogical operations (CTAE), and direct construction of production AI systems with three providers. AI/ML experience is operational rather than purely academic: the team owns and runs a production multi-provider system with measured costs across 187 priced production runs and a working durable token-usage persistence layer.

A note relevant to the program's stated interest in supporting researchers with limited institutional resources: Brazilian researchers building production AI infrastructure in education operate at a structural cost disadvantage relative to peers in North America or Europe. API spend currently comes out of the principal investigator's personal funds. This grant would unblock scientific-grade benchmarking at scale.

*Word count: ~283*

### Key team members

- **Otavio Bopp**, Principal Investigator. Designs, builds, and operates the NOVO CR system; conducts experiments.
- **Valdemar Pinho Neto**, Co-Applicant / Institutional Signatory. Coordinator of EPGE/FGV's undergraduate program. Supervises research direction.
- **Rubens Penha Cysne**, Senior Advisor. Director, EPGE/FGV. Encouraged project formal start (Dec 2025).
- **Moacyr Alvim H. B. da Silva**, Data Contributor. Professor, EMAp/FGV. Contributed master's-level student data; bridged the project to CTAE.
- **Mario Andrade**, Implementation Partner. Pedagogical coordinator, CTAE/FGV (FGV's K–12 school). Pathway to 2027 pilot deployment.

### Academic profile links

- Valdemar Pinho Neto: https://www.linkedin.com/in/valdemar-pinho-neto-9359a0204/
- Rubens Penha Cysne: https://epge.fgv.br/pt/professor/rubens-cysne
- Moacyr Alvim H. B. da Silva: https://emap.fgv.br/professores/moacyr-alvim-horta-barbosa-da-silva
- Otavio Bopp: [LinkedIn — to be filled]
- Mario Andrade: https://www.linkedin.com/in/mario-andrade-67a00544/

### Research Proposal (<500 words)

**Scientific question:** Can automated, transparent AI-assisted assessment produce longitudinal educational data of clinical quality — capturing not only what students get wrong but what skills they demonstrate and how they evolve across years and disciplines? And can that data be joined with currently siloed institutional records (attendance, behavioral, social) to support evidence-based educational interventions?

**Methodology:** NOVO CR runs a six-stage AI pipeline per exam: extract questions, extract answer key, extract student responses, correct by comparison (classification, not generation), analyze demonstrated skills, generate narrative report. The architecture is provider-agnostic; Claude, GPT, and Gemini models are configured per stage. The schema is longitudinal — subject N:M class — and every step is stored as an editable document, enabling audit of the model's reasoning at each layer. The system aggregates upward from question to student, to activity, to class, to subject, and to the cross-course report.

**Expected outcomes and deliverables:**
1. Per-stage benchmark study comparing Claude (Haiku 4.5, Sonnet 4.5) against OpenAI and Google models, with measured cost and quality at sample sizes that yield statistical confidence.
2. Production-ready batch pipeline for the cross-course longitudinal report (currently only available via chat).
3. Engineered prompt caching for the correction stage, projected to reduce input tokens by ~89% in a 30-student class run.
4. Peer-reviewed methodology paper submitted to the CNPq Jovem Cientista Prize 2026 (Track 3: AI and Education, deadline July 31, 2026).
5. Pilot deployment in one FGV K–12 school during 2027 (CTAE conversations under way).

**Timeline (6 months):**
- Months 1–2: Establish Claude API integration at production scale; configure per-stage benchmarks.
- Months 3–4: Run per-stage comparative study; engineer prompt caching at the correction stage.
- Months 5–6: Build batch pipeline for cross-course longitudinal report; pilot at single FGV class.

The system has been ongoing since December 2025 and runs in production today at https://ia-educacao-v2.onrender.com with 26 subjects and over 100 processed activities. A 7-page real cross-course report covering 9 disciplines across 4 years of the principal investigator's own undergraduate trajectory has already been generated as a working proof of the longitudinal infrastructure.

For a Brazilian researcher operating without institutional funding, API spend is the primary bottleneck. The requested credits transform a question of "can we run scientifically rigorous benchmarks" into "how do we run them best."

*Word count: ~360*

### How specifically will Claude be used (1-2 sentences, 300 words max)

Claude (Haiku 4.5 and Sonnet 4.5) is configured per pipeline stage: Haiku for cost-efficient extraction (questions, answer keys, student responses) and skill analysis; Sonnet for the correction stage where classification accuracy matters most, and where prompt caching of the answer key across students in a class is engineered to yield ~89% input-token reduction. The cross-course longitudinal report — currently chat-only — will use Claude's long-context capabilities to read multiple years of one student's documents into a single narrative report, then be packaged into a batch pipeline funded by these credits.

Measured production baselines: Claude Haiku 4.5 full pipeline ~$0.28 per student exam (~118k input / ~33k output tokens); Claude Sonnet 4.5 full pipeline ~$0.55 (~68k input / ~23k output tokens). Across 28 production runs in 2026 Q2, Anthropic-side spend totaled $0.99. Token usage is persisted durably via Supabase migration (`record_count=20` over 187 priced runs at the most recent audit, 2026-05-23).

*Word count: ~152*

### How will Claude accelerate research (1-2 sentences, 200 words max)

Two capabilities make Claude the right tool for stages where alternatives underperform: (1) structured extraction from messy real-world educational documents (handwritten exams, multi-page student responses, mixed-format PDFs) with reliability sufficient for production deployment, and (2) the long-context windows needed for cross-course longitudinal reports that may span multiple years of one student's documents. Existing alternatives are either opaque grading APIs without an audit trail or research prototypes without longitudinal infrastructure; Claude lets us combine the strengths of frontier models with the architectural transparency that educational deployment requires.

*Word count: ~98*

### Scientific impact (1-2 sentences, 200 words max)

NOVO CR's foundational contribution is methodological: a longitudinal data schema for AI-assisted educational assessment that joins clinical-quality narrative reports (per exam) with cross-time and cross-discipline aggregation — methodologically novel in Brazilian educational practice. If successful, the schema becomes reusable infrastructure for AI-in-education researchers, K–12 schools, and educational policy researchers, supported by an academic credentialing layer through the CNPq Jovem Cientista Prize submission.

*Word count: ~75*

### Practical applications (1-2 sentences, 200 words max)

The longitudinal infrastructure supports applications beyond pure pedagogy: early detection of academic decline (joining attendance, behavioral, and ocorrência records currently in disconnected school systems); measurement of socio-educational intervention efficacy for juvenile justice cases; and integration with child protection systems under strictest LGPD compliance for minors. Path to scale begins with the FGV K–12 pilot in 2027, expands to Rio de Janeiro's municipal network via SUBDEIS access, and extends to the state level conditional on political alignment.

*Word count: ~85*

### Success metrics (1-2 sentences, 200 words max)

- ≥1,000 student-exam-equivalents processed through Claude in benchmark experiments by month 4
- Documented cost/quality measurements for Claude vs alternatives at each of 6 pipeline stages, with effect sizes
- ≥85% measured input-token reduction at the correction stage via prompt caching (projected ~89%)
- ≥50 students processed end-to-end through the batch cross-course pipeline by month 6
- Documented LOI with one CTAE school for the 2027 pilot
- CNPq Jovem Cientista Prize 2026 submission accepted into final round

*Word count: ~85*

### Resource Requirements — credit amount

**Requested: up to $50,000 USD in Claude API credits over a 6-month period.**

Justification with measured baselines:
- Claude Haiku full pipeline: ~$0.28 per student exam
- Claude Sonnet full pipeline: ~$0.55 per student exam
- Mixed mid-tier configuration: ~$0.55 per exam
- With engineered prompt caching at the correction stage: ~$0.30 per exam

$50,000 supports approximately:
- 5,000–10,000 student-exam pipeline runs for benchmarking and per-stage measurement
- 500–1,000 cross-course longitudinal report generations
- Pilot deployment for one FGV class (~30 students × multiple disciplines × multiple semesters)
- Engineering and validation of the prompt caching infrastructure that the codebase already projects can yield ~89% input-token reduction at the correction stage

For a Brazilian researcher with no institutional funding line, this grant transforms a question of "can we afford to run scientifically rigorous benchmarks" into "how do we run them best."

*Word count: ~155*

### Biosecurity assessment

**Selected:** ☑ None of the above.

The system processes educational documents (exams, answer keys, student responses) and produces pedagogical reports. There is no pathogen research, drug resistance work, toxicology, or synthetic biology. Standard Anthropic Usage Policy compliance is in place. For the future basic-education extensions involving children's data (one of the project's downstream applications), Brazilian LGPD applies with strictest provisions for minors: identity-sovereign storage, purpose-bound use, limited retention, and access auditing.

### Additional information

- The project has been ongoing since December 2025 when Rubens Cysne encouraged its formal start.
- Production system in alpha at https://ia-educacao-v2.onrender.com.
- A real 7-page cross-course longitudinal report covering 9 disciplines across 4 years of the principal investigator's own undergraduate trajectory has already been generated, demonstrating the architecture end-to-end.
- Companion academic submission to the CNPq Jovem Cientista Prize 2026 (Track 3: AI and Education) is under preparation; deadline July 31, 2026.
- Parallel applications to OpenAI Researcher Access Program ($1K, complementary) and Google Cloud Research Credits (complementary) — targeting per-provider evaluation, with no overlap in API spend.

---

(v4 mapped to actual form fields. Critical pre-submission setup: Anthropic Organization ID. See [`REVIEW.md`](../../REVIEW.md) for full pendency list.)
