---
name: sprint-planning
description: Ajuda a escopar trabalho, estimar capacidade real do time e montar um plano de sprint com meta única e riscos explícitos. Use no planejamento de uma nova sprint ou em refinamento de backlog.
---

# Sprint Planning

## Quando usar

Início de sprint, refinamento de backlog, ou quando um time precisa decidir o que cabe de fato no ciclo — não o que caberia numa semana ideal que não existe.

## Como eu trabalho

1. **Levantar informação real do time** — composição, duração da sprint, itens priorizados de backlog, trabalho que ficou da sprint anterior (carryover), e dependências conhecidas. Carryover não é detalhe — é o primeiro sinal de que a estimativa passada estava otimista.
2. **Estimar capacidade de verdade** — disponibilidade de cada pessoa considerando férias, reuniões recorrentes e qualquer alocação parcial em outro time. Capacidade nominal (todo mundo, tempo todo) não existe na prática.
3. **Escopar e priorizar** — categorizo item de backlog em P0 (compromisso da sprint), P1 (entra se sobrar capacidade) e P2 (próxima sprint). Deixo explícito quais itens são "stretch" para negociar escopo se o ciclo apertar, em vez de negociar isso de surpresa no meio da sprint.
4. **Identificar risco** — dependência de outro time, decisão pendente, ou trabalho técnico não estimado ainda. Cada risco tem uma mitigação, não só um registro de "isso pode dar problema".
5. **Gerar o plano** (estrutura abaixo).

## Regra de capacidade

Planejo para 70-80% da capacidade nominal do time, nunca 100%. A margem não é desperdício — é o espaço para a interrupção que sempre aparece (bug crítico, pedido urgente, ausência não planejada). Time que planeja pra 100% da capacidade não entrega mais rápido; só acumula carryover e perde a meta da sprint com mais frequência.

Em produto que toca fluxo financeiro (pagamento, saldo, limite), reservo atenção extra na estimativa para item que envolve trava ou reversão de transação — esse tipo de trabalho quase sempre estima curto na primeira passada, porque o caso de borda (o que acontece quando algo falha no meio do fluxo) raramente aparece na estimativa inicial.

## Estrutura do plano de sprint

- **Metadados** — datas, tamanho do time, uma meta de sprint em uma frase só.
- **Tabela de capacidade** — tempo disponível e alocação de cada pessoa.
- **Backlog da sprint** — organizado por prioridade, com estimativa e responsável.
- **Cálculo de carga** — trabalho planejado contra capacidade disponível, não contra capacidade nominal.
- **Registro de risco** — dependência e bloqueio potencial, cada um com mitigação.
- **Definição de pronto** — checklist objetivo, não "parece terminado".
- **Datas-chave** — cronograma da sprint.

## Erros comuns que evito

- Meta de sprint dupla ou vaga — uma frase, um foco.
- Planejar para 100% de capacidade nominal.
- Item stretch decidido no meio da sprint em vez de nomeado desde o início.
- Estimativa de trabalho em fluxo financeiro sem considerar o caso de borda de falha no meio da transação.

## Follow-up

Depois do plano, ofereço: versão resumida para update de stakeholder (ver `stakeholder-update`), ou revisão de risco mais a fundo em uma dependência específica.
