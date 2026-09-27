# Desenho de Experimento: [nome do experimento/piloto]

> Skill de origem: `design-experiment`. Este documento é preenchido **antes** de ligar o experimento. Todo número carrega etiqueta de proveniência: `medido` · `meta` · `estimativa` · `a confirmar`.

**Data:** [AAAA-MM-DD] · **Autor:** [nome] · **Quem decide em cima do resultado:** [nome/área]

## Decisão que este experimento destrava

[O que muda no plano do time conforme o resultado. Se nenhum resultado possível muda alguma coisa, pare aqui — o experimento não precisa existir.]

## Hipótese

[Uma frase: o que se espera que aconteça e por quê.]

## Métrica primária

*(Uma só. Duas métricas primárias garantem que sempre haverá uma versão positiva do resultado para contar.)*

| Métrica | Fonte de medição | Valor de partida | Etiqueta |
|---|---|---|---|
| [nome] | [ferramenta/evento/query] | [valor] | `medido`/`a confirmar` |

## Métricas secundárias e a métrica que pode piorar

*(Toda mudança tem um efeito colateral plausível. Nomeie e instrumente antes de ligar — métrica que ninguém mediu não é evidência de que nada aconteceu.)*

| Métrica | Por que pode se mover | Fonte de medição | Etiqueta |
|---|---|---|---|
| [secundária] | [razão] | [fonte] | `medido`/`a confirmar` |
| **[a que pode piorar]** | [razão] | [fonte] | `medido`/`a confirmar` |

## Régua de sucesso

*(Definida antes da coleta, acordada com quem decide, e não muda depois que o primeiro número aparece.)*

- **Direção esperada:** [sobe / desce]
- **Corte que separa sucesso de fracasso:** [valor] — `meta`
- **Efeito mínimo que justifica o esforço:** [valor] — `meta`
- **Régua metodológica consagrada usada (se houver):** [ex.: corte de 40% de "muito desapontado(a)", metodologia Sean Ellis]
- **Acordada com:** [nomes] em [AAAA-MM-DD]

## Amostra e elegibilidade

- **Quem entra:** [definição do público]
- **Percentual da base:** [%]
- **Critério de atividade recente:** [ex.: pelo menos um acesso à funcionalidade nos 15 dias anteriores]
- **Grupo de controle:** [como é formado] *ou* [por que não há um, e o que isso limita na leitura]

## Janelas de medição

*(Nunca uma só — janelas separadas são o que distingue efeito real de sazonalidade.)*

| Janela | Período | O que ela isola |
|---|---|---|
| 1 | [de/até] | [ex.: baseline pré-mudança] |
| 2 | [de/até] | [ex.: efeito imediato] |
| 3 | [de/até] | [ex.: efeito sustentado] |

## Fases de rollout

| Fase | Público | Gatilho que autoriza a próxima |
|---|---|---|
| Piloto | [%/segmento] | [condição objetiva] |
| Expansão | [%/segmento] | [condição objetiva] |
| Base total | [—] | [condição objetiva] |

## Plano de leitura

*(O que se faz em cada cenário, decidido antes de ver o número.)*

- **Se bater a régua:** [ação]
- **Se não bater:** [ação]
- **Se o resultado vier misto** (primária melhora, secundária piora): [ação — este é o cenário mais provável e o menos planejado]

## Riscos da medição

- [Sazonalidade, contaminação entre grupos, mudança de metodologia no meio, volume insuficiente — cada um com o que fazer a respeito]

## Se a régua for um OKR

| Key result | Valor de partida | Valor de chegada | Janela | Fonte de medição | Etiqueta |
|---|---|---|---|---|---|
| [métrica nomeada] | [valor] | [valor] | [trimestre] | [fonte já resolvida] | `meta` |

*(Key result sem número, sem fonte definida, ou que mede entrega em vez de resultado, não entra. Entrega é marco de roadmap — ver `roadmap-update`.)*
