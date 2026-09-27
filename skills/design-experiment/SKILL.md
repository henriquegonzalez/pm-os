---
name: design-experiment
description: Desenha a medição antes de mexer no produto — métrica primária, régua de sucesso, amostra, elegibilidade e janelas de medição definidas com antecedência. Use antes de lançar experimento, piloto ou rollout faseado, e para escrever OKR cuja fonte de medição já esteja resolvida.
---

# Design Experiment

## Quando usar

Antes de rodar um experimento, de ligar um piloto ou de começar um rollout faseado — enquanto ainda dá para escolher o que medir. Também serve para escrever OKR ou meta trimestral, porque um key result sem fonte de medição definida é uma frase de intenção, não uma régua. Depois que os números existirem, o par desta skill é `metrics-review`.

Se você já lançou e agora quer entender o resultado, esta skill chegou tarde: vá direto para `metrics-review` e traga o aprendizado de volta para cá no próximo ciclo.

## O caso que molda esta skill

No piloto de um cofrinho de cashback que rende enquanto espera e libera limite proporcional ao pagamento da fatura, a parte que mais evitou dor de cabeça não foi o desenho do produto — foi ter definido as metas de adoção e retenção **antes do lançamento**, não durante. Isso obrigou o time a concordar sobre o que "funcionar" significava antes de qualquer número aparecer.

Parece burocracia até a primeira vez que não se faz. Sem régua prévia, o número que chega vira campo de disputa de interpretação: quem defendia a aposta acha que foi bom, quem era cético acha que foi ruim, e a discussão vira sobre pessoas em vez de sobre o produto. Com a régua acordada antes, o resultado — qualquer que seja — só precisa ser lido.

O corolário vem do experimento de fricção num fluxo de upgrade: a régua não cobre só a métrica que você espera melhorar. Eu tinha desenhado a medição para pegar também o comportamento de quem desistia, e foi justamente ali que apareceu o efeito colateral (o retorno no mesmo dia caiu 18 p.p.). Se eu só tivesse instrumentado a conversão, teria declarado vitória com 1,1 p.p. e não saberia do resto.

## Como eu trabalho

1. **Nomear a decisão que o experimento vai destravar.** Se nenhum resultado possível muda o que o time vai fazer, o experimento não precisa existir — isso economiza mais tempo do que qualquer otimização de desenho.
2. **Escolher a métrica primária — uma só.** Duas métricas primárias é o mesmo que nenhuma: garante que sempre haverá uma versão positiva do resultado para contar.
3. **Nomear a métrica que pode piorar.** Toda mudança tem um efeito colateral plausível. Escrevo qual é, e instrumento antes de ligar. Métrica que ninguém mediu não é evidência de que nada aconteceu.
4. **Definir a régua antes:** direção esperada, corte que separa sucesso de fracasso, e o tamanho mínimo de efeito que justifica o esforço. A régua é acordada com quem vai decidir em cima dela, não escrita depois por quem analisou.
5. **Definir amostra e elegibilidade.** Quem entra, qual percentual da base, e qual critério de atividade recente — por exemplo, pelo menos um acesso à funcionalidade nos 15 dias anteriores. Critério de elegibilidade frouxo é o jeito mais comum de medir gente que nunca ia reagir de qualquer forma.
6. **Definir as janelas de medição.** Nunca uma só: janelas separadas são o que permite distinguir efeito real de sazonalidade. Defino quantas, de que tamanho, e a partir de quando começam a contar.
7. **Registrar o desenho antes de ligar** (estrutura abaixo) e circular para quem vai receber o resultado. Esse registro é o que impede a régua de se mover depois.

## Regra da régua definida antes

A régua é escrita antes da coleta, por escrito, e não muda depois que o primeiro número aparece. Mudança de régua no meio só é legítima se a metodologia de medição se revelou errada — e nesse caso o experimento recomeça, não se reinterpreta.

Quando existe um corte metodológico consagrado, uso ele em vez de inventar um: numa pesquisa de PMF pela metodologia Sean Ellis, por exemplo, o corte de 40% de "muito desapontado(a)" é a régua, e foi definido muito antes de eu coletar qualquer resposta.

## Quando a régua é um OKR

Um key result bem escrito é exatamente o que esta skill produz: métrica nomeada, valor de partida, valor de chegada, janela de tempo e **fonte de medição já resolvida**. Se a fonte não existe ainda, o primeiro key result do trimestre é construir a medição — não é perda de tempo, é a condição de todos os outros.

O que não aceito num OKR: key result sem número, key result cuja fonte é "a gente vê depois", e key result que mede entrega ("lançar X") em vez de resultado. Entrega é marco de roadmap (ver `roadmap-update`), não key result.

## Regra de proveniência dos números

Régua e meta definidas antes da coleta são `meta`. Resultado apurado é `medido`. Projeção de efeito antes de rodar é `estimativa`. Fonte de medição ainda não instrumentada é `a confirmar` — e um experimento com métrica primária `a confirmar` não deveria ser ligado.

## Estrutura do desenho de experimento

> Template pronto para preencher: [`templates/experiment-design-template.md`](../../templates/experiment-design-template.md)

- **Decisão que este experimento destrava** — o que muda no plano do time conforme o resultado.
- **Hipótese** — o que se espera que aconteça e por quê, em uma frase.
- **Métrica primária** — uma só, com fonte de medição e valor de partida.
- **Métricas secundárias e a métrica que pode piorar** — nomeadas antes, instrumentadas antes.
- **Régua de sucesso** — corte, direção e efeito mínimo relevante, acordados com quem decide.
- **Amostra e elegibilidade** — quem entra, qual percentual, qual critério de atividade recente, grupo de controle (ou por que não há).
- **Janelas de medição** — quantas, de que tamanho, a partir de quando.
- **Fases de rollout** — piloto, expansão e o gatilho que autoriza cada passo.
- **Plano de leitura** — o que se faz em cada cenário de resultado, inclusive no resultado misto.
- **Riscos da medição** — sazonalidade, contaminação entre grupos, mudança de metodologia no meio.

## Erros comuns que evito

- Ligar o experimento e definir o que era sucesso depois de ver o número.
- Duas métricas primárias, o que garante que sempre haverá uma boa notícia para contar.
- Não instrumentar a métrica que pode piorar, e depois tratar a ausência de dado como ausência de efeito.
- Uma única janela de medição, que não separa efeito de sazonalidade.
- Critério de elegibilidade frouxo, que mede quem nunca ia reagir.
- Key result sem fonte de medição definida.
- Desenhar experimento cujo resultado não muda decisão nenhuma.

## Follow-up

Depois do desenho, ofereço: a leitura do resultado quando os dados chegarem (ver `metrics-review`), a seção de métricas de sucesso do PRD já preenchida com esta régua (ver `write-spec`), o plano de sprint das fases de rollout (ver `sprint-planning`), ou estressar a hipótese antes de gastar o ciclo (ver `product-brainstorming`).
