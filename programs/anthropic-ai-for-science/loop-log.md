# Anthropic AI for Science — Loop log

Log das ações da assistente (Ariadne/Claude Code) e dos prompts do Otavio durante o loop de preparação da aplicação. Formato cronológico; cada entrada tem timestamp aproximado, prompt/ação, e o que foi feito.

---

## Sessão 1 — abertura do loop (2026-05-24)

### P1 — Otavio (prompt inicial)

> "Li e gostei dos .mds. Vamos ocmeçar os loops? Para um dos programas, escreva dois .mds,
>
> 1. detalhando as exigencias e, posteriormente, comparando-as com o que nosso projeto tem. Faça isso primeiro lendo o site com os dados do programa alvo. Depois, faça a leitura dos documentos chave e sources adicionais. Por fim, você vai terminar de escrever este .md
> 2. Log das ações e dos meus prompts"

### Interpretação do P1

- Programa-alvo escolhido por mim: **Anthropic AI for Science** (justificativa: maior valor — $20K — e ciclo mensal, sem precisar de incorporação ou VC).
- Dois arquivos a produzir:
  1. `requirements-and-fit.md` — exigências detalhadas + comparação com o que o Novo CR tem
  2. `loop-log.md` — este arquivo
- Processo solicitado pra produzir o primeiro:
  1. Ler o site oficial do programa
  2. Ler documentos-chave do projeto + sources adicionais
  3. Terminar de escrever o `.md`

### Plano de ações para esta sessão

1. (✅ feito) Criar este loop-log com P1 registrado verbatim
2. WebFetch profundo da página oficial: https://support.claude.com/en/articles/11199177-anthropic-s-ai-for-science-program
3. WebSearch por projetos aceitos + exemplos do programa (se houver dados públicos)
4. WebSearch por Anthropic Usage Policy específica pra programas de subsídio
5. Reler shared/* (já tenho em contexto, só confirmar) + missao.md + audit_quotes (já lidos nesta conversa)
6. Escrever `requirements-and-fit.md` com:
   - Seção 1: exigências detalhadas em verbatim (do site)
   - Seção 2: comparação ponto-a-ponto com o que o Novo CR tem (usando shared/* como fonte)
   - Seção 3: conclusão (fit/probabilidade + posicionamento recomendado + pendências)
7. Atualizar este log com cada ação
8. Commit + push consolidado

### Princípios deste loop (lições do loop anterior do email)

- **Não inventar fatos.** Cada claim precisa de fonte rastreável (URL, doc, quote verbatim).
- **Não parafrasear voz do Otavio.** Usar `shared/voice-anchors.md` literalmente.
- **Não inverter arquitetura.** Filosofia geral (relatórios) é o foco; aplicações em educação básica/proteção infantil/socioeducação são exemplos, não foco.
- **Cidadão privado + alumni.** SUBDEIS e Valle são credenciais, não afiliação. Valdemar é o signatário.
- **Logar cada passo aqui.** Antes de avançar, anotar o que foi feito.

---

### A1 — WebFetch profundo da página de suporte (2026-05-24)

URL: https://support.claude.com/en/articles/11199177-anthropic-s-ai-for-science-program

Prompt do fetch pediu extração verbatim de 16 dimensões (elegibilidade, áreas, valor, duração, inclusões, exclusões, critérios de avaliação, afiliação institucional, time, ciclo, política de uso, exemplos de projetos aceitos, exclusões geográficas, renovação, contato).

Achados novos vs primeiro fetch (feito durante o setup inicial do repo):
- "Limited to academia and nonprofit organizations" — explícito.
- Time-level credentials, não individual.
- Renovação NÃO está documentada.
- Examples NÃO estão documentados.
- Notificação sem feedback pra rejeitados ("we regret that we cannot provide individual responses to unapproved submissions").
- Link do Google Form obtido: https://docs.google.com/forms/d/e/1FAIpQLSfwDGfVg2lHJ0cc0oF_ilEnjvr_r4_paYi7VLlr5cLNXASdvA/viewform.

### A2 — WebFetch das regras oficiais (2026-05-24)

URL: https://www.anthropic.com/ai-for-science-program-rules
Última atualização da página: 18 fev 2026.

Achados críticos novos:
- **Países excluídos** explícitos (Belarus, China, Cuba, Iran, Myanmar, North Korea, Russia, Sudan, Syria, Crimea, "Donetsk People's Republic", "Luhansk People's Republic"). Brasil OK.
- **Idade mínima**: 18 anos.
- **Cláusula de consents**: aplicante afiliado a empregador/instituição precisa ter obtido todos os consentimentos.
- **Licença perpétua + irrevogável** sobre dados que passam pela API durante uso dos créditos — Anthropic pode treinar modelos com isso.
- **Liberação perpétua de nome/imagem** para promoção.
- **5 dias úteis** pra responder à notificação; **14 dias corridos** pra assinar affidavit.
- **Tax status**: créditos podem ter implicação fiscal; responsabilidade do aplicante.
- **Renovação**: não especificada.

### A3 — WebSearch por exemplos de projetos aceitos (2026-05-24)

Query: "Anthropic AI for Science program accepted projects examples education research 2026".

Achados:
- Não há projetos aceitos publicados publicamente.
- Anthropic tem **parceria separada com Teach For All** (educação) — sinal de que educação é tópico de interesse, mas via outra trilha.
- Anthropic publicou Education Report "AI Fluency Index" — outra trilha separada de pesquisa educacional dentro da empresa.
- Programa Fellows é trilha separada (segurança de IA, não AI for Science).

### A4 — WebFetch do anúncio público (2026-05-24)

URL: https://www.anthropic.com/news/ai-for-science-program
Lançamento do programa: 5 mai 2025.

Achados:
- Anúncio é **biology-heavy**: só menciona bio/life sciences, drug discovery, agricultural productivity.
- **Não menciona** Computer Science nem "Other fields" — apesar de estarem na lista operacional do support article.
- Sinaliza que a categoria "Other fields" é catch-all com prioridade menor.
- Sem case studies de projetos aceitos.

### A5 — Síntese das fontes (2026-05-24)

Conclusões para o fit:
- Fit institucional: forte com co-aplicação (Otavio + Valdemar, FGV como organização).
- Fit de área: aceito mas fora da prioridade declarada (educação compete em "Other fields").
- Fit técnico: forte (sistema em produção, multi-provedor já implementado).
- Fit de impacto: forte (caminho de escala concreto via FGV + SUBDEIS + Paes).
- Biosecurity: sem vetor (educação não é vetor de biorisco direto).
- Compromissos pós-seleção: gerenciáveis, com algumas pendências operacionais (consents Moacyr, fiscal).

### A6 — Escrita do `requirements-and-fit.md` (2026-05-24)

Estrutura final do documento:
1. Fontes consultadas (5 fontes web + 4 docs do projeto).
2. Parte 1 — Exigências detalhadas verbatim (1.1 a 1.7).
3. Parte 2 — Fit pareado (2.1 a 2.8), uma seção por dimensão da exigência.
4. Parte 3 — Síntese: resumo do fit, probabilidade subjetiva (~25-35%), posicionamento recomendado, pendências pré-submissão, open questions.

Princípios mantidos durante a escrita:
- Cada claim com fonte rastreável (URL ou doc do projeto).
- Nenhum dado inventado — quando uma fonte não respondeu, marquei como "open question" ou "pendência".
- Voz do Otavio acessada via `shared/voice-anchors.md` (referenciei F3, D4, M3).
- Arquitetura preservada: educação superior é o presente; básica/proteção/socio são extensões = exemplos, não foco.

### A7 — Pendência: campos do Google Form (não acessível via WebFetch)

O formulário de aplicação é Google Form; não conseguimos acessar via WebFetch porque exige autenticação ou interação de browser. Listado como pendência: Otavio precisa abrir o link e levantar os campos antes de redigir o `draft.md`.

Link: https://docs.google.com/forms/d/e/1FAIpQLSfwDGfVg2lHJ0cc0oF_ilEnjvr_r4_paYi7VLlr5cLNXASdvA/viewform

### A8 — Próximas decisões pendentes (registradas em requirements-and-fit.md §3.4)

Esperando posição do Otavio sobre:
1. Janela de submissão: 1 jun (próxima) vs 6 jul (pós submissão CNPq, com mais credencial).
2. Co-aplicante: confirmar Valdemar; backup Cysne se Valdemar não disponível.
3. Conversa pré-submissão com Valdemar pra alinhar narrativa.
4. Quem levanta os campos do Google Form.

### A9 — Commit + push (2026-05-24)

Arquivos modificados/criados:
- `programs/anthropic-ai-for-science/requirements-and-fit.md` (NOVO)
- `programs/anthropic-ai-for-science/loop-log.md` (POPULADO; estava vazio)

---

## Sessão 2 — primeira leva de drafts em loop (2026-05-24)

### P2 — Otavio (autorização do loop autônomo)

> "Cara, então, eu to ocupado demais para fazer as revisões hoje. Uhm, inclusive, se você colocar um subagente para ver estimativas de custo com api, vai ver que estamos trabalhando para ter isto fechadinho. Queria que você fosse fazend oos drafts em loop mesmo, e quando eu tiver tempo eu verifico tudo!"

### A10 — Subagente: estimativas de custo no codebase (2026-05-24)

Subagente Explore disparado em `/home/otavio/Documents/vscode/prova-ia-v2/` pra mapear estimativas de custo de API. Tarefa: vasculhar `docs/`, `backend/`, `model_catalog.py`, `cost_tracking.py`, e qualquer arquivo com "custo/cost/price/token".

Achados principais:

**Custo medido por pipeline completo (1 prova, 1 aluno):**
- Claude Haiku 4.5: ~$0.28 (~118k input / ~33k output tokens)
- Claude Sonnet 4.5: ~$0.55 (~68k input / ~23k output tokens)
- Gemini 3 Flash: ~$0.19
- Google Flash (Beatriz full pipeline): ~$0.11

**Baseline de 28 runs medidos (2026-05-19):**
- Total: $1.48
- Anthropic: $0.99
- Google: $0.49

**Faixa por configuração (outreach.md §D.7):**
- Ultra-econômico (GPT-5 Nano): ~$0.04
- Econômico (Gemini mix): ~$0.12
- Equilibrado (Haiku + Sonnet + Haiku): ~$0.55
- Premium (GPT-5): ~$1.05

**Otimização planejada:** prompt caching reduz ~89% dos tokens de entrada na etapa CORRIGIR (mesmo gabarito reusado entre alunos de uma turma).

**Infra de medição:** `cost_tracking.py`, `token_usage.py`, endpoints `/api/custos/resumo` e `/api/custos/status`. Custo mensal agregado em produção: não exposto publicamente.

### A11 — Draft v1 escrito (2026-05-24)

Estrutura:
1. Project title
2. Project summary (3 parágrafos)
3. Team and institutional affiliation
4. Use of Claude API — methodology and technical feasibility
5. Expected impact
6. Biosecurity and safety considerations
7. Estimated credit usage (tabela + alocação)
8. Additional context

Língua: inglês (form é em inglês).
Comprimento aproximado: ~1300 palavras.

### A12 — Auto-crítica de v1 (2026-05-24)

Itens identificados:
1. **Fato inventado:** "~500 students × 6 disciplines × ~4 exams/year = ~12,000 exams/year" — chutei tamanho de escola FGV. Cortar.
2. **Inconsistência:** misturei "I" e "we". Padronizar pra "I" como pesquisador principal, "the team" pra coletivo.
3. **Sentence length:** alguns parágrafos longos demais.
4. **Sub-exploração do diferencial:** sistema em produção é o ponto mais forte e estava enterrado. Trazer pra frente.
5. **Atribuição vaga:** "preliminary analysis projects ~89%" — atribuir ao codebase analysis existente.

### A13 — Draft v2 escrito (2026-05-24)

Mudanças aplicadas:
- Abertura virou: "Most AI-in-education projects are still at the proposal stage. NOVO CR runs in production..." — diferencial forte primeiro.
- Cortei o cálculo "500 × 6 × 4 = 12k" — substituí por "Scaling the system to a full FGV pilot school in 2027" sem números chutados.
- "The codebase's existing cost analysis projects ~89% reduction" — atribuição clara.
- Padronizei "I" / "the team" / "the project".
- Apertei vários parágrafos.

### A14 — Auto-crítica de v2 (2026-05-24)

Pontos restantes:
1. "Scientifically high-return extensions beyond pedagogy" — marketing-speak. Cortar "Scientifically high-return".
2. "These are illustrative applications of the underlying architecture in basic education — they sit downstream of the methodology and motivate it, but the methodology is general." — meta-commentary redundante.
3. "Beneath that surface is the methodological contribution: a longitudinal schema (...) where the methodology supports early detection..." — "where the methodology supports" deselegante; "opening downstream applications such as" flui melhor.
4. "Concretely, the credits would support:" — "Concretely" é filler.

### A15 — Draft v3 escrito (2026-05-24)

Mudanças aplicadas:
- "Scientifically high-return extensions" → "Extensions beyond pedagogy"
- "where the methodology supports" → "opening downstream applications such as"
- Removido "Concretely,"
- Cortei a frase meta-final de Expected impact, reescrita como: "These are downstream applications in basic education; the methodology is general."

### A16 — Decisão: parar em v3 (2026-05-24)

Critério: três iterações com ganhos visíveis em cada uma; v3 está estável; iterações adicionais entrariam em micro-polimento sem ganho real. Lição do loop anterior do email: parar antes de over-fitting é melhor que iterar até cansar.

v3 está pronta para revisão do Otavio quando ele tiver tempo. Próximas ações ficam pendentes da revisão dele.

### A17 — Commit + push de drafts v1/v2/v3 (2026-05-24)

Apenas a v3 final fica em `draft.md`; v1 e v2 estão preservadas em git history (commits separados ou um commit consolidado, decidido na hora do commit).

---

## Pendências para a próxima sessão

1. **Otavio:** abrir o Google Form (https://docs.google.com/forms/d/e/1FAIpQLSfwDGfVg2lHJ0cc0oF_ilEnjvr_r4_paYi7VLlr5cLNXASdvA/viewform) e copiar os campos pra mim. Sem isso, o draft v3 é genérico pra estrutura típica — pode precisar de re-organização quando os campos reais aparecerem.
2. **Otavio:** revisar o draft v3 quando tiver tempo. Os itens críticos a verificar:
   - "BSc Economics, 2025" — confirmar formação correta
   - "started in late 2025" — bate com a história
   - Nomes e cargos da rede FGV — Cysne, Moacyr Alvim, Mario Andrade
   - "Encouraged the project's formal start in December 2025" — bate com o que Cysne fez
3. **Otavio:** decisão sobre janela (1 jun vs 6 jul vs 3 ago).
4. **Otavio:** conversa com Valdemar pra confirmar co-aplicação + carta de apoio.
5. **Ariadne (quando autorizada):** redigir draft de carta de apoio de Valdemar.
6. **Ariadne (quando autorizada):** atualizar `shared/metrics-current.md` com números live pré-submissão.

---

(v3 estável; loop pausado. Próximas entradas ao retomar.)

---

## Sessão 3 — reescrita pra campos reais do form (v3 → v4) — 2026-05-24

### P4 — Otavio compartilhou os campos verbatim do form

Mudanças que isso traz vs v3:
1. **Word limits estritos por campo** (Research Team <300, Research Proposal <500, Claude usage 300, Claude acceleration 200, impact 200, applications 200, success metrics 200) — v3 era um texto fluido, v4 precisa mapear ponto-a-ponto.
2. **Credit ceiling subiu pra até $50K** (eu tinha $20K). 30-min video call se aprovado.
3. **Novos campos:** Organization ID (Anthropic console), Position/title at organization, Where did you hear, Biosecurity checkbox + explanation, Practical applications (separado de Scientific impact).
4. **Brazilian researcher cost angle** — Otavio explicitamente pediu pra reforçar.
5. **"Ongoing since December 2025"** — framing temporal importante.

### A11 — Auto-crítica de v3 (pré-restructure)

v3 não mapeava aos word limits. Texto contínuo precisava virar blocos:
- §Project summary (v3) → vira §Research Proposal v4 mas tem 360 palavras, dentro do limite 500
- §Team and institutional affiliation (v3) → vira §Research Team v4 + §Key team members v4 separados
- §Use of Claude API (v3) → vira §How specifically + §How will Claude accelerate v4
- §Expected impact (v3) → vira §Scientific impact + §Practical applications + §Success metrics v4 (separados)
- §Estimated credit usage (v3) → vira §Resource Requirements v4 com ceiling até $50K, não $20K

### A12 — Escrever v4 (restructure completa)

Mudanças aplicadas:
- Adicionada §Contact information como tabela mapeada aos campos do form
- Adicionados Scientific field(s) checkboxes (CS + Other: Education)
- §Research Team escrito do zero com word count target ~280 (sob 300)
- §Key team members em formato bullet (name, role, brief)
- §Research Proposal recortado pra cobrir scientific question + methodology + outcomes + timeline em ~360 palavras (sob 500)
- §How specifically usa Claude com cost data verbatim do subagent (2026-05-24 audit, Doc 14)
- §How will Claude accelerate em ~98 palavras (sob 200) — foco em (1) structured extraction e (2) long-context cross-course report
- §Scientific impact em ~75 palavras (sob 200)
- §Practical applications em ~85 palavras (sob 200) — extensões downstream, NÃO core focus
- §Success metrics em ~85 palavras (sob 200) com 6 critérios mensuráveis
- §Resource Requirements com ceiling até $50K + alocação concreta
- §Biosecurity: ☑ None of the above + LGPD note pra extensões futuras
- §Additional information com ongoing since Dec 2025, parallel applications declaradas, CNPq companion

### A13 — Auto-crítica de v4

Itens que vou trazer pro REVIEW.md em vez de iterar:
1. "(institutional FGV email — to fill at submission)" — campo crítico que Otavio precisa preencher
2. Organization ID Anthropic — precisa criar/identificar pré-submissão
3. Position/title at organization é ambíguo: Otavio é alumni; Valdemar é Faculty. Resolver no REVIEW (provavelmente Valdemar como ponto institucional)
4. Frase "Brazilian researchers operate at structural cost disadvantage" — repetida em §Research Team e §Resource Requirements e §Research Proposal. Possivelmente redundante. Mas é deliberada (Otavio pediu reforçar). Manter.

### A14 — Decisão: parar em v4

Mapeamento aos campos reais é mais valioso que mais iterações cosméticas. Próxima ação real: Otavio preenche os campos que dependem dele (org ID, emails, profile links) e revisa o conteúdo dentro de cada bloco.

### A15 — Commit

Files: `draft.md` (v4 restructurada), `loop-log.md` (este).
Pendências novas no REVIEW.md: Organization ID, position/title, video call prep, credit ceiling corrigido.

---

(v4 mapeada aos campos reais. Loop pausado pendente do Otavio.)
