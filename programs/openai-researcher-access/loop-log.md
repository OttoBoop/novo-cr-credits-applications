# OpenAI Researcher Access — Loop log

Log das ações da assistente (Ariadne/Claude Code) durante o loop autônomo (Otavio ocupado, revisão futura).

---

## Sessão única — 2026-05-24

### Contexto

Otavio autorizou (P2 da sessão da Anthropic) que eu rodasse loops autônomos pra demais programas, com pendências consolidadas em `REVIEW.md`. Anthropic já fechou em v3.

### A1 — WebFetch direto da página FAQ oficial

URL: https://help.openai.com/en/articles/10139500-researcher-access-program-faq
Resultado: **HTTP 403 Forbidden** (mesma falha do primeiro fetch da sessão anterior).

### A2 — WebSearch como fallback

Query: `"OpenAI Researcher Access Program" FAQ 2026 eligibility credits amount academic institution alumni`.

Achados consolidados de fontes públicas indexadas (incluindo Granted AI mirror):
- Elegibilidade: "active affiliation to an academic institution or other research organization", nonprofits OK.
- $1,000 em créditos, validade 12 meses, sem renovação.
- Foco priorizado: pesquisadores com recursos limitados (early-stage).
- Ciclo trimestral: Mar/Jun/Sep/Dec.
- Áreas de interesse: alignment, fairness, **societal impact**, **interdisciplinary research**, interpretability, misuse, robustness.

### A3 — WebFetch do Granted AI mirror

URL: https://grantedai.com/grants/openai-researcher-access-program-api-credits-openai-group-c2fd0099
Resultado: extração detalhada dos critérios de seleção e estrutura do programa.

### A4 — Update `criteria.md`

Expandido com:
- Verbatim de elegibilidade e foco priorizado.
- Lista verbatim das áreas de pesquisa de interesse.
- Detalhes do ciclo (Mar/Jun/Sep/Dec, próxima janela junho 2026).
- "Active affiliation" como ponto crítico vs Otavio (alumni) — exige Valdemar como PI ativo, não só signatário.
- Pendências marcadas (smapply form, sharing & publication policy, conversa Valdemar).

### A5 — Escrever `requirements-and-fit.md`

Mesma estrutura de 3 partes que Anthropic (exigências verbatim → fit pareado → síntese).

Achados-chave do fit:
- Otavio sozinho NÃO passa "active affiliation" — diferente de Anthropic. Aqui Valdemar precisa ser aplicante principal (não só signatário).
- 3 áreas alinhadas fortemente: Societal Impact, Interdisciplinary Research, Interpretability.
- Recursos limitados é match forte (sinal explícito da OpenAI).
- Probabilidade subjetiva: 40-50% — mais alta que Anthropic (~25-35%) porque áreas alinham melhor; mais baixa que poderia ser porque $1K é seletivo.

### A6 — Escrever `draft.md` v1

Primeira versão escrita em ~10 min com:
- Estrutura adaptada do draft Anthropic mas reorganizada pras prioridades da OpenAI.
- §Alignment with OpenAI's research priorities como bloco central (não estava na Anthropic).
- Tom mais conciso (~900 palavras vs ~1200 da Anthropic) porque grant é menor.

### A7 — Auto-crítica de v1

Achados:
1. **Inventado:** "OpenAI models... have shown advantages over alternatives in our internal benchmarks" — o subagente não encontrou benchmarks de GPT-5 vs outros providers. Cortar.
2. **Erro factual:** "via the principal investigator's own access through EPGE" — confundi PI (Valdemar) com co-investigator (Otavio). Quem importou os próprios dados eClass foi Otavio.
3. **Mismatch estrutural:** "Measured per-pipeline production costs:" introduzia bullets que NÃO eram custos, eram descritivos. Substituir a frase de abertura.

### A8 — Escrever `draft.md` v3 com correções

Mudanças aplicadas:
1. "Internal benchmarks" → "ongoing internal benchmarking exercise" + reformulação que NÃO afirma vantagem específica do GPT-5.
2. "the principal investigator's own access" → "the co-investigator imported his own undergraduate transcript".
3. Lead-in dos bullets de "Use of OpenAI API" simplificado: "Per-stage model assignment is parameterized... The requested credits would support: 1. ...".
4. Pequenos polimentos de coesão.

Decisão de pular v2 explícita: as 3 correções de v1 eram diretas (cortar invenção + corrigir atribuição + reformular lead-in), não justificavam ciclo intermediário. Em vez disso, parei em v3 estável.

### A9 — Pendências geradas (para REVIEW.md)

Itens novos:
- 🔴 Critical: Otavio logar no portal smapply.org e copiar campos do form
- 🔴 Critical: Valdemar topar ser **aplicante principal** (não só signatário) — barra mais estrita aqui
- 🔵 Decide: janela junho vs setembro
- 🟡 Verify: ler "sharing & publication policy" da OpenAI
- 🟡 Verify: data usage / training rights da OpenAI — não disclosed nas fontes públicas

### A10 — Commit

Files: `criteria.md` (expandido), `requirements-and-fit.md` (novo), `draft.md` (v3), `loop-log.md` (este).

---

(Loop OpenAI Researcher Access fechado. Próximas ações dependem da revisão do Otavio + dos campos reais do form smapply.org.)
