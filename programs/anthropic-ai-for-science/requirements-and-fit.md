# Anthropic AI for Science — Exigências e fit do Novo CR

Análise pareada: exigências formais do programa (verbatim das fontes oficiais) vs estado atual do Novo CR (referenciando `shared/*` neste repo).

## Fontes consultadas (2026-05-24)

- Página de suporte: https://support.claude.com/en/articles/11199177-anthropic-s-ai-for-science-program
- Regras oficiais: https://www.anthropic.com/ai-for-science-program-rules (última atualização: 18 fev 2026)
- Anúncio: https://www.anthropic.com/news/ai-for-science-program (lançamento: 5 mai 2025)
- Documentos do projeto: `shared/project-description.md`, `shared/team-and-credentials.md`, `shared/voice-anchors.md`, `shared/framing-principle.md`, `shared/metrics-current.md`
- Documentos canônicos do Novo CR: `prova-ia-v2/docs/missao.md`, `prova-ia-v2/docs/audit_quotes_vs_implementation.md`

---

# Parte 1 — Exigências detalhadas

## 1.1 Quem pode aplicar

Verbatim das regras:
> "If you are an individual, then you must be at least 18 years of age"
> "If you are employed by a legal entity or affiliated with a university or other research institution, then you represent and warrant that you have obtained all consents from that employer or institution necessary to participate"
> "researchers attached to research institutions working on high-impact scientific projects"

Limitado a: "academia and nonprofit organizations" (page de suporte).

**Países excluídos** (regras):
> "You may not be a legal resident of Belarus, China, Cuba, Iran, Myanmar, North Korea, Russia, Sudan, Syria, Crimea, and the so-called Donetsk People's Republic or Luhansk People's Republic"

Brasil: não excluído.

## 1.2 Áreas de pesquisa aceitas

Ordem exata da página de suporte:
1. Biology/Life Sciences
2. Chemistry
3. Medicine/Healthcare
4. Environmental Science
5. Physics
6. Computer Science
7. Earth Sciences
8. "Other fields with potential for significant scientific impact"

Foco prioritário declarado:
> "We are particularly interested in applications where Claude can assist with understanding complex biological systems, accelerating drug discovery, analyzing genetic data, and other life sciences applications."

O anúncio público (anthropic.com/news) menciona somente bio/life sciences, drug discovery e agricultural productivity — **não menciona** Computer Science nem "Other fields" como áreas alvo. A inclusão dessas áreas só aparece na página operacional de suporte.

## 1.3 O que o programa oferece

> "up to $20,000 in API credits to your account for a 6-month period"
> "free API credits for our standard model suite"
> "Selected Researchers will receive Anthropic API credits ... placed in the account for the organization identified in your application"

Inclui: acesso à família Claude padrão via API.

Exclui:
> "This program does not provide access to non-standard or non-public models"
> "We do not currently provide finetuning access via an API at this time"
> "credits are for API use and do not apply to the Claude web app"

## 1.4 Critérios de seleção

Verbatim:
> "Scientific merit: team credentials in subject area and with AI, attached to a research institution"
> "Potential impact: contribution to critical foundational research and/or clear path to scale an application"
> "Technical feasibility: value of our model as applied to your use case"
> "Biosecurity screening: ensuring proposed research could not enable harmful applications"

Decisão é discricionária da Anthropic:
> "All judging decisions are final and binding. Anthropic reserves the right to disqualify any application at its sole discretion"

## 1.5 Ciclo de avaliação

> "On the first Monday of each month, Anthropic will select winning applications from among all eligible entries"
> "we regret that we cannot provide individual responses to unapproved submissions"

5 dias úteis pra responder à notificação. 14 dias corridos pra assinar affidavit.

## 1.6 Compromissos do aplicante aceito

**Licença de dados (perpétua e irrevogável):**
> "Selected Researchers represent and warrant that they have obtained all necessary permissions from their employer or institution to allow Anthropic to collect, analyze, train models on, and conduct research on all data, including Inputs and Outputs, generated from use of the API Credits"
> "By accepting API Credits, Selected Researchers grant Anthropic a perpetual, irrevocable license to use Program data for these purposes"

**Liberação de imagem e nome:**
> "you ... grant permission to Anthropic to use or publish your names, biographical information, photographs, voices and/or likenesses for advertising and promotional purposes worldwide in perpetuity without compensation or notification"

**Política de uso:**
> "Applicants through this program do not receive exemption from our Usage Policy. Our Trust & Safety team will follow our standard enforcement procedures"

**Status fiscal:**
> "API Credits awarded under this Program may have different tax implications than cash prizes. Selected Researchers are solely responsible for determining whether receipt of API Credits creates any tax obligations"

## 1.7 O que não está nas regras

- Política explícita de renovação após 6 meses: **não especificada**.
- Exemplos públicos de projetos aceitos: **não publicados**.
- Detalhes dos campos do Google Form: **não acessíveis sem submeter** (link: https://docs.google.com/forms/d/e/1FAIpQLSfwDGfVg2lHJ0cc0oF_ilEnjvr_r4_paYi7VLlr5cLNXASdvA/viewform).

---

# Parte 2 — Fit pareado com o Novo CR

Cada linha: requisito → estado atual → veredito → mitigação ou ação.

## 2.1 Aplicante = pesquisador afiliado a instituição

| Item | Estado | Veredito |
|---|---|---|
| Maior de 18 anos | Otavio é adulto | ✅ Forte |
| Afiliação a research institution | Otavio é **alumni EPGE/FGV (2025)**, não faculty. Mas o requisito é "attached to a research institution", e o programa aceita "team" — então **Valdemar Pinho Neto (coord. graduação EPGE, orientador de TCC, signatário primário)** entra como pesquisador afiliado. | ✅ Forte com co-aplicante |
| Consents do employer | Otavio é funcionário SUBDEIS (Prefeitura do Rio). O projeto é pessoal, mas as regras pedem "all consents from that employer or institution". | ⚠️ Aberto — verificar com SUBDEIS se requer ciência formal |
| Organização: academia/nonprofit | FGV via Valdemar = academia. SUBDEIS NÃO é organização aplicante; é credencial executiva. | ✅ Forte — desde que a aplicação seja submetida em nome do team com FGV como organização |
| Brasil não está excluído | Confirmado | ✅ Forte |

Fonte do Novo CR: [`shared/framing-principle.md`](../../shared/framing-principle.md), [`shared/team-and-credentials.md`](../../shared/team-and-credentials.md).

## 2.2 Área de pesquisa

| Item | Estado | Veredito |
|---|---|---|
| Área prioritária (bio/life sciences) | Novo CR é educação, não bio | ❌ Não se encaixa no foco |
| Áreas explicitamente listadas | "Computer Science" e "Other fields with potential for significant scientific impact" cobrem o caso | ⚠️ Médio — está na lista, mas não na prioridade |
| Anúncio público (bio-heavy) | Mensagem da marca é claramente bio. Compete por exceção na categoria "Other fields" | ⚠️ Risco real de filtro implícito |

**Posicionamento necessário:** o Novo CR precisa ser apresentado como **pesquisa em ciência de dados aplicada à educação longitudinal** — não como produto EdTech. O ângulo de "outras frentes além da pedagogia" (detecção de risco escolar, medidas socioeducativas, proteção infantil) tem componente de **ciência social aplicada e saúde pública** que pode reforçar o "significant scientific impact".

Fonte do Novo CR: [`shared/project-description.md`](../../shared/project-description.md), [`prova-ia-v2/docs/missao.md`](../../../prova-ia-v2/docs/missao.md).

## 2.3 Mérito científico

| Critério Anthropic | Estado do Novo CR | Veredito |
|---|---|---|
| Team credentials no assunto | Otavio: alumni EPGE, construiu sistema com 3 provedores em produção, 26 matérias, 100+ atividades, relatório longitudinal real de 9 disc/4 anos. Valdemar: economista, coord. graduação EPGE. Moacyr: matemático aplicado, EMAp. Cysne: diretor EPGE. | ✅ Forte mas heterogêneo (forte em economia/matemática aplicada, menos em learning sciences) |
| Team credentials com IA | Sistema rodando em produção com Claude/GPT-5/Gemini em paralelo, pipeline 6 etapas implementado | ✅ Forte (evidência operacional, não só teórica) |
| Foundational research | Schema longitudinal cross-curso é metodológico — junta dados que hoje vivem em silos. Há contribuição metodológica clara mas falta paper publicado | ⚠️ Médio — submissão CNPq julho ajuda |
| Path to scale | Implantação prevista em escola FGV 2027 + extensão pra rede municipal (SUBDEIS) e estadual (via gabinete Valle) | ✅ Forte (caminho concreto, não hipotético) |

## 2.4 Impacto potencial

| Aspecto | Estado | Veredito |
|---|---|---|
| Critical foundational research | Cross-curso como infra de dados longitudinais em educação | ⚠️ Médio — é genuíno mas não é o tipo de "foundational" que a Anthropic explicitamente prioriza (bio) |
| Clear path to scale | SUBDEIS (rede municipal Rio), vetor estadual (Paes), FGV (escola 2027) | ✅ Forte |
| Scientific publication | Submissão CNPq Jovem Cientista linha 3 (IA e Educação), prazo 31 jul | ⚠️ Pendente de execução; estará submetido antes da aplicação Anthropic se aplicarmos pós-julho |

## 2.5 Viabilidade técnica

| Aspecto | Estado | Veredito |
|---|---|---|
| Valor do modelo para o caso de uso | Pipeline 6 etapas já roda com Claude em produção (`ia-educacao-v2.onrender.com`). Multi-provedor implementado (Anthropic ao lado de OpenAI e Google) | ✅ Forte |
| Refinamento ainda pendente | Multi-provedor + relatório longitudinal cross-curso ainda precisam de refinamento | ⚠️ Honestidade exigida — declarar como item de refinamento que os créditos viabilizam |

Fonte: [`shared/metrics-current.md`](../../shared/metrics-current.md).

## 2.6 Biosecurity screening

| Aspecto | Estado | Veredito |
|---|---|---|
| Risco de "harmful applications" | Pipeline trata correção de provas + relatórios pedagógicos. **Não envolve** bioarmas, biossegurança, materiais perigosos ou síntese química | ✅ Forte (não tem vetor) |
| Dados sensíveis (crianças) | A extensão futura pra educação básica + proteção infantil envolve **dados de crianças e adolescentes** — LGPD se aplica com rigor especial. Mesmo que não seja "biosecurity", o tema requer cuidado | ⚠️ Anthropic provavelmente não veta, mas vale mencionar governança proativamente |

## 2.7 Compromissos pós-seleção

| Cláusula | Implicação prática para o Novo CR | Veredito |
|---|---|---|
| Licença perpétua para treinar em dados | A Anthropic pode treinar modelos com inputs/outputs gerados via os créditos. **Não inclui** os dados de FGV/eClass armazenados em outros lugares — só o que passa pela API durante o uso dos créditos | ⚠️ Aberto — verificar se há cláusula de consentimento do prof. Moacyr e do eClass para esse uso |
| Permissão de uso de nome/imagem | Anthropic pode publicar nome e biografia do Otavio + Valdemar pra promover o programa | ⚠️ Médio — provavelmente OK, mas é decisão pessoal |
| Compliance com Usage Policy | Padrão. Não há nada no Novo CR que viole policy padrão (não há geração de conteúdo nocivo, não há automação contra humanos) | ✅ Forte |
| Status fiscal | API credits podem ter implicação fiscal. Otavio precisa verificar com contador brasileiro se há obrigação tributária | ⚠️ Operacional — abrir tarefa |

## 2.8 Ciclo e prazo

| Item | Implicação | Veredito |
|---|---|---|
| Avaliação primeira segunda de cada mês | Otavio pode submeter em qualquer momento; primeira janela natural é **primeira segunda de junho 2026 (1 de junho)** | ✅ Forte (sem deadline rígido) |
| Notificação por email | Email do Otavio precisa ser o canal — não usar do SUBDEIS | ✅ Forte |
| 5 dias úteis pra responder | Sem problema | ✅ Forte |
| 14 dias pra affidavit | Pode requerer reconhecimento de firma; planejar | ⚠️ Operacional |

---

# Parte 3 — Síntese

## 3.1 Resumo do fit

| Dimensão | Veredito |
|---|---|
| Elegibilidade institucional | ✅ Forte (com Valdemar como co-aplicante / signatário) |
| Área de pesquisa | ⚠️ Aceito ("Computer Science" / "Other fields") mas fora da prioridade declarada |
| Mérito científico | ⚠️ Médio (sistema robusto + credenciais; falta publicação acadêmica) |
| Impacto potencial | ✅ Forte (caminho de escala concreto) |
| Viabilidade técnica | ✅ Forte (produto rodando) |
| Biosecurity | ✅ Forte (sem vetor) |
| Compromissos pós | ⚠️ Operacional (consents, fiscal) |

## 3.2 Probabilidade subjetiva

**Estimativa:** ~25-35% na primeira tentativa.

Justificativa:
- A favor: produto em produção, time com credenciais EPGE/FGV, caminho de escala concreto, biosecurity não é problema, infraestrutura técnica madura, multi-provider já demonstra uso real de Claude.
- Contra: educação não é a prioridade declarada, ausência de publicação acadêmica formal, time não tem PhD ativo nem perfil acadêmico tradicional.

A barra é "scientific merit + potential impact + technical feasibility". Cumprimos os três, mas a Anthropic provavelmente prioriza bio em caso de empate. O ângulo de extensão pra detecção de risco escolar/proteção infantil pode mover o impacto para um campo de saúde pública, o que ajuda.

## 3.3 Posicionamento recomendado

1. **Aplicar como team Otavio + Valdemar**, com FGV/EPGE como organização institucional.
2. **Enquadrar como ciência de dados longitudinais em educação**, não como EdTech / produto. Frase âncora possível (verbatim do Otavio em `voice-anchors.md`): "Eu quero criar algo que é muito mais que um número".
3. **Liderar com o método** (schema longitudinal cross-curso, classificação pura, transparência por etapa) e a evidência (relatório longitudinal real de 9 disciplinas em 4 anos).
4. **Mencionar extensão pra educação básica + detecção de risco + medidas socioeducativas como impacto científico de alto retorno fora da pedagogia.** Mas tratar como **exemplo** da arquitetura genérica, não como o foco — conforme [`shared/voice-anchors.md`](../../shared/voice-anchors.md) F3 e D4 do Otavio.
5. **Honestidade técnica:** declarar que multi-provedor + cross-curso ainda precisam refinamento; esse é o uso para o qual os créditos são instrumentais.
6. **Apresentação (PDF) como anexo:** `NOVO_CR_Apresentacao_v3.pptx_0.pdf` em `prova-ia-v2/` carrega tagline, pipeline, dados em produção. Slide 22 ("Estes Não São Mockups") é uma peça forte.

## 3.4 Pendências pré-submissão

| Item | Quem | Quando |
|---|---|---|
| Carta de apoio de Valdemar atestando afiliação acadêmica | Otavio → Valdemar | Antes da submissão |
| Conversa com Cysne se Valdemar não puder | Otavio | Backup |
| Verificar se SUBDEIS exige ciência formal | Otavio (operacional) | Antes da submissão |
| Acessar o Google Form e levantar os campos | Otavio (com browser) | Antes da submissão |
| Atualizar `shared/metrics-current.md` | Ariadne | Imediatamente pré-submissão |
| Submissão CNPq Jovem Cientista | Otavio + Valdemar | 31 jul 2026 |
| Decidir se submete a Anthropic em 1 jun (próxima janela) ou em 6 jul (após CNPq submetido, mais credencial) | Otavio | Esta sessão |
| Verificar com contador implicações fiscais dos créditos | Otavio (operacional) | Se selecionado |
| Confirmar com Moacyr que dados EMAp dele estão sob consentimento que cobre uso via API Anthropic | Otavio → Moacyr | Antes da submissão |

## 3.5 Open questions (não respondidas pelas fontes)

1. **A Anthropic aceita aplicação onde a organização é a faculdade do co-aplicante (Valdemar), mas o pesquisador principal de execução é alumni (Otavio)?** Linguagem das regras suporta team com pelo menos um membro afiliado — mas convém confirmar.
2. **Renovação após 6 meses:** se o projeto continua escalando, dá pra reaplicar? Regras não dizem.
3. **A licença "irrevocable" sobre dados que passam pela API afeta dados FGV armazenados em outros lugares?** Provavelmente não (só o que trafega pela API), mas vale confirmação legal.
4. **Existe contato humano pra perguntas pré-submissão?** Página não dá email direto. Talvez via Anthropic support.

---

## Próximo passo recomendado

Abrir `draft.md` e começar a escrever a aplicação propriamente dita usando este documento como guia + `shared/project-description.md` como conteúdo canônico. Antes disso, decidir com Otavio:

- Janela: junho ou julho?
- Co-aplicante confirmado: Valdemar ou alternativa?
- Pesquisa preliminar com Valdemar pra alinhar narrativa pré-submissão?
