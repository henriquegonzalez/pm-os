---
name: manage-external-dependency
description: Trata dependência de terceiro — parceiro comercial, processadora, fornecedor, outra squad — como escopo de produto, com dono, data de decisão e plano B. Use quando parte do resultado depende de alguém que não responde ao seu time.
---

# Manage External Dependency

## Quando usar

Quando a entrega depende de acesso, integração, contrato ou decisão de alguém fora do seu controle direto. Também quando um benchmark concluiu que a vantagem do concorrente veio de negociação e não de engenharia (ver `competitive-brief`), ou quando um PRD tem uma seção de dependências externas que ninguém está tocando (ver `write-spec`).

O sinal de que esta skill é necessária: a pergunta "quando isso fica pronto?" não tem resposta porque ninguém no time sabe quando a outra parte responde.

## O caso que molda esta skill

No redesenho de um menu de benefícios, a decisão que mais moveu o resultado não foi de design — foi conseguir **acesso logado com a bandeira parceira**, o que exigia mudar a integração técnica e o acordo comercial, não só a tela. Essa negociação levou mais tempo do que qualquer parte do desenho de produto, e foi ela que destravou o ganho medido depois do rollout.

O erro que quase cometi foi o padrão: tratar isso como "risco de implementação a resolver depois". Não é risco, é escopo. Um trabalho que depende de terceiro tem um calendário que não é o seu, e ignorar isso não o encurta — só transforma um prazo conhecido em atraso não comunicado.

O mesmo padrão apareceu de outra forma ao tirar uma prateleira de benefícios de dentro do domínio de uma processadora parceira: desacoplar de um parceiro técnico é, na prática, um projeto de migração disfarçado de decisão de produto. Subestimei o tempo até estar no meio dele.

**A regra que sobrou:** dependência de parceiro entra no escopo no dia 1, com dono dos dois lados, ou vira surpresa no dia 60.

## Como eu trabalho

1. **Classificar a dependência.** Construir (dá para resolver sozinho, com mais esforço), negociar (só existe com acordo do outro lado), ou contornar (existe um caminho pior que não depende de ninguém). Times gastam semanas discutindo prazo de algo que estava na terceira categoria desde o começo.
2. **Nomear dono dos dois lados.** Uma pessoa aqui, uma pessoa lá, com nome. "O time deles" não é dono; é um jeito educado de dizer que ninguém é.
3. **Descobrir o que o outro lado ganha.** Uma dependência só avança no ritmo do interesse da outra parte. Se eu não consigo articular o que eles ganham, ainda não entendi a negociação — e o prazo que eu prometer é ficção.
4. **Definir a data de decisão, não a data de entrega.** Eu não controlo quando eles entregam; controlo até quando vale a pena esperar. Essa data vai para o roadmap e para o plano de sprint.
5. **Desenhar o plano B e o gatilho que o aciona.** O plano B é escrito antes de ser necessário, e o gatilho é a data de decisão do passo anterior — não "quando ficar claro que não vai dar".
6. **Reportar status real, sempre.** "Em andamento" não é status. Status é: com quem está, o que essa pessoa precisa para responder, e quando ela disse que responde (ver `stakeholder-update`).

## Regra de proveniência dos números

Data e compromisso vindos de terceiro são `a confirmar` até existir acordo escrito — e continuam `a confirmar` num roadmap ou num update, por mais confiante que a conversa tenha soado. Estimativa de esforço de integração é `estimativa`. Só vira `medido` o que já aconteceu. Prazo de parceiro tratado como `meta` no roadmap é a origem mais comum de dívida de confiança com liderança.

## Estrutura do registro de dependência

> Template pronto para preencher: [`templates/external-dependency-template.md`](../../templates/external-dependency-template.md)

- **O que depende de quem** — a capacidade bloqueada e a organização do outro lado.
- **Classificação** — construir, negociar ou contornar, com o porquê.
- **Donos** — nome aqui, nome lá, e o canal onde a conversa acontece.
- **O que o outro lado ganha** — a razão pela qual isso avança sem cobrança.
- **Data de decisão** — até quando vale esperar, e quem decide seguir ou não.
- **Plano B** — o caminho sem eles, com o custo explícito de tomá-lo.
- **Gatilho do plano B** — a condição objetiva que o aciona.
- **Impacto no escopo** — o que muda no PRD, no roadmap e na sprint em cada cenário.
- **Status real** — última conversa, o que foi pedido, o que falta, próxima data.

## Erros comuns que evito

- Tratar dependência de parceiro como risco de implementação em vez de escopo de produto.
- Prometer data de entrega sobre trabalho que depende de terceiro.
- "O time deles" como dono da dependência.
- Negociar sem saber o que a outra parte ganha.
- Deixar o plano B para quando o plano A já falhou.
- Reportar "em andamento" no lugar do status real da conversa.
- Confundir desacoplamento técnico com projeto de tela — quase sempre é migração de dados e de base legada.

## Follow-up

Depois do registro, ofereço: a seção de dependências externas do PRD já escrita (ver `write-spec`), o risco com dono no roadmap (ver `roadmap-update`), o registro de risco da sprint (ver `sprint-planning`), ou a versão do status para o parceiro e para liderança (ver `stakeholder-update`).
