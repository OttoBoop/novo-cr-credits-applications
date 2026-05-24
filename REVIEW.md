# REVIEW — items requiring Otavio's attention

> Single consolidated file for all open items across every program application.
> Logs (`programs/<X>/loop-log.md`) carry the full chronology; this file carries only what needs *you* to act, decide, or verify.
> Last updated: 2026-05-24 (session 2 — autonomous draft loop).

## How to use this

- Read top-down. Each program section has three buckets:
  - 🔴 **Critical** — blocks submission of that program.
  - 🟡 **Verify** — fact-checks needed; doesn't block drafting but blocks submission.
  - 🔵 **Decide** — strategic / preference choices.
- Each item is checkboxed (`- [ ]`). Mark resolved as you go.
- Each item lists: my claim or question + my source/inference + my best guess + what I need from you + where the item shows up in the repo.

---

## Anthropic AI for Science

Status: draft v3 stable. Loop paused pending your review.

### 🔴 Critical

- [ ] **Open the official Google Form and copy the fields to me.**
  - URL: https://docs.google.com/forms/d/e/1FAIpQLSfwDGfVg2lHJ0cc0oF_ilEnjvr_r4_paYi7VLlr5cLNXASdvA/viewform
  - Why I can't: WebFetch can't open authenticated Google Forms; I only saw the public preamble pages.
  - Risk if skipped: draft.md is structured against my best guess of typical fields. Might need re-cutting if real fields differ (e.g., strict word limits per question).
  - Where: `programs/anthropic-ai-for-science/draft.md`

- [ ] **Decide submission window.**
  - Options: 1 jun (next first-Monday cycle) / 6 jul (after CNPq submission) / 3 ago.
  - My recommendation: **6 jul** — adds CNPq credential to the narrative without losing too much momentum.
  - Why this matters: timing affects the framing of "Companion academic submission" in §Additional context.

- [ ] **Confirm Valdemar Pinho Neto as co-applicant + institutional signatory.**
  - Source: `shared/team-and-credentials.md` + your own email v6 saying Valdemar recommended FGV Ventures.
  - Action: verbal/email confirmation from Valdemar that he agrees to be listed in the form + commit to sign a support letter.
  - Where: `programs/anthropic-ai-for-science/draft.md` §Team and institutional affiliation.

- [ ] **Authorize me to draft Valdemar's support letter.**
  - Format I'd produce: ~1 page in PT, formal but conversational, attesting (a) Otavio is a thesis advisee + alumni, (b) Novo CR is a personal research project of merit, (c) Valdemar is the institutional anchor for grant applications.
  - Recommendation: PT first since Valdemar reads it; translate to EN if Anthropic specifically requires English.

### 🟡 Verify (fact-checks)

- [ ] **"BSc Economics, 2025"** — is this the right title for your degree?
  - My inference: EPGE = Escola de Pós-Graduação em Economia → undergrad = BSc in Economics.
  - Where: `draft.md` §Team / Principal researcher.
  - If wrong: tell me the correct degree name; I update.

- [ ] **"Cysne encouraged the project's formal start in December 2025"** — bate com sua história?
  - Source: your email v6 to FGV Ventures says "O diretor Rubens Cysne me incentivou a iniciar o projeto, dezembro passado."
  - Where: `draft.md` §Team and `shared/team-and-credentials.md`.

- [ ] **Mario Andrade "13 years in the role" at CTAE.**
  - Source: `prova-ia-v2/docs/contatos/outreach.md` line 625 — "Coordenador Pedagógico CTAE FGV há 13 anos; também professor da rede estadual RJ desde 2007".
  - Where: `draft.md` §Team.

- [ ] **"~89% reduction in input tokens" via prompt caching at the CORRIGIR stage.**
  - Source: subagent extracted this from prova-ia-v2/ codebase analysis ("Otimização planejada: Prompt caching pode reduzir 89% dos tokens entrada em CORRIGIR para 30 alunos no mesmo gabarito").
  - Risk: confirm this 89% is from a stable analysis you trust, not a rough estimate that might change.
  - Where: `draft.md` §Use of Claude API.

- [ ] **Moacyr's EMAp data consent under Anthropic's "perpetual, irrevocable license to train".**
  - Source: Anthropic AI for Science Rules §"Data Handling & Research Use" — accepting credits means Anthropic can use Inputs/Outputs from the API for training.
  - Risk: data from prof. Moacyr's EMAp class flowing through the API while credits are used would fall under this license. Need Moacyr's explicit OK.
  - Where: blocks compliance check pre-submission.

- [ ] **SUBDEIS consent for personal research project.**
  - Source: Anthropic Rules — "you must have obtained all consents from that employer or institution".
  - My read: probably an informal notification to your boss suffices since the project is personal and pre-dates the SUBDEIS role. Verify with you / SUBDEIS HR.
  - Where: blocks compliance check pre-submission.

### 🔵 Decide

- [ ] **Allocation plan in §Estimated credit usage** — current split is 40% production / 30% cross-course refinement / 20% provider benchmark / 10% CNPq research.
  - My recommendation: keep as is.
  - Alternative: bump production to 50% if the FGV pilot looks more concrete in your view.

- [ ] **Tax implications of $20K USD API credits as a Brazilian resident.**
  - Source: Anthropic Rules — "API Credits may have different tax implications than cash prizes. Selected Researchers are solely responsible for determining whether receipt of API Credits creates any tax obligations."
  - Action only if selected — but worth a quick word with a contador to know what to expect.

---

## OpenAI Researcher Access

Status: draft v3 stable after autonomous loop. Loop paused pending your review.

### 🔴 Critical

- [ ] **Log into the smapply portal and copy the form fields to me.**
  - URL: https://openai.smapply.org/prog/openai_researcher_access_program/
  - Why I can't: portal exige login (Google or email).
  - Risk if skipped: same as Anthropic — draft é estruturado contra campos típicos.
  - Where: `programs/openai-researcher-access/draft.md`

- [ ] **Valdemar Pinho Neto agrees to be PRINCIPAL INVESTIGATOR (not just signatory).**
  - Source: OpenAI requirement "active affiliation to an academic institution" — Otavio as alumni does not satisfy this alone.
  - Why this is different from Anthropic: Anthropic accepts team with alumni member + faculty member. OpenAI's barrier seems stricter — Valdemar's role here is principal applicant, not co-applicant.
  - Action: explicit ask to Valdemar.
  - Where: `programs/openai-researcher-access/draft.md` §Principal investigator and team.

### 🟡 Verify (fact-checks)

- [ ] **OpenAI's Sharing & Publication Policy** — read before submission.
  - Source: OpenAI Researcher Access FAQ requires applicants to "review our sharing & publication policy" before applying.
  - Relevant to: how we attribute / publish results from credit-funded experiments, especially involving FGV data.
  - Action: open and skim the policy; flag any blockers.

- [ ] **OpenAI Data Usage / Training Rights on API inputs/outputs.**
  - Source: not disclosed in public FAQ; not stated in Granted AI mirror.
  - Status: open question — same risk as Anthropic but unclear if symmetric.
  - Action: read OpenAI's general API data policy + the program-specific terms inside the portal.

- [ ] **"Brazilian researchers... operate at a structural cost disadvantage compared to North American or European labs"** — bold claim in draft §Limited financial and institutional resources.
  - My intent: hits the priority signal "limited financial/institutional resources".
  - Risk: could sound like complaint. Verify wording fits your voice.
  - Where: `draft.md` §Limited financial and institutional resources.

### 🔵 Decide

- [ ] **Submission window.**
  - Next quarterly review: **June 2026** (first week).
  - Alternative: September 2026 (3 months later — adds CNPq credential after July 31 submission).
  - My recommendation: **June** — Valdemar conversation should be quick and the $1K is more about credentialing than financing; better to test the channel now.

- [ ] **Parallel narrative with Anthropic.**
  - Current framing in draft: "Not redundant — Anthropic credits target Claude-specific optimizations, OpenAI credits target GPT-specific evaluation."
  - My recommendation: keep this disclosure; some grant programs penalize undisclosed parallel applications.

---

## Google Cloud Research Credits

Status: draft v3 stable (220-word proposal under the 250 limit). Loop paused. Operational pendencies are heavy (billing account + pricing calculator).

### 🔴 Critical

- [ ] **Valdemar Pinho Neto agrees to be applicant of record (Faculty).**
  - Source: program eligibility — "limited to faculty, PhD students and postdoctoral researchers"; alumni not on the list of accepted job titles.
  - Why this is different: at OpenAI, Valdemar as PI is recommended; at GCP, it's the only path. The credits go INTO FGV's billing account on Valdemar's representation.
  - Action: explicit ask + Faculty representation Valdemar must sign at submission.

- [ ] **Obtain Google Cloud Billing Account ID — institutional FGV (max 25 characters).**
  - Source: form requires this field; faculty representation states credits used "on behalf of the educational entity".
  - Action: coordinate with EPGE financial/IT to either reuse an existing FGV institutional GCP billing account or open one.
  - Risk: this can take weeks to set up via institutional channels. May block submission if not ready.
  - Where used: form identification fields.

- [ ] **Generate expected cost estimate via Google's pricing calculator + share URL.**
  - Source: form requires this URL.
  - Tools needed: Google's pricing calculator (https://cloud.google.com/products/calculator) configured for projected Gemini API usage.
  - My current rough estimate: ~5,000–10,000 exam-equivalents at ~$0.19 Gemini Flash full pipeline.
  - Action: someone with GCP access creates a saved estimate; URL goes into the form.

### 🟡 Verify (fact-checks)

- [ ] **Email field — Valdemar's institutional FGV email.**
  - My placeholder: "(Valdemar's @fgv.br institutional address)".
  - Form prefers "institution account".

- [ ] **Project start date — when?**
  - Implication: activation must happen within 60 days of start date.
  - Recommendation: align with grant decision (start ~30 days after expected notification).

- [ ] **Department name in form — "EPGE — Graduate School of Economics" — is this FGV's accepted English name?**
  - My inference: from public FGV materials.

### 🔵 Decide

- [ ] **Field of Research: Computer Science vs Social Sciences?**
  - My recommendation: **Computer Science** (Google emphasizes CS for AI research; consistent with how Anthropic/OpenAI applications frame the work).
  - Alternative: Social Sciences (more aligned with the longitudinal education aspect; less aligned with Google's typical research credit awards which lean technical).

- [ ] **Submission timing.**
  - Application is rolling — no specific window.
  - My recommendation: submit **after** the billing account is set up (probably 1–2 months from now). Don't submit incomplete.

- [ ] **Award amount expectations.**
  - Google doesn't publish the amount per applicant. Public reports vary widely ($5K–$50K typical for academic AI research; outliers higher).
  - Implication for narrative: don't assume amount; ask for what the project actually needs (which the timeline + costs imply).

---

## Google Cloud Start

Status: **blocker fundamental** — programa requer empresa incorporada. Otavio não tem. Draft v1 esqueletal documenta o cenário hipotético; não submetido.

### 🔵 Decide (this is the only category that applies — the program itself is blocked until decision)

- [ ] **Decidir se incorporar empresa pro Novo CR.**
  - Source: Google Cloud Start tier requires "less than 5 years from incorporation" + "legitimate business" verification via website.
  - Coupling: same decision unlocks **OpenAI for Startups** ($2.5K-$5K), **Google Cloud Scale** ($200K, needs VC too), and potentially **AWS Activate** / **Microsoft Founders Hub** later.
  - Recommendation: **postpone until FGV Ventures responds.** If accepted to batch 20, incorporation becomes natural (FGV Ventures uses Gust ecosystem). If rejected, evaluate standalone.
  - Where: blocks `programs/google-cloud-start/draft.md`.

- [ ] **If incorporating: MEI vs Ltda.**
  - MEI: ~R$0/year registration, ~R$70/month, but has revenue/activity restrictions that may not fit EdTech.
  - Ltda: ~R$2K-5K initial + ~R$500-1500/month accounting; more flexible.
  - Action: consult an accountant.

### 🟡 Verify (only relevant if incorporating)

- [ ] **The "no educational institutions" restriction.** Once Otavio incorporates as a private EdTech company (not FGV-owned), this restriction doesn't apply. But framing has to be careful — application should describe the company, not the academic affiliation.

---

## FGV Ventures batch 20

(populated after Phase 4)

---

## Closed items

(Items will move here once resolved; keeps history without cluttering active sections.)
