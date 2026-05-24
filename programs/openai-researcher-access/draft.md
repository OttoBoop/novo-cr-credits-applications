# OpenAI Researcher Access — Application draft

> Latest stable version. Iteration history in [`loop-log.md`](loop-log.md).

---

## v3 (2026-05-24)

### Project title

**NOVO CR — Longitudinal data infrastructure for AI-assisted educational assessment**

### Principal investigator and team

**Principal investigator:** Valdemar Pinho Neto — coordinator of the undergraduate program at the School of Economics (EPGE/FGV), Fundação Getulio Vargas, Rio de Janeiro. Economist; supervisor of the project's research direction.

**Co-investigator (project builder):** Otavio Bopp — alumni of EPGE/FGV (BSc Economics, 2025), Valdemar's former undergraduate thesis advisee. Built and operates the NOVO CR system. Funds API costs personally; currently employed at SUBDEIS (Department of Economic Development, Innovation and Simplification, City of Rio de Janeiro).

**Additional collaborators:** Rubens Penha Cysne (director, EPGE/FGV; encouraged the project's formal start in December 2025); Moacyr Alvim H. B. da Silva (professor, EMAp/FGV; contributed real master's-level student data); Mario Andrade (pedagogical coordinator, CTAE/FGV; pathway to a K–12 pilot in 2027).

### Project summary

NOVO CR is a longitudinal data infrastructure for AI-assisted educational assessment, running in production at https://ia-educacao-v2.onrender.com with 26 subjects and over 100 processed activities. It uses three model providers (OpenAI, Anthropic, Google) in parallel.

The pedagogical surface is a six-stage pipeline that turns each exam into a narrative report explaining what the student got wrong, what skill they demonstrated, and how they evolve across activities — with the teacher keeping the final decision at every stage. The score is a byproduct; the report is the artifact.

Beneath that surface is a longitudinal schema (subject N:M class, transparent per-step storage) that joins data normally fragmented across institutions. A 7-page real cross-course report covering 9 disciplines across 4 years of one student's trajectory has already been generated as a proof of concept.

### Alignment with OpenAI's research priorities

The project addresses three of OpenAI's stated areas of interest:

**Societal impact.** Educational data on a single student lives in disconnected silos: the school holds grades and attendance, the tutoring council holds reports, the juvenile justice system holds socio-educational measures. No one sees the whole picture. The infrastructure we build is the missing connective tissue. Beyond pedagogy, the same architecture supports early detection of academic decline before child welfare cases escalate, longitudinal measurement of socio-educational interventions for juvenile offenders, and integration with child protection systems.

**Interpretability and transparency.** Every pipeline stage produces a visible, editable document. There is no black box. A teacher can inspect what the model extracted from each exam document, how it compared the student's answer to the answer key, what skills it inferred, and how the final report was assembled. This is a deliberate contrast to opaque grading systems.

**Interdisciplinary research.** The team combines economics (EPGE), applied mathematics (EMAp), K–12 pedagogical operations (CTAE), and the direct construction of production AI systems with three providers integrated — economics-trained researchers building infrastructure that crosses into learning sciences and child protection.

### Use of OpenAI API

The system runs GPT-5 family models alongside Anthropic Claude and Google Gemini, configurable per pipeline stage. Per-stage model assignment is parameterized; each provider is evaluated against the particular requirements of extraction, classification, and narrative generation, in an ongoing internal benchmarking exercise.

The requested credits would support:

1. Production-scale evaluation of per-stage provider selection — when GPT-5 is the right choice, with measured cost and quality compared to alternatives.
2. Refinement of the cross-course longitudinal report, which currently runs only via chat with no batch pipeline.
3. Research-grade experiments backing the submission to the Brazilian CNPq Jovem Cientista Prize 2026 (Track 3, AI and Education, deadline July 31, 2026).

### Limited financial and institutional resources

NOVO CR is a personal research project. API costs are paid out of pocket by the co-investigator. There is no institutional funding line, no venture capital, no commercial revenue. Brazilian researchers building production AI infrastructure in education operate at a structural cost disadvantage compared to North American or European labs. The $1,000 credit grant is meaningful at this scale and reduces the friction of running production-grade experiments.

### Compliance and data

The team will comply with OpenAI's Usage Policy and Sharing & Publication Policy. Educational data already in the system was contributed under appropriate institutional permissions: prof. Moacyr Alvim (EMAp/FGV) contributed master's-level discipline data; the co-investigator imported his own undergraduate transcript via FGV's eClass platform. Brazilian LGPD applies, with strictest provisions for minors as the system extends into basic education.

### Expected outputs over the 12-month grant period

1. Per-stage benchmark report comparing GPT-5 family against Anthropic and Google for each pipeline stage.
2. A working batch pipeline for the cross-course longitudinal report.
3. Research artifact submitted to CNPq Jovem Cientista Prize 2026 (July 31).
4. Production deployment in a pilot FGV K–12 school in 2027.

### Additional context

- **Live system:** https://ia-educacao-v2.onrender.com (alpha; public)
- **Parallel application:** Anthropic AI for Science (submitted separately; not redundant — Anthropic credits target Claude-specific optimizations, OpenAI credits target GPT-specific evaluation)
- **Companion academic submission:** Prêmio Jovem Cientista CNPq 2026, Track 3 (AI and Education), July 31, 2026
- **Presentation deck:** "NOVO CR — Mais que um Número" (29 slides), available on request

---

(v3 stabilized after self-critique. Stopping here pending Otavio's review.)
