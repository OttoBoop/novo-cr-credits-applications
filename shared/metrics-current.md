# Métricas atuais do Novo CR

Snapshot dos números do sistema em produção. **Atualizar antes de cada aplicação** rodando os comandos de verificação no final.

> Última verificação: 2026-05-23 (durante o setup do repo)

## Produção

- **URL:** https://ia-educacao-v2.onrender.com
- **Estado:** em alpha, rodando em produção
- **Provedores de IA:** OpenAI (GPT-5 family), Anthropic (Claude 4.x family), Google (Gemini 3.x family) — em paralelo

## Conteúdo no sistema

- **26 matérias** cadastradas e em uso
- **Mais de 100 atividades** processadas pelo pipeline completo

## Dados FGV reais usados como base

1. **Graduação completa do fundador na EPGE** — 18 disciplinas, 2021–2025, importadas via eClass (plataforma digital da FGV) com provas, gabaritos e avaliações. Cobre Cálculo II, Computação, Direito e Economia, Econometria I, Economia Brasileira Contemporânea, Finanças, Formação Econômica do Brasil, História Econômica Geral I, Interpretações do Brasil, Introdução ao R, Lab. Ciência de Dados/Finanças, Lab. Políticas Públicas, Macroeconomia III, Microeconomia I, Quantitative Methods in Marketing, Teoria da Probabilidade.
2. **1 disciplina de mestrado EMAp** — Álgebra Linear Avançada, enviada pelo prof. Moacyr.
3. **1 turma externa Cálculo 1 EPGE 2021** — usada como caso central de demonstração.

## Pipeline

- **6 etapas** por prova: extração de questões → extração de gabarito → extração de respostas → correção → análise de habilidades → relatório final.
- **Decisão final é do professor** em todas as etapas.
- **Relatórios:** narrativos por aluno, agregados por turma, agregados por matéria, **longitudinal cross-curso** (eixo central).

## Output longitudinal já gerado

- **Relatório longitudinal real:** 9 disciplinas em 4 anos (graduação do fundador), 7 páginas.
- **Cross-curso:** ainda sai parcialmente via chat, sem pipeline batch automatizado (em refinamento).

## Comandos pra atualizar este arquivo

```bash
# Total de matérias
curl -s https://ia-educacao-v2.onrender.com/api/materias | jq length

# Total de turmas
curl -s https://ia-educacao-v2.onrender.com/api/turmas | jq length

# Matérias por escola (filtra eClass + EPGE + EMAp)
curl -s https://ia-educacao-v2.onrender.com/api/materias | jq '[.[] | select(.descricao | test("eClass|EPGE|EMAp"))] | length'
```

(Total de atividades não tem endpoint público direto — verificar via dashboard ou contagem manual.)
