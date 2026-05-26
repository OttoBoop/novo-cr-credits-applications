# REVIEW — items requiring Otavio's attention

> Single consolidated file for all open items across every program application.
> Logs (`programs/<X>/loop-log.md`) carry the full chronology; this file carries only what needs *you* to act, decide, or verify.
> Last updated: 2026-05-24 (session 3 — drafts v4 mapped to real form fields).

## How to use this

- Read top-down. Each program section has three buckets:
  - 🔴 **Critical** — blocks submission of that program.
  - 🟡 **Verify** — fact-checks needed; doesn't block drafting but blocks submission.
  - 🔵 **Decide** — strategic / preference choices.
- Each item is checkboxed (`- [ ]`). Mark resolved as you go.

---

## 🎯 Cross-cutting (one action unlocks 3 programs)

### 🔴 Critical

- [ ] **Send the support email to Valdemar Pinho Neto.**
  - Draft ready at [`shared/valdemar-support-email.md`](shared/valdemar-support-email.md).
  - Covers all 3 research programs (Anthropic, OpenAI, Google Research) in one email.
  - Why unified: same project, same credentials, respects Valdemar's time.
  - Action: review draft, edit if needed, send to Valdemar's @fgv.br email.

- [ ] **If Valdemar agrees, authorize me to draft the support letter for Anthropic.**
  - Anthropic accepts team applications but typically expects a brief institutional letter.
  - Length: ~1 page in PT-BR (Valdemar reads); EN version if requested.
  - Content: attests Otavio is alumni + research collaborator under Valdemar's supervision; the project is genuine research aligned with EPGE/FGV.

### 🔵 Decide

- [ ] **Submit unified email vs three separate emails to Valdemar.**
  - My recommendation: unified (drafted that way).
  - Alternative: 3 separate emails per program. Costs more of Valdemar's time but allows him to engage with each on its own merits.

---

## Anthropic AI for Science

Status: **draft v4 mapped to real form fields**. Up to **$50,000** in API credits (corrected from my earlier $20K). 30-min video call if approved.

### 🔴 Critical

- [ ] **Create / locate Anthropic Organization ID.**
  - URL: https://console.anthropic.com/settings/organization
  - Format example given by Anthropic: `1bc14c5d-6442-4fa9-bgjj-c1ejei29aef01v`
  - Action: log into Anthropic Console with the email you want associated with the project; copy the org ID into draft.md §Project information.

- [ ] **Position/title at organization** — ambiguous in v4 because Otavio is alumni and Valdemar is Faculty.
  - My current draft text: "Alumni and research collaborator; institutional supervision by Valdemar Pinho Neto (Coordinator of EPGE Undergraduate Program)"
  - Alternative: list Valdemar as primary contact and have his Position field state "Coordinator of EPGE/FGV Undergraduate Program".
  - Decide who is "primary contact" in the form: Otavio (operates the system) or Valdemar (faculty signatory)?

- [ ] **GitHub of the project — make public for the application.**
  - Currently the production system runs from a repo; need to confirm visibility and ensure it's appropriate for an external review.

### 🟡 Verify

- [ ] **Otavio's LinkedIn URL** — currently `[LinkedIn — to be filled]` in §Key team members.

- [ ] **Brazilian cost angle wording** — appears in §Research Team, §Resource Requirements, §Research Proposal. Otavio asked to reinforce; I may have over-reinforced. Verify the wording reads as context, not lamentation.

- [ ] **GPT-5.4 Mini at $0.079** number used in §Use of Claude API context — actually this stat is for GPT, not Claude. v4 only uses Claude-specific numbers ($0.28 Haiku, $0.55 Sonnet). Verify no cross-contamination of numbers.

### 🔵 Decide

- [ ] **Video call prep** — if approved, Anthropic schedules a 30-min video call before applying credits.
  - Suggested prep: demo of the live system, walkthrough of the longitudinal report, Q&A. I can draft a video-call brief if you want.

- [ ] **Where did you hear about this program?** — free-text. Current value: "Direct discovery via the Anthropic Help Center". Adjust if the source was different.

---

## OpenAI Researcher Access

Status: **draft v4 mapped to real form fields**. Up to **$1,000** in API credits (12 months, non-renewable). Valdemar required as main author.

### 🔴 Critical

- [ ] **Confirm Valdemar agrees to be primary applicant (main author).** Same as cross-cutting item.

- [ ] **Create / locate OpenAI Org-ID.**
  - URL: https://platform.openai.com/account/organization
  - Action: Valdemar (or Otavio under Valdemar's email) creates an OpenAI account for the research; copy the org-ID into draft.md.

- [ ] **Valdemar's institutional FGV email.**
  - Currently placeholder in draft.md §Contact.

### 🟡 Verify

- [ ] **Research Areas selection** — currently 3 selected: Societal impact, Interdisciplinary research, Interpretability/transparency.
  - Verify with Valdemar: does he agree these are the right framing? Alternative areas (Fairness & representation, Robustness) are possible.

- [ ] **Past research field** — placeholder in draft.md. Suggested entries: Otavio's TCC, Valdemar's published economics papers.
  - Action: Valdemar / Otavio select 1-3 relevant entries.

- [ ] **Gender Identity field** — Valdemar's preference. Leave blank if he prefers.

### 🔵 Decide

- [ ] **Additional collaborators (up to 6 investigators).**
  - Current list: Otavio (co-investigator), Cysne, Moacyr, + 3 optional slots.
  - Decide: include Mario Andrade? Layla Mendes? Diogo Robaina?
  - Constraint: each collaborator listed must have an OpenAI API account.

- [ ] **Submission window.**
  - Next quarterly review: **June 2026** (first week).
  - Alternative: September 2026 (after CNPq July 31 submission, adds peer-review credential).
  - My recommendation: June (don't wait — Valdemar conversation should move quickly).

---

## Google Cloud Research Credits

Status: **draft v4 mapped to real form fields, Field of Research = Computer Science**. Heavy operational pendencies remain.

### 🔴 Critical

- [ ] **Confirm Valdemar as Faculty applicant of record.** Same as cross-cutting.

- [ ] **Obtain Google Cloud Billing Account ID — institutional FGV (max 25 characters).**
  - Setup link: https://console.cloud.google.com/billing
  - Action: coordinate with EPGE financial/IT department.
  - Risk: this can take weeks via FGV institutional channels.

- [ ] **Generate Google Cloud Pricing Calculator URL.**
  - Calculator: https://cloud.google.com/products/calculator
  - Action: configure for projected Gemini API usage (~5,000–10,000 exam-equivalents × ~$0.19 = ~$1K–$2K), save, share URL.

- [ ] **Valdemar's institutional email** — placeholder.

### 🟡 Verify

- [ ] **"We already use Gemini in production"** wording — v4 brings this prominently. Verify it reads as positive signal (we know the tooling) rather than negative (you already use it, why need more credits).
  - My intent: positive signal of operational maturity + cost data credibility.

- [ ] **Project start date = December 2025** in draft v4. Bate com a história (Cysne instigou).

### 🔵 Decide

- [ ] **Submission timing.**
  - Application is rolling — no fixed window.
  - My recommendation: submit after billing account is set up (probably 1–2 months from now). Don't submit incomplete.

- [ ] **Award amount expectations.**
  - Google doesn't publish per-applicant amounts. Range varies widely.
  - Implication: don't anchor on a specific number; ask for what the project needs.

---

## Google Cloud Start

Status: **PARKED** — Otavio explicitly cannot incorporate right now. Re-evaluate when this changes.

### 🔵 Decide

- [ ] **Re-open when:** (a) FGV Ventures accepts into batch 20 (may facilitate incorporation via Gust ecosystem), OR (b) Otavio's circumstances change.

- [ ] **Backlog (not for this round):**
  - MEI vs Ltda consultation
  - Microsoft Founders Hub, AWS Activate, NVIDIA Inception (all incorporation-gated)

---

## FGV Ventures batch 20

Status: **email v6 enviado em 2026-05-15.** 9 dias sem resposta documentada. Aguardando resposta de Isabel Pinheiro e Luciana Cualheta.

### 🔴 Critical (time-sensitive)

- [ ] **Considere follow-up curto no mesmo thread.**
  - My recommendation: uma mensagem curta ("queria confirmar que recebem") sem novo subject, sem novo conteúdo. Padrão respeitoso para programa estruturado.

### 🔵 Decide

- [ ] **If they respond with interest:** próximos passos (entrevista, dossiê adicional, decisão sobre inscrição formal no Gust).

- [ ] **If they accept into batch 20:** isto destrava a decisão de incorporação. Re-abrir Google Cloud Start + considerar OpenAI Startups.

- [ ] **If they reject:** registrar feedback no `loop-log.md`; usar como input pra Microsoft / AWS / NVIDIA.

### 🟡 Verify

- [ ] **Subject do email v6** — confirmar com Otavio se foi com subject específico ou padrão.

---

## Closed items

(Items will move here once resolved.)

- ✅ **Anthropic credit ceiling** — corrected from $20K to up to $50K (Otavio shared form 2026-05-24).
- ✅ **Anthropic form fields** — now fully known (verbatim from Otavio 2026-05-24).
- ✅ **OpenAI form fields** — now fully known (verbatim from Otavio 2026-05-24).
- ✅ **Google Cloud Research Field of Research** — Computer Science (Otavio confirmed).
- ✅ **Otavio cannot incorporate now** — Google Cloud Start moved to PARKED status.
