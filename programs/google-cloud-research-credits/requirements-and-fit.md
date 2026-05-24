# Google Cloud Research Credits — Exigências e fit do Novo CR

## Fonte (2026-05-24)

- Página oficial: https://edu.google.com/programs/credits/research/
- Docs do projeto: `shared/project-description.md`, `shared/team-and-credentials.md`, `shared/framing-principle.md`

---

# Parte 1 — Exigências detalhadas

Já catalogadas em [`criteria.md`](criteria.md). Resumo dos pontos críticos:

- **Job titles aceitos:** Faculty / Postdoc / PhD Student / IT Admin.
- **País:** Brasil aprovado.
- **Proposal:** máximo 250 palavras, deve incluir: problema, GCP tools, timeline, milestones/outcomes, como GCP suporta a pesquisa no futuro.
- **Billing account:** ID obrigatório no momento da aplicação.
- **Pricing calculator:** estimativa de uso obrigatória, com link.
- **Validade:** 365 dias a partir do resgate; ativação em até 60 dias.
- **Restrições:** uso institucional only (não pessoal); sem uso comercial.

---

# Parte 2 — Fit pareado

## 2.1 Quem aplica

| Item | Estado | Veredito |
|---|---|---|
| Job Title aceito | Otavio = alumni → **NÃO encaixa em nenhuma das 4 categorias** | ❌ Bloqueante sozinho |
| Solução | Valdemar Pinho Neto = Faculty (coord. graduação EPGE) → aplica como Faculty | ✅ Forte com Valdemar como aplicante |
| Alternativa | Cysne (Faculty, diretor EPGE) — mais sênior, menos direto na operação | ⚠️ Backup |
| Alternativa 2 | Moacyr (Faculty, EMAp) — diferente escola da FGV, possível pra ângulo applied math | ⚠️ Backup |

**Decisão recomendada:** Valdemar como aplicante (continuidade com Anthropic + OpenAI loops).

## 2.2 Field of Research

| Categoria | Conexão com Novo CR | Veredito |
|---|---|---|
| Computer Science | Pipeline AI multi-provider, classification + structured output, schema longitudinal cross-curso | ✅ Forte |
| Social Sciences | Educação como aplicação de pesquisa em learning sciences | ✅ Forte |
| Outras (Bio, Chemistry, etc.) | Não aplicável | — |

**Decisão:** CS é mais aderente pro programa Google Research Credits (Google enfatiza CS pra AI research). Mencionar "education as applied research domain" no proposal.

## 2.3 Intended Credit Application

| Opção | Encaixa? | Por quê |
|---|---|---|
| Proof of concept | ✅ Forte | Sistema já em produção; créditos extendem POC pra mais matérias/turmas |
| **Evaluation/Comparison** | ✅ Forte | Multi-provider benchmarking é uso central — comparar Gemini vs Claude vs GPT-5 por etapa |
| Workshop or Training | ⚠️ Possível | Se pretendêssemos rodar workshops na FGV |
| Developing Open Source Software | ⚠️ Possível | NOVO CR não é OSS hoje; poderia ser declarado como intenção |

**Decisão:** "Evaluation/Comparison" é a categoria mais honesta. POC é redundante com o que já existe.

## 2.4 Infrastructure

| Item | Estado | Veredito |
|---|---|---|
| GCP Billing Account ID | Otavio não tem conta institucional FGV; pode ter conta pessoal mas Faculty Rep diz "on behalf of educational entity" — exige conta institucional | ⚠️ Pendência operacional pesada |
| Pricing calculator | Precisa rodar pra estimar uso Gemini API no pipeline | ⚠️ Pendência (calcular antes) |

**Risco:** o billing account institucional FGV pode demorar pra obter via TI/financeiro. Se isso virar gargalo, considerar adiar pra após CNPq julho.

## 2.5 Uso real de Gemini

| Aspecto | Estado | Veredito |
|---|---|---|
| Gemini já no sistema | Sim — Gemini 3 Flash e Gemini 2.5 Flash medidos em produção | ✅ Forte |
| Custos medidos | Gemini 3 Flash full pipeline: ~$0.19; Google Flash (Beatriz): ~$0.11 | ✅ Forte |
| Total Google em 28 runs | $0.49 | ✅ Forte |

Diferenciação útil: enquanto Anthropic Researcher credits focam em Claude e OpenAI Researcher Access em GPT, os Google Research Credits cobrem o terceiro provider que já roda no sistema — completa o trifecta.

## 2.6 Post-expiration funding plan

Possibilidades a declarar:
- Funding do **CNPq Jovem Cientista** (se aceito após submissão julho).
- Continuidade via **FGV institutional support** (depende de discussão com Valdemar/Cysne sobre como FGV institucionaliza apoio).
- **FGV Ventures** se aceito no batch 20 (pode trazer outras formas de funding).
- **Capacidade própria de continuar** com custo de bolso reduzido pós-otimizações de prompt caching.

---

# Parte 3 — Síntese

## 3.1 Resumo do fit

| Dimensão | Veredito |
|---|---|
| Elegibilidade (job title) | ⚠️ Exige Valdemar como aplicante direto, não signatário |
| País | ✅ Forte (Brasil aprovado) |
| Field of research | ✅ Forte (CS + Social Sciences) |
| Intended credit application | ✅ Forte (Evaluation/Comparison) |
| Uso real de Gemini | ✅ Forte (em produção) |
| Billing account institucional | ⚠️ Pendência pesada (FGV TI) |
| Pricing calculator | ⚠️ Pendência |
| 250-word proposal | ✅ Exigirá redação cirúrgica |

## 3.2 Probabilidade subjetiva

**Estimativa:** ~35-45% — depende fortemente da execução do proposal de 250 palavras e da disponibilidade do billing account institucional.

Justificativa:
- A favor: Brasil aprovado, Gemini já no sistema, dados longitudinais reais, Valdemar como Faculty.
- Contra: 250 palavras é muito pouco pra contar a história completa; competição por créditos GCP é forte; "post-expiration funding plan" pode soar fraco sem CNPq já aprovado.

## 3.3 Posicionamento recomendado

1. **Valdemar como aplicante (Faculty), FGV/EPGE como organização.**
2. **Field of Research: Computer Science.**
3. **Intended Credit Application: Evaluation/Comparison** — uso central dos créditos é benchmarkar Gemini vs alternativas por etapa do pipeline.
4. **Proposal (250 palavras) — estrutura proposta:**
   - 1 frase: o problema (dados educacionais em silos longitudinais)
   - 2-3 frases: o sistema (em produção, métricas, schema)
   - 2-3 frases: o que os créditos GCP viabilizam (evaluation de Gemini por etapa)
   - 1-2 frases: outcomes esperados + continuidade pós-expiração
5. **Frase âncora possível** (verbatim do Otavio): "Mais que um número" pode aparecer como tagline curta se sobrar espaço.

## 3.4 Pendências pré-submissão (vão pra REVIEW.md)

| Item | Quem |
|---|---|
| Valdemar topa ser aplicante direto (Faculty) | Otavio → Valdemar |
| GCP Billing Account ID institucional FGV | FGV TI / EPGE financeiro |
| Pricing calculator URL com estimativa | Ariadne pode estimar; URL final depende do Otavio ter acesso ao calculator |
| Post-expiration funding plan: definir narrativa | Otavio decide framing |
| Field of research: confirmar CS ou Social Sciences | Otavio (preferência estratégica) |

## 3.5 Open questions

1. **FGV institucionalmente aceita ser entidade de aplicação?** Há restrições internas FGV sobre receber créditos cloud em nome da instituição?
2. **GCP Billing Account ID:** existe um da FGV ativo, ou precisa criar?
3. **Award amount típico:** Google não publica; precisa pesquisar relatos de outros aplicantes.

---

## Próximo passo

Abrir `draft.md` e produzir o proposal de 250 palavras + texto auxiliar pros campos do form (Project Name, milestones, post-expiration plan). Loop curto (v1 → v3) — o constraint de 250 palavras torna iteração mais valiosa.
