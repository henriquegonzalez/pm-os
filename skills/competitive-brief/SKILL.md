---
name: competitive-brief
description: Gera um brief de análise competitiva para embasar estratégia de produto, priorização de feature ou material de negociação. Use quando precisar entender onde o produto está em desvantagem ou vantagem real contra concorrentes específicos.
---

# Competitive Brief

## Quando usar

Antes de redesenhar uma área de produto que já tem concorrência madura, antes de uma negociação com parceiro comercial que também atende concorrentes, ou quando liderança pede "como estamos contra X" e a resposta não pode ser opinião.

## O caso que molda esta skill

Para redesenhar um menu de benefícios, fiz benchmark de **16 produtos concorrentes** com SWOT completo antes de desenhar qualquer tela. Isso sozinho não teria virado nada — benchmark de feature é fácil de fazer e fácil de ignorar. O que mudou o jogo foi cruzar o SWOT com um **workshop de dores** rodado com os times de atendimento e CS: só quando as duas coisas se encontraram — o que os concorrentes tinham e o que os nossos clientes de fato reclamavam — deu para separar feature vistosa de feature que resolvia dor real.

E o achado que mais moveu o resultado não era uma feature: era que parte da experiência dependia de negociar acesso logado com a bandeira parceira — mudança de integração técnica e de acordo comercial, não de tela. Um benchmark que só compara interface não serve para decidir prioridade; serve para decidir **onde abrir conversa fora do time**. Depois do rollout, o segmento priorizado teve acesso ao menu cerca de 5x maior (`medido`); retenção e NPS seguem `a confirmar`.

## Como eu trabalho

1. **Escopar a análise** — quais concorrentes, qual foco (comparação completa, feature específica, posicionamento, pricing) e qual decisão de negócio essa análise vai embasar. Um benchmark sem decisão de destino vira relatório que ninguém lê.
2. **Pesquisar com fonte rastreável** — páginas de produto, pricing, lançamentos, cobertura de imprensa, reviews de usuário, vagas abertas (revelam prioridade de investimento do concorrente). Cada achado carrega a fonte, para poder ser conferido depois.
3. **Cruzar com dor interna.** Benchmark isolado leva a copiar concorrente. Cruzo o levantamento com o que atendimento, CS e suporte já ouvem todo dia — é isso que separa paridade de feature de problema real.
4. **Gerar o brief** (estrutura abaixo).
5. **Separar o que é "copiar tela" do que é "abrir negociação".** Toda vantagem competitiva que depende de acesso a um parceiro externo, dado exclusivo, ou escala que a empresa ainda não tem, entra numa seção própria — não misturada com gap de feature que o time consegue resolver sozinho.

## Regra de proveniência dos números

Todo número e toda afirmação de capacidade no brief carrega origem: `medido` (dado público verificável, página de pricing, release note) · `estimativa` (inferência a partir de sinal indireto, como vaga aberta ou cobertura de imprensa) · `a confirmar` (ouvido, não verificado). Afirmação de concorrente sem fonte rastreável não entra no brief — vira pergunta aberta.

## Estrutura do brief

> Template pronto para preencher: [`templates/competitive-brief-template.md`](../../templates/competitive-brief-template.md)

- **Visão geral dos concorrentes** — quem são, porte, posicionamento declarado.
- **Matriz de comparação de features** — capacidade por concorrente, com escala simples (tem / não tem / parcial) ou detalhada quando o gap for sutil.
- **Análise de posicionamento** — mensagem, reivindicação de categoria, diferenciação declarada de cada concorrente.
- **Forças e fraquezas** — com evidência (review de usuário, dado público), não opinião do time.
- **Vantagens que dependem de terceiro** — o que um concorrente tem porque negociou acesso, exclusividade ou parceria — não porque construiu melhor. Essa distinção decide se a resposta certa é "construir" ou "negociar".
- **Cruzamento com dor interna** — quais gaps do benchmark batem com reclamação recorrente de cliente, e quais não batem com nada.
- **Oportunidades e ameaças** — lacunas de mercado e riscos competitivos.
- **Implicações estratégicas** — recomendação amarrada de volta à decisão que motivou o benchmark.

## Erros comuns que evito

- Comparar feature sem marcar quais dependem de acesso/parceria que o concorrente tem e nós não.
- Benchmark genérico sem decisão de destino clara.
- Levantar concorrente sem cruzar com a dor que o atendimento já ouve — é assim que se copia feature que não resolve nada aqui.
- SWOT com "fraquezas" que são só opinião do time, sem evidência.
- Ignorar vaga aberta e cobertura de imprensa como sinal de prioridade de investimento do concorrente.

## Follow-up

Depois do brief, ofereço: resumo executivo de uma página, battle card para time comercial, plano de monitoramento contínuo do concorrente mais relevante, ou levar os gaps priorizados direto para o roadmap (ver `roadmap-update`). Quando a conclusão for "precisamos decidir entre construir e negociar", o próximo passo natural é `product-brainstorming`.
