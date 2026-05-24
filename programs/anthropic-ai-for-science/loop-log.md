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

(Próximas entradas serão adicionadas quando o loop continuar — abertura do draft.md depende da decisão sobre janela de submissão.)
