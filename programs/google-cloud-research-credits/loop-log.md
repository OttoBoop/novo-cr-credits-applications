# Google Cloud Research Credits — Loop log

Log das ações do loop autônomo de aplicação (Otavio ocupado, revisão futura via REVIEW.md).

---

## Sessão única — 2026-05-24

### A1 — WebFetch detalhado da página oficial

URL: https://edu.google.com/programs/credits/research/
Resultado: extração completa em uma única chamada (página acessível sem auth).

Achados-chave novos vs. notas iniciais:
- **Brasil aprovado** explicitamente na lista de países.
- **Eligibility stricta:** Faculty / Postdoc / PhD Student / IT Admin. **Alumni não está na lista.**
- **Lista completa dos campos do formulário** capturada — diferente de OpenAI/Anthropic onde o form é gated.
- **Proposal limite: 250 palavras.** Constraint crítico.
- **Billing Account ID obrigatório** no momento da aplicação (max 25 chars).
- **Pricing calculator URL** obrigatório.
- **Post-expiration funding plan** é campo do form.
- **Validade:** 365 dias após resgate; ativação em 60 dias após project start date.
- **Field of Research:** Social Sciences listado — categoria possível alongside CS.

### A2 — Update `criteria.md`

Expandido com:
- Verbatim dos critérios de eligibility.
- Lista completa dos campos obrigatórios + opcionais do form.
- Conteúdo requerido do proposal (verbatim).
- Restrições de uso (non-transferable, non-commercial, on behalf of educational entity).
- Compliance reps.
- Field of Research options.
- Pontos críticos identificados: job title bloqueante para Otavio sozinho, exige Valdemar como aplicante direto.

### A3 — Escrever `requirements-and-fit.md`

Estrutura padrão 3 partes (exigências verbatim → fit pareado → síntese).

Conclusões principais:
- Valdemar como Faculty é a única via.
- Field of Research = Computer Science (mais aderente que Social Sciences para AI research no Google).
- Intended Credit Application = Evaluation/Comparison (uso central honesto dos créditos).
- Probabilidade subjetiva: 35-45%. Constraint de 250 palavras eleva risco de erro.

Pendências adicionais identificadas:
- GCP Billing Account ID institucional FGV — pendência operacional pesada
- Pricing calculator — exige acesso pra rodar
- Post-expiration funding plan — exige decisão de framing

### A4 — Escrever `draft.md` v1

Primeira versão escrita rapidamente:
- Bloco de identification fields (Valdemar como aplicante)
- Project name, field of research, intended credit application
- Proposal de ~222 palavras

### A5 — Auto-crítica de v1

Achados:
1. "AI-assisted educational assessment" — leve jargão; verificar se substituir.
2. "trajectory has been generated as proof of concept" — slightly awkward. "already been produced" é mais natural.
3. "GCP credits would fund production-scale evaluation of Gemini at each of the six pipeline stages (extraction, classification, narrative report)" — listou 3, mas o pipeline tem 6 stages. Mismatch.
4. "Post-expiration: continued via CNPq funding if accepted" — vago. Pode ser mais concreto.

### A6 — Escrever `draft.md` v2 (deltas)

Mudanças:
- "has been generated as proof of concept" → "has already been produced as proof of concept"
- Listagem específica do silo (child welfare councils, juvenile justice system) — mais concreta
- "missing batch pipeline" — mais concreto
- Post-expiration agora menciona 4 fontes (CNPq + cost reductions + pilot deployment paths + institutional discussions)

### A7 — Auto-crítica de v2

Achados:
1. "at each of the six pipeline stages (question extraction, answer-key extraction, response extraction, correction, skill analysis, narrative report)" — expandi listar todas as 6 etapas, mas isso come ~12 palavras só pra parenthetical. Em 250 palavras limit, é caro.
2. Geral: balanço OK; o constraint de 250 palavras força disciplina.

### A8 — Escrever `draft.md` v3 (delta)

Mudanças:
- Cortei o parenthetical dos 6 stages, deixei só "at each of six pipeline stages". Economizou ~12 palavras.
- Word count final: ~221 palavras.

### A9 — Pendências geradas (para REVIEW.md)

- 🔴 Critical: Valdemar como aplicante direto (Faculty), não signatário
- 🔴 Critical: GCP Billing Account ID institucional FGV (FGV TI/financeiro)
- 🔴 Critical: Pricing calculator URL com estimativa
- 🟡 Verify: Field of Research — Computer Science vs Social Sciences
- 🟡 Verify: Project start date a definir
- 🟡 Verify: Email institucional Valdemar @fgv.br
- 🔵 Decide: Award amount não publicado — aplicar mesmo sem saber valor esperado

### A10 — Commit

Arquivos: `criteria.md` (expandido), `requirements-and-fit.md` (novo), `draft.md` (v3), `loop-log.md` (este).

---

(Loop Google Cloud Research Credits fechado em v3. Próxima ação: Otavio decide se Valdemar topa + FGV TI disponibiliza Billing Account.)
