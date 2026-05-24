# SOURCES.md — mapa de origem dos materiais

Este repo é **derivado**. A fonte de verdade do projeto está em `prova-ia-v2/`. Os arquivos em `shared/` foram extraídos/curados a partir das fontes originais — quando algum fato mudar, atualizar primeiro a fonte original, depois sincronizar aqui.

## Repo do produto

**`/home/otavio/Documents/vscode/prova-ia-v2/`** — código + docs do Novo CR. Não modificar daqui.

## Mapa de derivação

| Arquivo neste repo | Derivado de (em `prova-ia-v2/`) | Quando atualizar |
|---|---|---|
| `shared/project-description.md` | `docs/missao.md` + apresentação `NOVO_CR_Apresentacao_v3.pptx_0.pdf` + email v6 (em `docs/contatos/`) | Quando a missão/visão for revisada |
| `shared/voice-anchors.md` | `docs/audit_quotes_vs_implementation.md` (D1–D10) + `docs/missao.md` (quotes em primeira pessoa) + `docs/prompts/sessao_*.md` | Quando novas quotes verbatim importantes aparecerem |
| `shared/team-and-credentials.md` | `docs/contatos/outreach.md` §G (Rede FGV) + email v6 do Otavio | Quando a rede mudar de status (novo apoiador, mudança de papel) |
| `shared/metrics-current.md` | API live (`https://ia-educacao-v2.onrender.com/api/materias`) + apresentação | Antes de cada aplicação a programa de crédito |
| `shared/framing-principle.md` | Decisão do Otavio na sessão de 2026-05-23 ("cidadão privado + alumni") | Quando o status muda (ex: incorporar empresa) |

## Documentos NÃO copiados (apenas referenciados)

Estes ficam onde estão; aplicações usam por referência ou anexo.

| Doc original | Conteúdo | Como usar em aplicações |
|---|---|---|
| `prova-ia-v2/docs/missao.md` | Visão raiz, princípios canônicos, voz Otavio | Fonte de quotes; referência conceitual |
| `prova-ia-v2/docs/contatos/outreach.md` | Inventário-mestre (727 linhas) — voz canônica, prova de execução, rede, princípios | Consulta quando shared/ não bastar |
| `prova-ia-v2/docs/contatos/fgv_ventures.md` | Dossiê FGV Ventures + email canônico v6 | É a "aplicação" do FGV Ventures batch 20. `programs/fgv-ventures-batch-20/` referencia este. |
| `prova-ia-v2/docs/audit_quotes_vs_implementation.md` | 10 quotes verbatim catalogadas + tabela de GAPs do tutorial | Fonte de `voice-anchors.md` |
| `prova-ia-v2/docs/plano_geral_novo_tutorial.md` | Plano mestre do tutorial em produção | Referência arquitetural |
| `prova-ia-v2/docs/plano_pipeline/11_decisoes_otavio.md` | 23 decisões + 15 correções verbatim do Otavio | Histórico técnico |
| `prova-ia-v2/docs/prompts/sessao_*.md` | Log verbatim de prompts por sessão | Fonte de quotes ainda não catalogadas |
| `prova-ia-v2/NOVO_CR_Apresentacao_v3.pptx_0.pdf` | 29 slides apresentação (tagline, pipeline, dados em produção, longitudinal) | Anexo padrão em aplicações |
| Site `https://ia-educacao-v2.onrender.com` | Fonte canônica de métricas em tempo real | Atualizar `shared/metrics-current.md` antes de aplicar |

## Como manter sincronização

- **Nunca duplicar voz do Otavio em texto novo** — citar verbatim de `voice-anchors.md` ou da fonte.
- **Atualizar `metrics-current.md`** antes de cada aplicação (comando no próprio arquivo).
- **Se uma fonte muda** em `prova-ia-v2/`, atualizar os derivados aqui no mesmo commit.
- **Não mover material do `prova-ia-v2/`** pra cá — esse repo é overlay de captação, não substituto do código/docs do produto.

## Programs/ — fontes web e nível de loop

| Programa | Fontes primárias | Nível de loop fechado |
|---|---|---|
| Anthropic AI for Science | support.claude.com + anthropic.com/ai-for-science-program-rules + anthropic.com/news/ai-for-science-program | Full (draft v3 stable) |
| OpenAI Researcher Access | help.openai.com (FAQ — 403 via WebFetch; via WebSearch) + smapply portal + grantedai mirror | Full (draft v3 stable) |
| Google Cloud Research Credits | edu.google.com/programs/credits/research/ (acessível direto) | Full (draft v3, 220 words under 250 limit) |
| Google Cloud Start | cloud.google.com/startup/* (truncado via WebFetch; via WebSearch) | Short — blocker de incorporação. v1 esqueletal |
| FGV Ventures batch 20 | prova-ia-v2/docs/contatos/fgv_ventures.md (overlay); status only neste repo | Status update only |

## Subagentes usados

- **2026-05-24:** Explore agent vasculhou `prova-ia-v2/` para custos de API. Resultado: per-pipeline costs por provider, baseline 28 runs em produção. Achados em `programs/anthropic-ai-for-science/loop-log.md` §A10 e `programs/google-cloud-research-credits/criteria.md`.
