---
name: stakeholder-update
description: Gera comunicação de status adaptada à audiência — update semanal, resumo mensal, anúncio de lançamento ou escalonamento pontual. Use quando o mesmo progresso precisa ser contado de formas diferentes para liderança, engenharia, parceiro externo ou cliente.
---

# Stakeholder Update

## Quando usar

Update recorrente de progresso, anúncio de lançamento, ou comunicação pontual sobre uma mudança de rumo, atraso ou resultado — especialmente quando o resultado não é uma vitória limpa.

## O caso que molda esta skill

A parte mais difícil de comunicar não é o progresso — é o resultado misto. Quando a fricção que adicionei num fluxo de upgrade melhorou a conversão em 1,1 p.p., piorou o retorno no mesmo dia em 18 p.p. e deixou o abandono geral parado em ~89%, a comunicação certa não escolheu qual dos três mostrar: mostrou os três, junto com o que isso significava para a decisão seguinte. Quem recebe esse tipo de update aprende a confiar no próximo, porque sabe que não vai receber só a parte boa.

O segundo caso que moldou esta skill foi de outra natureza: comunicar a saída de um menu de benefícios do domínio de uma processadora parceira para domínio próprio. Ali o update não era sobre feature nova, era sobre **migração de base legada** — carência, reversão, quem perde acesso quando e por quanto tempo. Cada audiência precisava de uma versão diferente do mesmo fato, e a frente que dependia do parceiro precisava ser reportada com status real da conversa, não "em andamento" genérico.

## Como eu trabalho

1. **Definir o tipo de update** — progresso semanal, resumo mensal, anúncio de lançamento, ou escalonamento pontual. Cada um tem um nível de detalhe e uma urgência diferentes.
2. **Identificar a audiência** — executivo, engenharia, parceiro/time cross-funcional, ou cliente. O mesmo fato muda de forma dependendo de quem lê.
3. **Reunir o contexto** — o que foi entregue, o que está bloqueado, decisão tomada, próximo passo. Se algo saiu misto ou pior que a meta, isso entra no update com o mesmo peso do que saiu bem.
4. **Gerar o conteúdo estruturado** por audiência (abaixo).
5. **Revisar tom e nível de detalhe** antes de enviar, e formatar para o canal (e-mail, mensagem, documento).

## Regra de proveniência dos números

Todo número no update carrega uma etiqueta: `medido` · `meta` · `estimativa` · `a confirmar`. É o ponto em que a etiqueta mais importa, porque o update é o documento que mais circula fora do time: um número `estimativa` que viaja sem etiqueta volta como cobrança de meta três meses depois.

## Estruturas por audiência

> Template pronto para preencher: [`templates/stakeholder-update-template.md`](../../templates/stakeholder-update-template.md)

- **Executivo** — abre com um resumo de uma frase e status (verde/amarelo/vermelho), progresso amarrado à meta, risco crítico que exige decisão, e a decisão específica que está sendo pedida. Cabe em poucas frases; se precisa de mais que isso, o problema é outro documento, não o update.
- **Engenharia** — o que foi entregue (com link), o que está em andamento e com quem, bloqueio atual, decisão técnica tomada, prioridade da próxima janela.
- **Parceiro/cross-funcional** — entregável que afeta o time deles, pedido específico com prazo, decisão que impacta o trabalho deles. Se o andamento depende de uma negociação externa em paralelo, isso aparece explicitamente, com status real da conversa — não "em andamento" genérico.
- **Cliente** — nova capacidade, prazo, alternativa temporária para problema conhecido, e como dar feedback. Linguagem acessível, sem jargão interno.
- **Anúncio de lançamento** — escopo, disponibilidade, métrica de sucesso definida antes do lançamento (não depois), estratégia de rollout.
- **Comunicação de migração** — quando há base legada envolvida: quem é afetado, o que muda, prazo de carência, o que acontece se nada for feito, e como reverter. A UX da transição precisa aparecer no update, não só no plano interno.
- **Resultado misto (quando existir)** — todas as métricas afetadas juntas, com o que isso muda na decisão seguinte.

## Erros comuns que evito

- Mostrar só a métrica que melhorou quando o resultado real foi misto.
- Pedir decisão sem dizer qual decisão específica é essa.
- Reportar dependência externa como "em andamento" sem status real da negociação.
- Comunicar migração só pelo destino, sem dizer o que acontece com quem está no legado durante a transição.
- Deixar número sem etiqueta de proveniência num documento que vai circular fora do time.
- Update de executivo que passa de poucas frases — se precisa de mais espaço, é outro documento.

## Follow-up

Depois do update, ofereço: versão para outro canal (e-mail vs. mensagem curta), uma segunda versão só com o que é urgente para quem só vai ler o título, ou o review de métricas por trás dos números citados (ver `metrics-review`).
