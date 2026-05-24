# Anthropic AI for Science — Application draft

> Latest stable version. Iteration history in [`loop-log.md`](loop-log.md).

---

## v3 (2026-05-24)

### Project title

**NOVO CR — Longitudinal data infrastructure for AI-assisted educational assessment**

### Project summary

Most AI-in-education projects are still at the proposal stage. NOVO CR runs in production at https://ia-educacao-v2.onrender.com with 26 subjects and over 100 processed activities, using three model providers (Anthropic, OpenAI, Google) in parallel. The bulk of its real data is my own four-year undergraduate degree at EPGE/FGV (18 disciplines, 2021–2025), imported through FGV's digital platform eClass, plus a master's-level discipline (Advanced Linear Algebra, EMAp/FGV) contributed by prof. Moacyr Alvim.

The pedagogical surface is a six-stage pipeline that turns each exam into a narrative report explaining what the student got wrong, what skill they demonstrated, and how they evolve across activities — with the teacher keeping the final decision at every stage. The score is a byproduct; the report is the artifact.

Beneath that surface is the methodological contribution: a longitudinal schema (subject N:M class, transparent per-step storage) that joins data which normally lives in disconnected institutional silos. An end-to-end demonstration already exists — a 7-page cross-course report covering 9 disciplines across 4 years of one student's trajectory. The same architecture extends into basic education, opening downstream applications such as early detection of academic decline, longitudinal measurement of socio-educational interventions, and integration with child protection systems.

### Team and institutional affiliation

**Principal researcher:** Otavio Bopp — alumni of FGV/EPGE (BSc Economics, 2025). Built the NOVO CR as a personal research project starting in late 2025. Currently works at SUBDEIS (Department of Economic Development, Innovation and Simplification, City of Rio de Janeiro); previously served in the office of city councilman Flávio Valle (close ally of former mayor and current state-governor candidate Eduardo Paes). These are executive credentials and policy network, not the project's institutional affiliation.

**Institutional affiliation:** Fundação Getulio Vargas through its School of Economics (EPGE/FGV). Specifically:

- **Valdemar Pinho Neto** — coordinator of EPGE's undergraduate program and my undergraduate thesis (TCC) advisor. Co-applicant and institutional signatory.
- **Rubens Penha Cysne** — director of EPGE. Encouraged the project's formal start in December 2025.
- **Moacyr Alvim H. B. da Silva** — professor at EMAp/FGV (School of Applied Mathematics). Contributed real student data and connected the project to FGV's pedagogical coordination at CTAE.
- **Mario Andrade** — pedagogical coordinator at CTAE/FGV (FGV's K–12 school); 13 years in the role. Conversations under way to pilot the system inside a FGV school during 2027.

The team's combined credentials span economics, applied mathematics, K–12 pedagogical operations, and direct construction of production AI systems with three providers integrated.

### Use of Claude API — methodology and technical feasibility

For each exam, the system runs a six-stage pipeline:

1. **Extract questions** from the exam
2. **Extract the answer key** from the corresponding document
3. **Extract the student's answers** from their submission
4. **Correct** by comparing the student's answers to the ideal answers — pure classification, no problem-solving
5. **Analyze skills** demonstrated and gaps revealed
6. **Generate the final report** in narrative form

Each stage produces a visible, editable document — no black box. The teacher retains the decision throughout. The same schema aggregates upward: from the question, to the student, to the activity, to the class, to the subject, and finally to the longitudinal cross-course report.

The system is provider-agnostic by design. Claude runs alongside OpenAI and Google models, configurable per stage. Measured per-pipeline costs in production:

- **Claude Haiku 4.5 (full pipeline, one student):** ~$0.28 (~118k input / ~33k output tokens)
- **Claude Sonnet 4.5 (full pipeline, one student):** ~$0.55 (~68k input / ~23k output tokens)
- **Anthropic-side total across 28 measured production runs:** $0.99

A core architectural opportunity that the credits would enable: **prompt caching of the answer key in the correction stage**, where the same gabarito is reused across every student in a class. The codebase's existing cost analysis projects ~89% reduction in input tokens for this stage in a 30-student run. Sustained API usage is required to engineer and benchmark this properly.

The credits would support:

1. Production refinement of the cross-course longitudinal report, which currently runs only via chat with no batch pipeline.
2. Production-scale evaluation of multi-provider configuration: where Claude is the right model for which stage, with measured cost and quality.
3. Scaling the system to a full FGV pilot school in 2027.

### Expected impact

**Foundational methodological contribution:** the longitudinal schema. Joining classroom data into trajectories that cross courses and years is methodologically novel in Brazilian educational practice — and the 7-page longitudinal report already generated is the proof of concept that the infrastructure produces something previously unobtainable.

**Path to scale (concrete, not hypothetical):**

1. **FGV K–12 school pilot, 2027** — active conversations with CTAE for in-school implementation.
2. **Rio de Janeiro municipal network** — my position at SUBDEIS provides direct access.
3. **Rio de Janeiro state network** — conditional on the gubernatorial election; the political pathway is already built.
4. **Peer-reviewed credential** — submission to the CNPq Jovem Cientista Prize 2026, Track 3 (AI and Education), deadline July 31, 2026.

**Extensions beyond pedagogy.** The same longitudinal infrastructure supports early detection of students in academic decline before child welfare cases escalate, longitudinal measurement of socio-educational interventions for juvenile offenders, and integration with child protection systems. These are downstream applications in basic education; the methodology is general.

### Biosecurity and safety considerations

The system processes educational documents (exams, answer keys, student responses) and produces pedagogical reports. There is no biosecurity vector: no biological, chemical, or weapons-related content; no model fine-tuning; no generation of harmful instructions. Standard Anthropic Usage Policy compliance is in place.

The basic-education extensions involve children's data and apply Brazilian LGPD compliance with the strictest provisions for children and adolescents: identity-sovereign storage, purpose-bound use, limited retention, and access auditing. The system's principle is to **alert the right human, not replace them** — every signal goes to a person with the authority and responsibility to act.

### Estimated credit usage

Based on measured per-pipeline costs:

| Configuration | Cost per student exam | Exams in $20,000 |
|---|---|---|
| Anthropic Haiku only | ~$0.28 | ~71,000 |
| Anthropic Sonnet only | ~$0.55 | ~36,000 |
| Mixed (Haiku extract + Sonnet correct + Haiku analyze) | ~$0.55 | ~36,000 |
| Mixed with prompt caching at correction stage | ~$0.30–0.40 | ~50,000–66,000 |

Allocation across the 6-month grant:

- **~40%** — production usage for the 2026–2027 FGV pilot deployment
- **~30%** — refinement of the cross-course longitudinal report pipeline
- **~20%** — benchmark experiments for per-stage provider selection
- **~10%** — research experiments for the CNPq submission and follow-up academic work

### Additional context

- **Live system:** https://ia-educacao-v2.onrender.com (public, in alpha)
- **Real longitudinal output:** the 7-page, 9-discipline, 4-year cross-course report generated from the principal researcher's own undergraduate transcript imported via eClass — a working demonstration of the infrastructure
- **Companion academic submission:** Prêmio Jovem Cientista CNPq 2026, Track 3 (AI and Education), July 31, 2026
- **Presentation deck:** "NOVO CR — Mais que um Número" (29 slides), available on request

---

(v3 stabilized. Stopping iteration here pending Otavio's review.)
