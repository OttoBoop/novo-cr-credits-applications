# Novo CR — Descrição canônica do projeto

Peça reusável de uma página em voz do Otavio, derivada de `prova-ia-v2/docs/missao.md`, da apresentação `NOVO_CR_Apresentacao_v3.pptx_0.pdf`, do email v6 produzido pelo Otavio para FGV Ventures, e ancorada nos quotes em [voice-anchors.md](voice-anchors.md).

Antes de adaptar para uma aplicação específica, reler [voice-anchors.md](voice-anchors.md), [team-and-credentials.md](team-and-credentials.md) e [framing-principle.md](framing-principle.md).

---

## O que é

O Novo CR é uma plataforma de educação baseada em dados. O MVP visível é uma ferramenta de correção pedagógica com IA, em produção em ia-educacao-v2.onrender.com. O sistema processa cada prova numa cadeia de seis etapas (extração de questões, gabarito, respostas; correção; análise de habilidades; relatório final) e em todas elas o professor mantém a decisão.

A nota é um subproduto. O que importa são os relatórios — que contam por que o aluno errou, que habilidade demonstrou e como evolui ao longo das atividades. Há também relatórios agregados por turma, por matéria, e o longitudinal cross-curso, que rastreia a trajetória de competências de um aluno ao longo dos anos.

## Estado atual

Em alpha, mas em produção. 26 matérias, mais de 100 atividades processadas. Roda com três provedores em paralelo (OpenAI, Anthropic, Google). O relatório longitudinal cross-curso, eixo central, ainda sai parcialmente via chat sem pipeline batch automatizado; o multi-provedor ainda precisa de refinamento.

A maior parte dos dados que alimentam o sistema vem da graduação completa do fundador na EPGE/FGV (18 disciplinas, 2021–2025), importadas via eClass com provas, gabaritos e avaliações. A partir disso foi gerado um relatório longitudinal real de 9 disciplinas em 4 anos. O professor Moacyr (EMAp) enviou uma disciplina de mestrado (Álgebra Linear Avançada); existe também uma turma de Cálculo 1 EPGE 2021 usada como caso central de demonstração.

## Por que importa

O projeto roda hoje em cursos específicos da FGV, mas a plataforma é genérica: qualquer matéria com avaliação pode entrar nela, dentro ou fora da FGV, da educação superior à básica. É na educação básica que abrem aplicações além da pedagogia — exemplos incluem detecção de risco escolar com dados longitudinais, acompanhamento de medidas socioeducativas, proteção infantil.

A correção automática funciona porque a IA não precisa resolver a questão — apenas comparar a resposta ideal com a do aluno. É um trabalho de classificação. Critérios de correção aumentam precisão. A decisão final é sempre do professor.

O case real saiu de uma cena conhecida na FGV: a prova termina, vem a fila pós-aula, o monitor passa horas explicando aluno por aluno, alguns professores oferecem ponto extra a quem não pede revisão pra recuperar parte do dia. Com o Novo CR, o aluno lê o relatório, e se discorda pleiteia por escrito; o professor decide; e os dados ficam registrados.

## Rede acadêmica

O projeto tem apoio de:

- **Rubens Cysne** (diretor EPGE/FGV) — incentivou o início do projeto em dezembro de 2025.
- **Moacyr** (prof. EMAp/FGV) — colocou os primeiros dados de alunos no sistema e fez a ponte com Mario Andrade.
- **Mario Andrade** (coord. pedagógico CTAE/FGV) — caminho de implantação em escola FGV em 2027.
- **Valdemar Pinho Neto** (coord. graduação EPGE, orientador de TCC do fundador) — signatário acadêmico para programas de pesquisa.

Outros professores acompanham com apoio menor (Layla Mendes, Diogo Robaina — EPGE; Walter Wagner — EMAp).

## Cronograma

- **Maio 2026:** primeira aplicação a programas de crédito (Anthropic AI for Science, OpenAI Researcher Access).
- **Junho 2026:** Rio Web Summit (8–11), networking com aceleradoras e EdTech privada.
- **Julho 2026:** submissão ao Prêmio Jovem Cientista CNPq (linha 3, IA e Educação, prazo 31).
- **2027:** alvo de implantação em pelo menos uma escola FGV via CTAE.

## Quem aplica

Otavio Bopp aplica como cidadão privado e alumni EPGE/FGV. Trabalha hoje na SUBDEIS (Prefeitura do Rio) e tem passagem prévia pelo gabinete do vereador Flávio Valle — credenciais executivas, não afiliação institucional do projeto. Para programas que exigem afiliação acadêmica, Valdemar Pinho Neto é o signatário primário.
