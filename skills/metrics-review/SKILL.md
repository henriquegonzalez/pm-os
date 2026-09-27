---
name: metrics-review
description: Estrutura a análise de métricas de produto — tendências, desempenho contra meta, anomalias — em um review que separa efeito real de ruído. Use para reviews semanais/mensais/trimestrais ou para investigar uma variação inesperada.
---

# Metrics Review

## Quando usar

Reviews recorrentes de métricas, investigação de uma queda ou alta inesperada, ou quando um número solto precisa virar recomendação.

## O caso que molda esta skill

Medi o efeito de adicionar fricção deliberada — uma etapa de confirmação — num fluxo de upgrade de cartão. Desenhei a medição antes/depois em **três janelas de tempo**, especificamente para separar sazonalidade do efeito real da mudança: uma janela só teria me dado um número, não uma resposta. E acompanhei não só a conversão, mas quanto tempo quem desistia levava para tentar de novo — parte que não estava no desenho original e entrou porque eu suspeitava que fricção pudesse empurrar gente para fora, não só filtrar quem não queria de verdade.

O resultado veio misto: a conversão do fluxo subiu **1,1 ponto percentual**, o retorno no mesmo dia de quem desistiu caiu **18 pontos percentuais**, e o abandono geral do fluxo seguiu em torno de **89%**, praticamente inalterado — todos `medido`. Apresentei os três juntos, sem escolher qual mostrar. Um review que só mostra o que "deu certo" não é análise, é curadoria de boa notícia — e quem decide em cima disso decide errado. Esta skill existe para produzir o outro tipo de review.

## Como eu trabalho

1. **Reunir os dados** — métrica atual, período de comparação, meta, e recorte por segmento quando existir. Se não houver ferramenta de analytics conectada, peço os números manualmente e pergunto por eventos de negócio recentes que possam explicar variação (lançamento, campanha, incidente).
2. **Organizar em hierarquia** — uma métrica norte (a que resume saúde do produto), métricas de saúde de primeiro nível (aquisição, ativação, engajamento, retenção, monetização, satisfação) e métricas diagnósticas de segundo nível por baixo de cada uma.
3. **Analisar tendência, não só ponto** — valor atual, direção da mudança, variação contra meta, se está acelerando ou desacelerando, e se a mudança é sustentada ao longo de mais de uma janela de medição (não só o último dia).
4. **Checar a métrica que não era a esperada.** Toda mudança tem um efeito colateral plausível; se ninguém mediu, o review diz isso em vez de concluir sem ele.
5. **Gerar o review** (estrutura abaixo).

## Regra de proveniência dos números

Todo número no review carrega uma etiqueta: `medido` · `meta` · `estimativa` · `a confirmar`. Se a métrica vem de uma ferramenta conectada, é `medido`. Se vem de meta definida antes do período, é `meta`. Se é projeção, `estimativa`. Se a fonte não está clara ainda, `a confirmar` — e isso não impede o review de sair, só impede que alguém trate aquele número como fato.

## Estrutura do review

> Template pronto para preencher: [`templates/metrics-review-template.md`](../../templates/metrics-review-template.md)

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
- Ler uma única janela de medição e chamar de efeito o que pode ser sazonalidade.
- Tratar estimativa como se fosse medição.
- Comparar períodos com metodologia de medição diferente sem avisar.
- Declarar vitória quando a métrica principal não se moveu e só as secundárias mexeram.
- "Continuar monitorando" como única ação recomendada.

## Follow-up

Depois do review, ofereço: investigação mais profunda de uma métrica específica, especificação de dashboard, proposta de experimento para testar a hipótese de causa levantada, ou a versão do resultado adaptada por audiência (ver `stakeholder-update`) — especialmente quando o resultado foi misto.
