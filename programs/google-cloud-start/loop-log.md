# Google Cloud Start — Loop log

Loop curto justificado pelo blocker fundamental (sem incorporação). Não iterar até decisão estratégica.

---

## Sessão única — 2026-05-24

### A1 — WebFetch tentativas

URLs tentadas, todas truncaram via WebFetch:
- https://cloud.google.com/startup/benefits
- https://cloud.google.com/startup/pre-funded
- https://cloud.google.com/startup/early-stage

Mensagem padrão: "Content truncated due to length...".

### A2 — WebSearch fallback

Query: `"Google for Startups Cloud" Start tier 2026 $2000 credits eligibility application "less than 5 years"`

Achados consolidados:
- $2,000 GCP credits + $200 training credits (12 meses)
- Idade < 5 anos da **incorporação** (não do projeto)
- Sem funding VC institucional
- Website funcional verificável
- One-time benefit (não renovável)
- Restrição geral do programa: "Google does not accept educational institutions, government entities, nonprofits"

### A3 — Diagnóstico do blocker

**Otavio não tem empresa incorporada.** O Novo CR é projeto pessoal de pesquisa + alumni FGV.

Para aplicar:
1. Incorporar uma empresa (MEI vs Ltda — custo e operação variáveis)
2. Ter CNPJ, conta empresarial, contabilidade
3. Aplicar com a empresa, não com Otavio pessoa física

Esta é uma decisão estratégica grande pra um ganho de $2.200 isolado.

### A4 — Escrever `criteria.md`

Catalogado com:
- Critérios verbatim (consolidados de fontes públicas)
- Restrição do programa "no educational institutions" — relevante apenas se Novo CR for descrito como projeto FGV; OK se for empresa privada
- Hipotético encaixe se incorporasse
- Pendências (decisão sobre incorporação, MEI vs Ltda)

### A5 — Escrever `requirements-and-fit.md`

Loop curto: análise de fit + decisão estratégica.

Recomendação: **adiar.** Acoplar decisão com FGV Ventures + OpenAI for Startups — se incorporar pra um, faz sentido aplicar a todos.

### A6 — Escrever `draft.md` v1 esqueletal

Versão hipotética cobrindo o que iria no form se Otavio decidir incorporar. Não vai ser submetido agora. Loop curto não iterado (v1 stops here).

### A7 — Pendências geradas (para REVIEW.md)

- 🔵 Decide: Otavio incorpora empresa (acoplado a FGV Ventures + OpenAI Startups)
- 🟡 Verify: MEI vs Ltda — consultar contador

### A8 — Commit

Files: `criteria.md`, `requirements-and-fit.md`, `draft.md` (v1 esqueletal), `loop-log.md`.

---

(Loop Google Cloud Start pausado em v1 esqueletal. Retoma com decisão de incorporação.)
