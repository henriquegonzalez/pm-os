---
name: write-spec
description: Escreve specs e PRDs com escopo defensável — non-goals explícitos, critérios de aceite testáveis e proveniência clara de cada número. Use quando precisar transformar um pedido de feature em um documento que engenharia possa estimar sem pressupor nada escondido.
---

# Write Spec

## Quando usar

Sempre que um pedido de feature, dor de usuário ou aposta de negócio precisa virar um documento que outro time (engenharia, design, dados) vai estimar e construir. Também serve para formalizar depois de um brainstorm ou uma síntese de pesquisa — ver `product-brainstorming` e `synthesize-research`.

## O caso que molda esta skill

Escrevi a spec de uma prateleira de pacotes de benefícios que precisava sair de dentro do domínio de uma processadora parceira e passar a rodar em domínio próprio. O corte de escopo mais importante não foi nenhuma feature da prateleira nova: foi reconhecer que aquilo era, na prática, uma migração de base legada disfarçada de decisão de produto. Carência e reversão para quem já tinha benefício ativo entraram como requisito bloqueante de lançamento; "redesenhar toda a prateleira" virou não-objetivo da primeira fase, com o porquê escrito ao lado. Sem essa separação, engenharia teria estimado a tela nova e descoberto a migração no meio do caminho.

A lição que carrego para todo PRD desde então: **a UX da transição é escopo, não detalhe de implementação** — e tudo que não está sob controle do time (parceiro comercial, processadora, outra squad) é dependência externa nomeada, com dono e data, nunca uma linha escondida dentro de "requisitos técnicos".

## Como eu trabalho

1. **Entender o pedido além do pedido.** Quase nunca o primeiro enunciado é o problema real. Antes de escrever qualquer seção, pergunto: quem sente essa dor, com que frequência, e o que a empresa perde enquanto ela não é resolvida. Se a resposta for "não sei", isso vira a primeira pergunta aberta do doc — não escrevo em torno de um vácuo.
2. **Levantar contexto real, não genérico.** Puxo dado de suporte, pesquisa já feita (ver `synthesize-research`), métricas atuais (ver `metrics-review`) e qualquer decisão anterior relacionada. Se nada disso existir, registro explicitamente que o PRD parte de hipótese, não de evidência.
3. **Separar o que é construir do que é migrar.** Se existe base legada, integração a desligar ou contrato a renegociar, isso é escopo de primeira classe: entra como requisito e como não-objetivo explícito do que fica para depois.
4. **Gerar o documento estruturado** (seções abaixo).
5. **Iterar em cima de objeção real.** A primeira versão do PRD é para ser atacada, não aprovada. As melhores mudanças de escopo que já fiz vieram de alguém apontando uma dependência que eu tinha escondido dentro de "requisitos técnicos".

## Regra de proveniência dos números

Todo número que entra no PRD carrega uma etiqueta: `medido` · `meta` · `estimativa` · `a confirmar`. Nunca escrevo um número "nu" no documento. Se a origem não está clara, marco como `a confirmar` e sigo — isso é mais útil do que fingir precisão que não existe, e evita que alguém tome decisão de engenharia em cima de um chute vestido de dado.

## Estrutura do PRD

> Template pronto para preencher: [`templates/prd-template.md`](../../templates/prd-template.md)

- **Problema** — 2-3 frases. Quem é afetado, com que frequência, e o impacto de negócio de não resolver.
- **Contexto e evidência** — de onde vem a convicção de que isso é real (pesquisa, dado, ticket de suporte, pedido recorrente de vendas).
- **Objetivos** — 3-5 metas mensuráveis. Nunca "melhorar a experiência" sem número associado.
- **Não-objetivos** — o que fica de fora, com o porquê. Esta é a seção que mais evita retrabalho depois; escrevo mesmo quando parece óbvio.
- **Histórias de usuário** — "Como [tipo de usuário], eu quero [capacidade] para que [benefício]."
- **Requisitos** — categorizados em P0 (bloqueante de lançamento), P1 (desejável), P2 (futuro), cada um com critério de aceite no formato Given/When/Then.
- **Dependências externas** — qualquer coisa que não está sob controle do time (parceiro comercial, outra squad, fornecedor). Tem dono e data, e nunca fica escondida dentro de "requisitos técnicos".
- **Métricas de sucesso** — indicadores líderes (adoção, conclusão) e atrasados (retenção, receita), cada um já com a fonte de medição definida antes do lançamento, não depois.
- **Perguntas abertas** — o que ainda não sei, marcado com quem precisa responder.
- **Cronograma** — prazos, fases, o que depende do quê.

## Erros comuns que evito

- Objetivo vago sem meta mensurável associada.
- Non-goals implícitos, que só aparecem quando alguém pergunta depois de o time já estar construindo.
- Critério de aceite que não é testável ("deve ser intuitivo").
- Dependência externa escondida dentro de "requisitos técnicos" em vez de nomeada como risco com dono.
- Tratar migração de base legada como detalhe de implementação em vez de escopo com requisito próprio.
- Número sem proveniência — todo dado no doc diz de onde veio.

## Follow-up

Depois da primeira versão, ofereço: resumo executivo de uma página para liderança (ver `stakeholder-update`), checklist de prontidão para revisão de engenharia, ou o desenho da medição das métricas de sucesso especificadas (ver `metrics-review`) — nunca as três coisas misturadas no mesmo documento.
