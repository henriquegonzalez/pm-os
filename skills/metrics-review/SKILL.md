---
name: metrics-review
description: Estrutura a análise de métricas de produto — tendências, desempenho contra meta, anomalias — em um review que separa efeito real de ruído. Use para reviews semanais/mensais/trimestrais ou para investigar uma variação inesperada.
---

# Metrics Review

## Quando usar

Reviews recorrentes de métricas, investigação de uma queda ou alta inesperada, ou quando um número solto precisa virar recomendação.

## O princípio que guia esta skill

Já medi o efeito de uma mudança em um fluxo de upgrade em três janelas de tempo diferentes, antes e depois. O resultado não foi limpo: a taxa de conclusão subiu, o retorno no mesmo dia caiu, mas o abandono geral no fluxo continuou praticamente igual. Apresentei os três números juntos, sem esconder o que não tinha melhorado. Um review de métricas que só mostra o que "deu certo" não é análise, é curadoria de boa notícia — e quem toma decisão em cima disso decide errado. Esta skill existe para produzir o outro tipo de review.

## Regra de proveniência

Todo número no review carrega uma etiqueta: `medido` · `meta` · `estimativa` · `a confirmar`. Se a métrica vem de uma ferramenta conectada, é `medido`. Se vem de meta definida antes do período, é `meta`. Se é projeção, `estimativa`. Se a fonte não está clara ainda, `a confirmar` — e isso não impede o review de sair, só impede que alguém trate aquele número como fato.

## Como eu trabalho

1. **Reunir os dados** — métrica atual, período de comparação, meta, e recorte por segmento quando existir. Se não houver ferramenta de analytics conectada, peço os números manualmente e pergunto por eventos de negócio recentes que possam explicar variação (lançamento, campanha, incidente).
2. **Organizar em hierarquia** — uma métrica norte (a que resume saúde do produto), métricas de saúde de primeiro nível (aquisição, ativação, engajamento, retenção, monetização, satisfação) e métricas diagnósticas de segundo nível por baixo de cada uma.
3. **Analisar tendência, não só ponto** — valor atual, direção da mudança, variação contra meta, se está acelerando ou desacelerando, e se a mudança é sustentada ao longo de mais de uma janela de medição (não só o último dia).
4. **Gerar o review** (estrutura abaixo).

## Estrutura do review

- **Resumo** — 2-3 frases: saúde geral, mudança mais notável, o alerta principal (se houver).
- **Placar de métricas** — tabela com valor atual, período anterior, variação percentual, meta e status.
- **Análise de tendência** — o que aconteceu, hipótese mais provável de causa, e se a tendência é sustentada ou pontual.
- **Pontos positivos** — métricas acima da meta.
- **Pontos de atenção** — métricas abaixo da meta ou sinal de alerta precoce, apresentados com o mesmo peso dos pontos positivos, nunca minimizados.
- **Resultado misto (quando existir)** — quando uma mudança melhora uma métrica e piora ou não afeta outra, isso vira uma seção própria, não uma nota de rodapé.
- **Ações recomendadas** — investigação específica, experimento, ou alerta de monitoramento — nunca "continuar observando" sem um próximo passo concreto.
- **Contexto e ressalvas** — qualidade do dado, mudança de metodologia de medição, qualquer coisa que afete comparabilidade entre períodos.

## Erros comuns que evito

- Mostrar só a métrica que melhorou quando o experimento teve efeito misto.
- Tratar estimativa como se fosse medição.
- Comparar períodos com metodologia de medição diferente sem avisar.
- "Continuar monitorando" como única ação recomendada.

## Follow-up

Depois do review, ofereço: investigação mais profunda de uma métrica específica, especificação de dashboard, ou proposta de experimento para testar a hipótese de causa levantada.
