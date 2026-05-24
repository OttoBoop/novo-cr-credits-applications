# OpenAI Researcher Access Program — Exigências e fit do Novo CR

Análise pareada: exigências formais (verbatim das fontes oficiais) vs estado do Novo CR.

## Fontes consultadas (2026-05-24)

- FAQ oficial (via WebSearch, página retorna 403): https://help.openai.com/en/articles/10139500-researcher-access-program-faq
- Granted AI mirror: https://grantedai.com/grants/openai-researcher-access-program-api-credits-openai-group-c2fd0099
- Portal de submissão (auth-walled): https://openai.smapply.org/prog/openai_researcher_access_program/
- Docs do projeto: `shared/project-description.md`, `shared/team-and-credentials.md`, `shared/voice-anchors.md`, `shared/framing-principle.md`

---

# Parte 1 — Exigências detalhadas

## 1.1 Quem pode aplicar

Verbatim:
> "Researcher(s) with an active affiliation to an academic institution or other research organization, as well as nonprofits conducting research activities (not operational support) are eligible to apply."

Aplicantes baseados em "countries supported by our API" (Brasil suportado, sem exclusão).

## 1.2 Áreas de pesquisa de interesse

Listadas:
- Alignment
- Fairness & representation
- Societal impact
- Interdisciplinary research
- Interpretability / transparency
- Misuse potential
- Robustness

## 1.3 Foco priorizado

Verbatim:
> "OpenAI is especially interested in subsidizing work from researchers with limited financial and institutional resources."

Sinal explícito: **early-stage researchers** com recursos limitados.

## 1.4 O que oferece

- Até **$1.000** em créditos da API
- Validade **12 meses**
- Modelos publicamente disponíveis (sem fine-tuning, sem experimentais)
- **Não renovável, não extensível**

## 1.5 Ciclo de avaliação

- Revisão trimestral: **Março, Junho, Setembro, Dezembro**
- **Próxima janela: junho 2026**
- Turnaround: 4–6 semanas após a janela fechar

## 1.6 Compromissos

- Compliance com Usage Policy + applicable OpenAI policies
- Compliance com OpenAI "sharing & publication policy" — **a ler antes de submeter**, especialmente porque trata de uso de dados de FGV
- Dados/training rights da OpenAI sobre Inputs/Outputs: **não disclosed explicitamente** nas fontes públicas

---

# Parte 2 — Fit pareado

## 2.1 "Active affiliation to an academic institution"

| Item | Estado | Veredito |
|---|---|---|
| Otavio como pesquisador principal | Alumni EPGE/FGV (2025) — não conta como "active affiliation" stricto sensu | ❌ Sozinho não passa |
| Otavio + Valdemar como team | Valdemar é coord. graduação EPGE + faculty ativo → Valdemar como aplicante principal, Otavio como pesquisador associado | ✅ Forte (com Valdemar como PI) |
| FGV/EPGE como instituição | Reconhecida globalmente | ✅ Forte |

**Implicação:** OpenAI Researcher Access requer Valdemar como aplicante principal (não apenas signatário). Diferente de Anthropic, onde o team pode ter um membro alumni e outro faculty. Aqui o "active affiliation" parece mais estrito.

Fonte: [`shared/framing-principle.md`](../../shared/framing-principle.md), [`shared/team-and-credentials.md`](../../shared/team-and-credentials.md).

## 2.2 "Limited financial and institutional resources"

| Item | Estado | Veredito |
|---|---|---|
| Projeto pessoal sem funding institucional | Verdade — custos de API saem do bolso do Otavio | ✅ Forte |
| Brasil + projeto sem investimento externo | Sinal natural de recursos limitados na avaliação | ✅ Forte |
| Estágio (early-stage) | Otavio formado 2025, projeto rodando há menos de 1 ano em escala pequena | ✅ Forte |

## 2.3 Áreas de pesquisa

| Área OpenAI | Conexão com Novo CR | Veredito |
|---|---|---|
| Alignment | Pouca conexão direta | — |
| Fairness & representation | Indireta — sistema lida com avaliação educacional onde fairness é relevante | ⚠️ Mencionável |
| **Societal impact** | Direta — educação baseada em dados longitudinais, extensões pra detecção de risco escolar, medidas socioeducativas, proteção infantil | ✅ Forte |
| **Interdisciplinary research** | Direta — econ + applied math + pedagogia + AI engineering | ✅ Forte |
| Interpretability / transparency | Indireta — pipeline 6 etapas transparente, sem black box, cada etapa gera documento visível | ✅ Razoável |
| Misuse potential | Pouca conexão; aplicação não envolve risco de uso indevido | — |
| Robustness | Indireta — multi-provider em paralelo é uma forma de robustness | ⚠️ Mencionável |

**Hooks fortes:** societal impact + interdisciplinary research + interpretability (via pipeline transparente).

## 2.4 Uso da API

| Aspecto | Estado | Veredito |
|---|---|---|
| Uso real existente | GPT-5 family configurado e rodando em produção como um dos 3 providers no pipeline | ✅ Forte |
| Modelos publicamente disponíveis | GPT-5, GPT-5-mini, o3-mini — todos públicos | ✅ Forte |
| Sem fine-tuning | Não usamos | ✅ Compatível |

## 2.5 Coerência com Anthropic (peças similares)

| Aspecto | Anthropic | OpenAI |
|---|---|---|
| Valor | $20K | $1K |
| Afiliação | Pode aceitar team com membro alumni + faculty | Exige "active" — Valdemar como PI |
| Foco | Bio/life sciences (cat. "Other fields" pra Novo CR) | Societal impact + interdisciplinary (mais alinhado) |
| Cycle | Mensal | Trimestral (junho próxima) |

**Estratégia paralela:** as duas aplicações podem rodar em paralelo se Valdemar topar duplo papel — co-aplicante em Anthropic, PI em OpenAI. As narrativas se reforçam.

---

# Parte 3 — Síntese

## 3.1 Resumo do fit

| Dimensão | Veredito |
|---|---|
| Elegibilidade institucional | ⚠️ Aberto — exige Valdemar como PI ativo, não apenas signatário |
| Área de pesquisa | ✅ Forte (societal impact + interdisciplinary alinham com Novo CR) |
| Recursos limitados | ✅ Forte (projeto pessoal, sem funding) |
| Uso real da API | ✅ Forte (GPT-5 em produção) |
| Valor | ⚠️ $1K é simbólico vs. tempo de aplicação |

## 3.2 Probabilidade subjetiva

**Estimativa:** ~40-50% na primeira tentativa (junho).

Justificativa:
- A favor: três sinais que OpenAI explicitamente prioriza (early-stage + recursos limitados + interdisciplinary). Sistema rodando com OpenAI já. Projeto está claramente fora do mainstream bio-heavy.
- Contra: precisa Valdemar como PI; a barra "active affiliation" é mais estrita. Valor baixo ($1K) significa que talvez a OpenAI seja seletiva (poucos slots).
- Comparação: Anthropic AI for Science (que é mais caro) tem barra de afiliação mais flexível; OpenAI Researcher Access (que é barato) tem barra mais estrita. Faz sentido — o programa mais barato é mais distribuído entre mais aplicantes.

## 3.3 Posicionamento recomendado

1. **Valdemar como aplicante principal**, Otavio como pesquisador associado / co-aplicante.
2. **Enquadrar como pesquisa de societal impact + interdisciplinary** — não como EdTech.
3. **Liderar com transparência metodológica** (pipeline 6 etapas, cada etapa gera documento visível). Isso tica também "interpretability".
4. **Mencionar a extensão pra detecção de risco escolar** com peso maior aqui do que na Anthropic — societal impact é o slot principal e isso é caso forte.
5. **Frase âncora possível** (verbatim do Otavio): "Eu quero avisar o humano certo na situação certa." (`shared/voice-anchors.md` M4)
6. **Honestidade técnica:** OpenAI já roda no sistema; os créditos são pra evaluar GPT-5 vs alternativas por etapa e refinar o uso pra escala.

## 3.4 Pendências pré-submissão (vão pra REVIEW.md)

| Item | Quem | Quando |
|---|---|---|
| Otavio loga no smapply portal e copia campos do form | Otavio | Pré-submissão |
| Valdemar topa ser aplicante principal (não só signatário) | Otavio → Valdemar | Pré-submissão |
| Ler "sharing & publication policy" da OpenAI | Otavio + Ariadne | Pré-submissão |
| Decidir se submete em junho (próxima janela) ou setembro | Otavio | Após Valdemar topar |

## 3.5 Open questions

1. **"Active affiliation"** aceita alumni que conduz projeto sob supervisão de faculty ativo? Ou exige stricto sensu que o aplicante principal seja faculty?
2. **Data usage policy:** OpenAI usa Inputs/Outputs pra training como Anthropic faz no AI for Science? Não disclosed nas fontes públicas.
3. **Sharing & publication policy:** o que se compromete a publicar / atribuir?

---

## Próximo passo

Abrir `draft.md` e produzir v1 da proposta. Estrutura provável (sem ver o form ainda): título, abstract, team & affiliation, área de pesquisa (societal impact + interdisciplinary), uso da API, impacto esperado, recursos limitados (declaração).
