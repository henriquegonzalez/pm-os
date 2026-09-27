---
name: pricing-unit-economics
description: Avalia se um benefício, plano ou feature se sustenta financeiramente — custo por usuário, o que escala com o uso e a partir de que ponto a conta vira. Use quando a validação de desejo já existe e falta responder se dá para pagar por ela.
---

# Pricing & Unit Economics

## Quando usar

Quando uma pesquisa, um piloto ou um resultado de engajamento já mostrou que as pessoas querem aquilo, e a pergunta seguinte — se a empresa consegue continuar pagando — ainda está em aberto. Também antes de expandir um benefício que já existe, de mudar a régua de um plano pago, ou de decidir entre cortar e reduzir.

Esta skill começa exatamente onde `synthesize-research` e `design-experiment` param: elas medem desejo, esta mede sustentação.

## O caso que molda esta skill

Rodei uma pesquisa de PMF pela metodologia Sean Ellis em dois benefícios de cashback. A régua estava definida antes — 40% de "muito desapontado(a)" é sinal de encaixe real — e o resultado veio bem acima: 63%. Validação forte, decisão aparentemente fechada a favor de expandir a experiência.

Só que cashback tem um problema estrutural: **cada real devolvido ao cliente é custo direto**. Cada ponto de engajamento validado pela pesquisa é, ao mesmo tempo, mais um sinal de que o custo do benefício vai continuar — ou crescer — se a experiência for expandida em cima dele. Terminei a pesquisa com uma validação forte de amor ao produto e exatamente a mesma pergunta em aberto que tinha antes.

Sou honesto sobre o limite disto: eu tenho a pergunta bem formulada, não a conta fechada. O que esta skill carrega é o hábito de não deixar as duas perguntas se confundirem. **PMF mede desejo, não mede se o desejo cabe no orçamento** — são perguntas independentes, e resolver a primeira não adianta a segunda. Se eu tivesse decidido "expandir tudo" só com o 63% na mão, teria confundido validação de produto com validação de negócio.

## Como eu trabalho

1. **Separar as duas perguntas, por escrito.** "As pessoas querem?" e "dá para sustentar?" recebem seções próprias, com evidências próprias. A maior parte da confusão nasce de responder a primeira e dar a segunda por respondida.
2. **Montar a conta por unidade.** Receita incremental por usuário beneficiado, menos o custo do benefício por usuário, na mesma janela de tempo. Uma unidade clara — um cliente, um mês — vale mais do que um total anual que ninguém consegue decompor.
3. **Identificar o que escala com o uso e o que não escala.** Custo fixo de construir é uma coisa; custo que cresce a cada transação é outra completamente diferente. Benefício cujo custo escala com sucesso precisa de teto, régua de elegibilidade ou contrapartida de comportamento.
4. **Amarrar o benefício a um comportamento que paga por ele, quando der.** No caso do cashback, a liberação proporcional ao pagamento da fatura é exatamente isso: o benefício cresce junto com o comportamento que sustenta a conta, em vez de crescer sozinho.
5. **Testar sensibilidade nas duas ou três variáveis que mais mexem.** Não modelo dezenas de cenários; acho as variáveis que viram o sinal da conta e mostro a partir de que valor ela deixa de fechar.
6. **Definir o gatilho de revisão.** Qual número, medido quando, obriga a revisitar a decisão. Sem isso, um benefício caro continua rodando por inércia muito depois de deixar de fazer sentido.
7. **Gerar a análise** (estrutura abaixo), com cada número etiquetado.

## Regra: desejo e sustentação são perguntas independentes

Um resultado acima da régua de PMF autoriza investir em experiência; não autoriza expandir custo. As duas decisões usam evidências diferentes e podem ir em direções opostas — é perfeitamente coerente concluir "as pessoas amam e vamos reduzir o escopo mesmo assim". Quando as duas respostas divergem, isso vira uma seção própria da análise, não uma ressalva no rodapé.

## Regra de proveniência dos números

Custo unitário apurado de sistema é `medido`. Receita incremental atribuída ao benefício quase sempre é `estimativa`, porque separar o efeito do benefício do resto é difícil — e dizer isso é mais útil do que fingir precisão. Meta de contribuição definida antes é `meta`. Variável de modelo sem fonte é `a confirmar`, e a análise sai assim mesmo, com a lacuna visível.

## Estrutura da análise

> Template pronto para preencher: [`templates/unit-economics-template.md`](../../templates/unit-economics-template.md)

- **A decisão em jogo** — expandir, manter, reduzir ou cortar, e quem decide.
- **Evidência de desejo** — o que já se sabe sobre o quanto as pessoas querem isso, com a fonte.
- **A unidade** — o que está sendo contado (um cliente, um mês, uma transação).
- **Conta por unidade** — receita incremental, custo do benefício, contribuição resultante.
- **O que escala com o uso** — custos que crescem junto com o sucesso, nomeados separadamente dos fixos.
- **Contrapartida de comportamento** — o que o cliente faz que sustenta o benefício, se houver.
- **Sensibilidade** — as duas ou três variáveis que viram o sinal, e o ponto de virada de cada uma.
- **Cenários** — expandir, manter e reduzir, com o efeito na conta e no cliente.
- **Divergência entre desejo e sustentação** — quando as duas respostas apontam para lados diferentes.
- **Gatilho de revisão** — qual número, medido quando, reabre a decisão.
- **O que ainda não sei** — as lacunas `a confirmar` que impedem uma conclusão mais forte.

## Erros comuns que evito

- Tratar validação de desejo como se fosse validação de negócio.
- Somar custo total anual sem conseguir decompor por unidade.
- Esquecer que benefício com custo variável fica mais caro exatamente quando dá certo.
- Modelar dezenas de cenários em vez de achar as poucas variáveis que viram a conta.
- Expandir experiência em cima de um benefício sem teto nem contrapartida.
- Fechar a análise sem gatilho de revisão — é assim que custo vira inércia.
- Esconder a lacuna: se a receita incremental é chute, o número sai etiquetado como chute.

## Follow-up

Depois da análise, ofereço: o desenho da medição do gatilho de revisão (ver `design-experiment`), a versão da conclusão por audiência, especialmente quando desejo e sustentação divergem (ver `stakeholder-update`), o reflexo no escopo e nos não-objetivos do PRD (ver `write-spec`), ou a repriorização da aposta com a conta na mão (ver `roadmap-update`).
