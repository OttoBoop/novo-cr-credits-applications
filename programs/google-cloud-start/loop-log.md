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

---

## Sessão 2 — maturação a v3 (2026-05-24)

### P3 — Otavio (autorização de maturação igual)

> "Vai fazendo os drafts! Registre os problemas! Eu quero todos igualmente maturos"

Interpretação: trazer Google Cloud Start de v1 esqueletal pra v3, mesmo nível de profundidade dos outros 3 drafts. O blocker de incorporação permanece — o draft fica "ready in content", não "ready to submit".

### A9 — Auto-crítica de v1 esqueletal

Itens identificados pra maturação:
1. **Seção "Eligibility note"** ausente. Adicionar nota upfront sobre o blocker pra leitor entender o estado.
2. **Identification fields** muito magros. Adicionar todos os campos típicos do form Google.
3. **Company description** muito curta (~3 frases). Expandir pra ~150-200 palavras como os outros drafts, com referência aos dados reais (18 disciplines, 26 subjects, 100+ activities, 7-page longitudinal report).
4. **Use of Google Cloud** sem números. Trazer custos medidos do subagent (Gemini 3 Flash ~$0.19, baseline 28 runs).
5. **Founder credentials** sem rede acadêmica completa. Adicionar Cysne / Moacyr / Mario Andrade como outros drafts fazem.
6. **Roadmap** ausente. Adicionar tabela de fases.
7. **Why this tier** ausente. Justificar Start vs Scale/AI tier (gating de VC funding).
8. **Additional context** mais robusto. Cross-reference com outras aplicações (Anthropic / OpenAI Researcher / CNPq) — declarar paralelo é prática boa.

### A10 — Escrever v2 (deltas)

Mudanças:
- Adicionada "Eligibility note (read first)" no topo
- Identification fields expandido (11 linhas)
- Company description expandida pra 2 parágrafos com fatos reais do projeto
- Use of Gemini/Cloud com custos medidos + 3 bullets de uso dos créditos
- Founder credentials com rede acadêmica completa
- Roadmap em tabela com 5 fases
- Why this tier explicit (justifica não-elegibilidade Scale/AI)
- Additional context cross-references outras aplicações

### A11 — Auto-crítica de v2

Itens menores:
1. "Otavio's CPF" — referenciar CPF na hipótese MEI pode ser sensível; manter genérico ("MEI under Otavio's CPF" → manter, é hipotético).
2. "Vertex AI exploration" — claim novo. Tem como sustentar? Sim — Vertex é o produto Google natural pra batch + structured workflows. Mantém como hipótese declarada ("may offer the missing automation layer"), não como fato.
3. "8–9 months ... Batch automation of longitudinal report" — overlap com "6 months post-incorporation: Per-stage Gemini benchmark report" — clarificar que são fases paralelas/sequenciais.

### A12 — Escrever v3 (ajuste fino do roadmap)

Mudanças mínimas:
- Roadmap reformulado pra ficar mais claro nas durações: "6 months post-incorporation", "6–9 months", "2027" — fluência temporal melhor.
- Mantida hedge em "Vertex AI exploration" ("may offer the missing automation layer").

### A13 — Decisão de parar em v3

v3 está no mesmo nível dos outros drafts. O blocker permanece operacional (incorporação), não editorial.

### A14 — Pendências atualizadas em REVIEW.md

Mantém os itens originais (incorporação como decisão estratégica). Adicionei sub-itens:
- Decisão MEI vs Ltda (consultar contador)
- Coupling com FGV Ventures (esperar resposta primeiro)
- Quando incorporar: aplicar simultaneamente a Google Start + OpenAI Startups + considerar AWS Activate, Microsoft Founders Hub, NVIDIA Inception

---

(v3 estável. Operational status: ready in content, awaits incorporation.)
