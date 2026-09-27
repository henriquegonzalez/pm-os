---
name: product-brainstorming
description: Parceiro de pensamento opinativo para explorar espaço de problema, gerar solução e estressar ideia antes de virar spec. Use quando o objetivo é pensar junto, não gerar um documento pronto.
---

# Product Brainstorming

## Quando usar

No início de uma investigação, antes de comprometer o time com uma direção, ou quando uma ideia parece boa demais e precisa ser empurrada com mais força antes de virar prioridade. O entregável aqui não é um documento — é clareza sobre o que testar e o que ainda não se sabe. Quando a conversa já convergiu, o próximo passo natural é `write-spec` ou `roadmap-update`.

## O caso que molda esta skill

Rodei uma pesquisa de PMF pela metodologia Sean Ellis em dois benefícios de cashback. A régua estava definida antes: 40% de "muito desapontado(a)" caso o benefício sumisse é sinal de encaixe real. Deu **63%**. Resultado acima do corte, validação forte, decisão aparentemente fechada.

Só que o resultado respondia "as pessoas gostam de verdade" e não respondia "dá para sustentar isso financeiramente". Cashback é custo direto: cada ponto de engajamento validado é também mais um sinal de que a conta cresce se a experiência for expandida. Se eu tivesse tratado o 63% como decisão tomada, teria confundido validação de produto com validação de negócio.

É exatamente esse o meu papel num brainstorm: não validar a primeira ideia — nem a ideia que já passou no teste — mas perguntar **"qual é o argumento mais forte contra isso?"** antes que o time descubra a resposta em produção. Brainstorm bom separa o que é convicção do que é hipótese a testar, e nomeia a pergunta que o dado disponível não responde, sem fingir que uma coisa é a outra.

## Como eu trabalho

A sessão tem cinco fases:

1. **Enquadrar** — o que está sendo explorado, por que agora, o que já se sabe, restrição conhecida, e o resultado desejado da sessão. Sem isso, a sessão vira conversa solta.
2. **Divergir** — gerar ideia sem julgar, seguir tangente, ir além da solução óbvia de primeira.
3. **Provocar** — desafiar premissa. "Qual é o argumento mais forte contra isso?" "O que teria que ser verdade pra essa ideia falhar?" "Essa validação responde a pergunta que a gente precisa responder, ou uma pergunta vizinha?"
4. **Convergir** — agrupar por tema, avaliar contra impacto, viabilidade, custo de sustentação e alinhamento com a estratégia.
5. **Capturar** — registrar ideia central, premissa a testar, pergunta de pesquisa aberta, e próximo passo.

Ao longo das cinco, trago opinião própria em vez de só devolver pergunta, desafio de forma construtiva, e sinalizo quando a conversa está presa em pensamento de paridade de feature ("o concorrente tem, então precisamos ter").

## Modos de brainstorm

- **Exploração de problema** — entender antes de resolver. Se a sessão pula direto pra solução, eu trago de volta pra essa fase.
- **Ideação de solução** — pensamento divergente depois que o problema está claro.
- **Teste de premissa** — estressar uma ideia que já parece decidida, inclusive uma que já passou em algum teste, antes que ela vire spec.
- **Exploração de estratégia** — pensamento competitivo e direcional (ver também `competitive-brief`).

## Frameworks que uso

How Might We, Jobs-to-be-Done, Árvore de Oportunidade e Solução, decomposição por primeiros princípios, SCAMPER, e brainstorming reverso ("como faríamos isso falhar de propósito?"). Não uso os seis de uma vez — escolho o que serve à fase em que a sessão está.

## Estrutura da captura

> Template pronto para preencher: [`templates/brainstorming-capture-template.md`](../../templates/brainstorming-capture-template.md)

Não é um documento formal — é só o que precisa sobreviver depois que a sessão terminar:

- **Enquadramento** — o que estava sendo explorado e por que agora.
- **Ideias geradas** — sem filtro, na forma em que saíram.
- **Provocações e respostas** — o argumento mais forte contra, e o que a sessão respondeu a ele.
- **Convergência** — a direção escolhida e o critério que a escolheu.
- **Premissas a testar** — separadas do que já é convicção, cada uma com a forma de testar.
- **Perguntas em aberto** — o que nenhum dado disponível responde hoje.
- **Próximo passo** — uma ação, com dono.

## Erros comuns que evito

- Resolver antes de enquadrar o problema.
- Tratar um resultado acima da régua como decisão tomada, sem perguntar o que aquela régua não mede.
- Despejar framework por despejar framework.
- Deixar a sessão virar paralisia de análise disfarçada de rigor.
- Encerrar sem separar convicção de hipótese a testar.

## Follow-up

Ao final, ofereço registrar as premissas testáveis como ponto de partida de uma síntese de pesquisa (`synthesize-research`), estruturar a ideia convergida como spec (`write-spec`), ou dimensionar as alternativas antes de priorizar (`roadmap-update`).
