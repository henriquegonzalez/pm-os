---
name: roadmap-update
description: Cria, atualiza ou repriorizar um roadmap de produto — inclusive quando não existe histórico de dados para embasar a decisão. Use para adicionar itens, mudar prioridade, ajustar prazos ou montar o roadmap do zero.
---

# Roadmap Update

## Quando usar

Toda vez que o roadmap precisa refletir uma informação estratégica nova: uma meta trimestral mudou, um item atrasou, uma dependência apareceu, ou simplesmente não existe roadmap ainda e alguém precisa de um ponto de partida defensável.

## O caso que molda esta skill

Uma vez precisei decidir prioridade de roadmap sem ter histórico de dados — produto novo, sem base de uso para embasar projeção. A saída não foi fingir que o dado existia. Foi construir uma calculadora com 14 variáveis (tamanho de público alcançável, taxa de conversão esperada por segmento, capacidade de engenharia, dependências externas, entre outras) e rodar uma simulação de adoção — **rotulada como simulação, não como previsão**. Essa etiqueta importa: ela muda a conversa de "por que erramos a meta" para "o que a simulação assumia e o que já sabemos hoje que era diferente". Todo roadmap que ajudo a montar sem dado histórico segue esse princípio.

## Como eu trabalho

1. **Entender o estado atual.** Levanto os itens existentes (status, dono, data) e a última justificativa de prioridade registrada — se não existir, é a primeira lacuna a resolver, não uma suposição a preencher.
2. **Identificar a operação.** Adicionar item, atualizar status, repriorizar, mover prazo, ou construir do zero — cada uma exige uma pergunta diferente antes de tocar no roadmap.
3. **Se faltar dado histórico, ser explícito sobre isso.** Construo (ou peço) as variáveis que sustentam a decisão — público alcançável, capacidade, dependência — e deixo claro que a saída é uma simulação, com as premissas visíveis ao lado do número.
4. **Gerar o roadmap atualizado** (formato abaixo).
5. **Resumir o que mudou e por quê.** Toda mudança de prioridade tem uma frase de justificativa ligada a uma informação nova — nunca "porque sim" ou "porque pediram".

## Formatos de visualização

- **Agora / Próximo / Depois** — o mais usado no dia a dia, porque comunica intenção sem prometer data em coisa que ainda pode mudar.
- **Temas trimestrais** — quando o roadmap precisa amarrar em OKR ou meta de negócio.
- **Timeline com dependência visível** — só quando o compromisso de data é real (lançamento com parceiro externo, por exemplo); fora disso, data fixa em roadmap é promessa que vira dívida de confiança.

## Priorização

Uso RICE ou Valor vs. Esforço como ponto de partida, mas a pergunta que realmente decide é: essa aposta depende de alguém fora do meu controle direto (outra squad, parceiro comercial, fornecedor)? Se sim, isso entra como risco explícito no roadmap, com dono, não como uma linha igual às outras.

Capacidade: guio por uma proporção prática — a maior parte do time em features de roadmap, uma fração reservada para saúde técnica, e uma margem de buffer para o que sempre aparece no meio do trimestre. Explicito essa divisão em vez de deixar implícita, porque é o primeiro lugar que a liderança pergunta quando o roadmap "não anda".

## Erros comuns que evito

- Roadmap com data fixa em item que depende de terceiro sem essa dependência estar visível.
- Reprioridade sem frase de justificativa ligada a informação nova.
- Simulação apresentada como se fosse previsão histórica.
- Buffer de capacidade zerado "para caber tudo" — isso não elimina o imprevisto, só empurra ele pra virar atraso não comunicado.

## Follow-up

Depois do roadmap atualizado, ofereço: versão formatada para audiência específica (ver `stakeholder-update`) ou rascunho de comunicação sobre o que mudou e por quê.
