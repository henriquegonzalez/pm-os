---
name: sprint-planning
description: Ajuda a escopar trabalho, estimar capacidade real do time e montar um plano de sprint com meta única e riscos explícitos. Use no planejamento de uma nova sprint ou em refinamento de backlog.
---

# Sprint Planning

## Quando usar

Início de sprint, refinamento de backlog, ou quando um time precisa decidir o que cabe de fato no ciclo — não o que caberia numa semana ideal que não existe.

## O caso que molda esta skill

Planejei o ciclo de um cofrinho de cashback que rende enquanto espera e libera limite proporcional ao pagamento da fatura. A parte difícil não foi o cofrinho — foi o conjunto de **travas do fluxo financeiro**: liberação, reversão e elegibilidade, cada uma com um caso de borda do tipo "o que acontece se falhar no meio". Esse tipo de item estima curto na primeira passada, sempre, porque o caminho feliz é óbvio e o caminho de falha só aparece quando alguém pergunta.

Duas coisas entraram no plano por causa disso. Primeiro: **rollout faseado**, começando por piloto controlado antes de expandir a base — o que muda o que é compromisso da sprint e o que é stretch. Segundo: a **régua de sucesso definida antes do piloto**, não durante, o que obrigou o time a concordar sobre o que "funcionar" significava antes de qualquer número aparecer, e evitou briga de interpretação depois.

## Como eu trabalho

1. **Levantar informação real do time** — composição, duração da sprint, itens priorizados de backlog, trabalho que ficou da sprint anterior (carryover), e dependências conhecidas. Carryover não é detalhe — é o primeiro sinal de que a estimativa passada estava otimista.
2. **Estimar capacidade de verdade** — disponibilidade de cada pessoa considerando férias, reuniões recorrentes e qualquer alocação parcial em outro time. Capacidade nominal (todo mundo, tempo todo) não existe na prática.
3. **Escopar e priorizar** — categorizo item de backlog em P0 (compromisso da sprint), P1 (entra se sobrar capacidade) e P2 (próxima sprint). Deixo explícito quais itens são "stretch" para negociar escopo se o ciclo apertar, em vez de negociar isso de surpresa no meio da sprint.
4. **Interrogar o caminho de falha de cada item crítico.** Para item que toca dinheiro, estado ou integração externa, a pergunta obrigatória antes de estimar é: o que acontece se isso falhar no meio? A resposta quase sempre acrescenta trabalho que a estimativa inicial não tinha.
5. **Identificar risco** — dependência de outro time, decisão pendente, ou trabalho técnico não estimado ainda. Cada risco tem uma mitigação, não só um registro de "isso pode dar problema".
6. **Gerar o plano** (estrutura abaixo).

## Regra de capacidade

Planejo para 70-80% da capacidade nominal do time, nunca 100%. A margem não é desperdício — é o espaço para a interrupção que sempre aparece (bug crítico, pedido urgente, ausência não planejada). Time que planeja pra 100% da capacidade não entrega mais rápido; só acumula carryover e perde a meta da sprint com mais frequência.

Em produto que toca fluxo financeiro (pagamento, saldo, limite, cashback), reservo atenção extra na estimativa para item que envolve trava, liberação ou reversão de transação — esse tipo de trabalho quase sempre estima curto na primeira passada, porque o caso de borda raramente aparece na estimativa inicial.

## Regra de proveniência dos números

Estimativa de esforço é `estimativa`, mesmo quando o time tem confiança alta; capacidade apurada a partir de calendário e férias é `medido`; meta da sprint é `meta`. A etiqueta importa no cálculo de carga: comparar trabalho `estimativa` contra capacidade `medido` é exatamente o lugar onde o otimismo entra sem ser percebido.

## Estrutura do plano de sprint

> Template pronto para preencher: [`templates/sprint-plan-template.md`](../../templates/sprint-plan-template.md)

- **Metadados** — datas, tamanho do time, uma meta de sprint em uma frase só.
- **Tabela de capacidade** — tempo disponível e alocação de cada pessoa.
- **Backlog da sprint** — organizado por prioridade, com estimativa e responsável.
- **Cálculo de carga** — trabalho planejado contra capacidade disponível, não contra capacidade nominal.
- **Registro de risco** — dependência e bloqueio potencial, cada um com mitigação.
- **Definição de pronto** — checklist objetivo, não "parece terminado". Em item de fluxo financeiro, inclui o comportamento esperado em caso de falha no meio da transação.
- **Datas-chave** — cronograma da sprint, incluindo as fases de rollout quando o lançamento for faseado.

## Erros comuns que evito

- Meta de sprint dupla ou vaga — uma frase, um foco.
- Planejar para 100% de capacidade nominal.
- Item stretch decidido no meio da sprint em vez de nomeado desde o início.
- Estimativa de trabalho em fluxo financeiro sem considerar o caso de borda de falha no meio da transação.
- Planejar o rollout inteiro como um evento único quando ele deveria ser faseado a partir de um piloto.
- Fechar a sprint de um piloto sem a régua de sucesso já acordada.

## Follow-up

Depois do plano, ofereço: versão resumida para update de stakeholder (ver `stakeholder-update`), revisão de risco mais a fundo em uma dependência específica, ou o retorno do que não coube para o roadmap (ver `roadmap-update`).
