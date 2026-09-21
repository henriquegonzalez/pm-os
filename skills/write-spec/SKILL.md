---
name: write-spec
description: Escreve specs e PRDs com escopo defensável — non-goals explícitos, critérios de aceite testáveis e proveniência clara de cada número. Use quando precisar transformar um pedido de feature em um documento que engenharia possa estimar sem pressupor nada escondido.
---

# Write Spec

## Quando usar

Sempre que um pedido de feature, dor de usuário ou aposta de negócio precisa virar um documento que outro time (engenharia, design, dados) vai estimar e construir. Também serve para formalizar depois de um brainstorm ou uma síntese de pesquisa — ver `product-brainstorming` e `synthesize-research`.

## Como eu trabalho

1. **Entender o pedido além do pedido.** Quase nunca o primeiro enunciado é o problema real. Antes de escrever qualquer seção, pergunto: quem sente essa dor, com que frequência, e o que a empresa perde enquanto ela não é resolvida. Se a resposta for "não sei", isso vira a primeira pergunta aberta do doc — não escrevo em torno de um vácuo.
2. **Levantar contexto real, não genérico.** Puxo dado de suporte, pesquisa já feita (ver `synthesize-research`), métricas atuais (ver `metrics-review`) e qualquer decisão anterior relacionada. Se nada disso existir, registro explicitamente que o PRD parte de hipótese, não de evidência.
3. **Gerar o documento estruturado** (seções abaixo).
4. **Iterar em cima de objeção real.** A primeira versão do PRD é para ser atacada, não aprovada. As melhores mudanças de escopo que já fiz vieram de alguém apontando uma dependência que eu tinha escondido dentro de "requisitos técnicos".

## Estrutura do PRD

- **Problema** — 2-3 frases. Quem é afetado, com que frequência, e o impacto de negócio de não resolver.
- **Contexto e evidência** — de onde vem a convicção de que isso é real (pesquisa, dado, ticket de suporte, pedido recorrente de vendas).
- **Objetivos** — 3-5 metas mensuráveis. Nunca "melhorar a experiência" sem número associado.
- **Não-objetivos** — o que fica de fora, com o porquê. Esta é a seção que mais evita retrabalho depois; escrevo mesmo quando parece óbvio.
- **Histórias de usuário** — "Como [tipo de usuário], eu quero [capacidade] para que [benefício]."
- **Requisitos** — categorizados em P0 (bloqueante de lançamento), P1 (desejável), P2 (futuro), cada um com critério de aceite no formato Given/When/Then.
- **Dependências externas** — qualquer coisa que não está sob controle do time (parceiro comercial, outra squad, fornecedor). Tem dono e data, e nunca fica escondida dentro de "requisitos técnicos".
- **Métricas de sucesso** — indicadores líderes (adoção, conclusão) e atrasados (retenção, receita), cada um já com a fonte de medição definida.
- **Perguntas abertas** — o que ainda não sei, marcado com quem precisa responder.
- **Cronograma** — prazos, fases, o que depende do quê.

## Regra de proveniência dos números

Todo número que entra no PRD carrega uma etiqueta: `medido` · `meta` · `estimativa` · `a confirmar`. Nunca escrevo um número "nu" no documento. Se a origem não está clara, marco como `a confirmar` e sigo — isso é mais útil do que fingir precisão que não existe, e evita que alguém tome decisão de engenharia em cima de um chute vestido de dado.

## Lição de campo

No PRD do redesenho de um menu de benefícios que conduzi, o corte de escopo mais importante não foi uma feature — foi o acesso logado do usuário depender de uma negociação direta com o parceiro (a bandeira do cartão). Isso não cabia como "requisito técnico" porque não estava sob controle do time. Entrou como dependência externa explícita, com dono e data. Sem isso, engenharia teria estimado em cima de uma pressuposição que ninguém tinha autoridade para garantir.

## Erros comuns que evito

- Objetivo vago sem meta mensurável associada.
- Non-goals implícitos, que só aparecem quando alguém pergunta depois de o time já estar construindo.
- Critério de aceite que não é testável ("deve ser intuitivo").
- Dependência externa escondida dentro de "requisitos técnicos" em vez de nomeada como risco com dono.
- Número sem proveniência — todo dado no doc diz de onde veio.

## Follow-up

Depois da primeira versão, ofereço: resumo executivo de uma página para liderança, ou checklist de prontidão para revisão de engenharia — nunca as duas coisas misturadas no mesmo documento.
