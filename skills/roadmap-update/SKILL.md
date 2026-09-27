---
name: roadmap-update
description: Cria, atualiza ou reprioriza um roadmap de produto — inclusive quando não existe histórico de dados para embasar a decisão. Use para adicionar itens, mudar prioridade, ajustar prazos ou montar o roadmap do zero.
---

# Roadmap Update

## Quando usar

Toda vez que o roadmap precisa refletir uma informação estratégica nova: uma meta trimestral mudou, um item atrasou, uma dependência apareceu, ou simplesmente não existe roadmap ainda e alguém precisa de um ponto de partida defensável.

## O caso que molda esta skill

Precisei priorizar apostas de roadmap para produtos novos sem histórico de dado nenhum — o tipo de situação em que "o que a gente acha" vira a régua padrão. A saída não foi fingir que o dado existia. Foi construir uma calculadora com 14 variáveis, da capacidade de engenharia às premissas de comportamento, para dimensionar cada aposta com a mesma régua, e simular adoção com um ecossistema de 10 copilotos de IA especializados — cada um cobrindo uma perspectiva diferente (financeira, de risco, de experiência).

Duas decisões sustentam o método. A primeira: dimensionar pela **audiência efetivamente alcançável**, não pelo público total endereçável — esse corte encolheu apostas que pareciam grandes no papel e disputavam recurso que não mereciam. A segunda: manter a etiqueta **`estimativa` / simulação** visível em todo lugar onde o número aparecesse — planilha, apresentação, conversa. Um número que sai de um processo elaborado parece mais sólido do que é, e a etiqueta é o que muda a conversa de "por que erramos a meta" para "o que a simulação assumia e o que já sabemos hoje que era diferente".

## Como eu trabalho

1. **Entender o estado atual.** Levanto os itens existentes (status, dono, data) e a última justificativa de prioridade registrada — se não existir, é a primeira lacuna a resolver, não uma suposição a preencher.
2. **Identificar a operação.** Adicionar item, atualizar status, repriorizar, mover prazo, ou construir do zero — cada uma exige uma pergunta diferente antes de tocar no roadmap.
3. **Se faltar dado histórico, ser explícito sobre isso.** Construo (ou peço) as variáveis que sustentam a decisão — audiência alcançável, capacidade, dependência — e deixo claro que a saída é uma simulação, com as premissas visíveis ao lado do número.
4. **Gerar o roadmap atualizado** (formato abaixo).
5. **Resumir o que mudou e por quê.** Toda mudança de prioridade tem uma frase de justificativa ligada a uma informação nova — nunca "porque sim" ou "porque pediram".

## Regra de proveniência dos números

Todo número no roadmap carrega uma etiqueta: `medido` · `meta` · `estimativa` · `a confirmar`. Saída de simulação é `estimativa`, sempre, mesmo quando vem de um processo sofisticado. Meta trimestral é `meta`, não previsão. Se a origem não está clara, `a confirmar` — isso não impede o roadmap de circular, só impede que alguém trate aquele número como fato.

## Formatos de visualização

- **Agora / Próximo / Depois** — o mais usado no dia a dia, porque comunica intenção sem prometer data em coisa que ainda pode mudar.
- **Temas trimestrais** — quando o roadmap precisa amarrar em OKR ou meta de negócio.
- **Timeline com dependência visível** — só quando o compromisso de data é real (lançamento com parceiro externo, por exemplo); fora disso, data fixa em roadmap é promessa que vira dívida de confiança.

## Priorização

Uso RICE ou Valor vs. Esforço como ponto de partida, mas a pergunta que realmente decide é: essa aposta depende de alguém fora do meu controle direto (outra squad, parceiro comercial, fornecedor)? Se sim, isso entra como risco explícito no roadmap, com dono, não como uma linha igual às outras.

A segunda pergunta é de dimensionamento: o tamanho que estou usando para comparar apostas é o público que dá para alcançar de fato, ou o endereçável total? Comparar apostas por TAM é como comparar maçã com laranja entre times que defendem prioridades diferentes.

Capacidade: guio por uma proporção prática — a maior parte do time em features de roadmap, uma fração reservada para saúde técnica, e uma margem de buffer para o que sempre aparece no meio do trimestre. Explicito essa divisão em vez de deixar implícita, porque é o primeiro lugar que a liderança pergunta quando o roadmap "não anda".

## Estrutura do roadmap

> Template pronto para preencher: [`templates/roadmap-template.md`](../../templates/roadmap-template.md)

- **O que mudou e por quê** — cada mudança de prioridade com a informação nova que a motivou.
- **Divisão de capacidade** — features, saúde técnica e buffer, explícitos.
- **Visão escolhida** — Agora/Próximo/Depois, temas trimestrais, ou timeline com dependência.
- **Riscos e dependências externas** — com dono nomeado.
- **Simulação (quando não houver dado histórico)** — variáveis, premissas e o número, todos marcados como `estimativa`.

## Erros comuns que evito

- Roadmap com data fixa em item que depende de terceiro sem essa dependência estar visível.
- Reprioridade sem frase de justificativa ligada a informação nova.
- Simulação apresentada como se fosse previsão histórica.
- Dimensionar aposta pelo público endereçável total em vez do efetivamente alcançável.
- Buffer de capacidade zerado "para caber tudo" — isso não elimina o imprevisto, só empurra ele pra virar atraso não comunicado.

## Follow-up

Depois do roadmap atualizado, ofereço: versão formatada para audiência específica (ver `stakeholder-update`), rascunho de comunicação sobre o que mudou e por quê, ou quebra do item de topo em plano de sprint (ver `sprint-planning`).
