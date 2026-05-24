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

(populated after Phase 1)

---

## Google Cloud Research Credits

(populated after Phase 2)

---

## Google Cloud Start

(populated after Phase 3)

---

## FGV Ventures batch 20

(populated after Phase 4)

---

## Closed items

(Items will move here once resolved; keeps history without cluttering active sections.)
