# Novo CR — Credits & Accelerator Applications

Workspace de captação para o Novo CR (plataforma de educação baseada em dados, em produção em ia-educacao-v2.onrender.com). Aplicações a programas de créditos gratuitos de provedores de IA e aceleradoras.

## Princípio de afiliação

Otavio aplica como **cidadão privado + alumni EPGE/FGV (2025)**.

- Trabalho na **SUBDEIS** (Subsecretaria de Desenvolvimento Econômico, Inovação e Simplificação, Prefeitura do Rio) e passagem prévia pelo **gabinete do vereador Flávio Valle** são **credenciais** (execução institucional, rede política), não afiliação.
- Programas de pesquisa (Anthropic AI for Science, OpenAI Researcher Access, Google Cloud Research Credits) exigem **professor signatário**: **Valdemar Pinho Neto** (coord. graduação EPGE, orientador TCC) é o signatário primário; Cysne e Moacyr conforme o programa.
- Programas de startup (OpenAI for Startups, Google Cloud Scale/AI Tier) dependem de **incorporação formal** — decisão futura.

Detalhe em [shared/framing-principle.md](shared/framing-principle.md).

## Estrutura

```
.
├── long_term_plan.md          # Objetivos de longo prazo, valores, cronograma
├── todos.md                   # Ações imediatas e backlog
│
├── shared/                    # Insumos canônicos pra qualquer aplicação
│   ├── framing-principle.md   # A regra cidadão privado / alumni / professor signatário
│   ├── team-and-credentials.md # Otavio + rede acadêmica FGV
│   ├── metrics-current.md     # Números do site + apresentação
│   ├── voice-anchors.md       # Quotes verbatim do Otavio (não inventar voz)
│   └── project-description.md # Peça canônica de 1 página
│
├── programs/                  # Uma pasta por programa
│   ├── anthropic-ai-for-science/
│   ├── openai-researcher-access/
│   ├── google-cloud-research-credits/
│   ├── google-cloud-start/
│   └── fgv-ventures-batch-20/
│
└── SOURCES.md                 # Mapa de ponteiros pra prova-ia-v2/docs/
```

## Como usar (loop de aplicação)

Antes de escrever uma aplicação X:

1. Reler `shared/project-description.md`, `shared/team-and-credentials.md`, `shared/voice-anchors.md`.
2. Reler `programs/X/criteria.md` — os critérios do programa em verbatim.
3. Iterar em `programs/X/draft.md`, registrando crítica em `programs/X/loop-log.md`.

`shared/` é a Phase 0. `programs/X/criteria.md` é a âncora externa. `programs/X/draft.md` é o equivalente ao "v6" (versão canônica que itera). `programs/X/loop-log.md` é o histórico explícito.
