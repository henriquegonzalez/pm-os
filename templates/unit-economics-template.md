# Unit Economics: [benefício/plano/feature]

> Skill de origem: `pricing-unit-economics`. Todo número carrega etiqueta de proveniência: `medido` · `meta` · `estimativa` · `a confirmar`. Receita incremental atribuída a um benefício quase sempre é `estimativa` — dizer isso é mais útil do que fingir precisão.

**Data:** [AAAA-MM-DD] · **Autor:** [nome]

## A decisão em jogo

**Decisão:** [expandir · manter · reduzir · cortar]
**Quem decide:** [nome/área]
**Prazo da decisão:** [AAAA-MM-DD]

## Evidência de desejo

*(O que já se sabe sobre o quanto as pessoas querem isso — e nada além disso. Esta seção não responde a pergunta da conta.)*

| Evidência | Fonte | Resultado | Etiqueta |
|---|---|---|---|
| [ex.: pesquisa de PMF, metodologia Sean Ellis] | [amostra, critério de elegibilidade, data] | [ex.: 63% vs. corte de 40%] | `medido` |

## A unidade

**O que está sendo contado:** [um cliente · um mês · uma transação]
**Janela:** [período]

*(Uma unidade clara vale mais do que um total anual que ninguém consegue decompor.)*

## Conta por unidade

| Linha | Valor | Etiqueta | Fonte |
|---|---|---|---|
| Receita incremental por usuário beneficiado | [valor] | `estimativa` | [como foi atribuída] |
| (−) Custo do benefício por usuário | [valor] | `medido` | [sistema/apuração] |
| (−) Outros custos variáveis por usuário | [valor] | [etiqueta] | [fonte] |
| **= Contribuição por unidade** | **[valor]** | | |

## O que escala com o uso

*(Custo fixo de construir é uma coisa; custo que cresce a cada transação é outra completamente diferente.)*

| Custo | Fixo ou variável | Cresce com o quê | Tem teto? |
|---|---|---|---|
| [custo] | [fixo/variável] | [transação, saldo, usuário ativo] | [sim/não — qual] |

## Contrapartida de comportamento

[O que o cliente faz que sustenta o benefício, se houver. Ex.: liberação proporcional ao pagamento da fatura — o benefício cresce junto com o comportamento que paga por ele, em vez de crescer sozinho.]

**Se não houver contrapartida:** [teto, régua de elegibilidade ou outro mecanismo de contenção proposto]

## Sensibilidade

*(As duas ou três variáveis que viram o sinal da conta — não dezenas de cenários.)*

| Variável | Valor atual | Ponto de virada | Etiqueta |
|---|---|---|---|
| [variável] | [valor] | [a partir de que valor a conta deixa de fechar] | [etiqueta] |

## Cenários

| Cenário | Efeito na conta | Efeito no cliente |
|---|---|---|
| Expandir | [contribuição resultante] | [o que melhora/piora] |
| Manter | [contribuição resultante] | [o que melhora/piora] |
| Reduzir | [contribuição resultante] | [o que melhora/piora] |

## Divergência entre desejo e sustentação

*(Quando as duas respostas apontam para lados diferentes. Seção própria, nunca ressalva de rodapé — é perfeitamente coerente concluir "as pessoas amam e vamos reduzir o escopo mesmo assim".)*

[O que o desejo indica · o que a conta indica · a recomendação e o porquê]

## Gatilho de revisão

**Qual número:** [métrica] · **Medido quando:** [janela/data] · **Reabre a decisão se:** [condição]

*(Sem isso, um benefício caro continua rodando por inércia muito depois de deixar de fazer sentido.)*

## O que ainda não sei

- [Lacunas `a confirmar` que impedem uma conclusão mais forte — deixadas visíveis, não preenchidas com chute]
