---
name: synthesize-research
description: Transforma pesquisa qualitativa e quantitativa bruta (entrevista, survey, ticket de suporte) em achados estruturados e acionáveis. Use depois de rodar entrevistas, workshop de dores ou survey, quando o material ainda está em bruto.
---

# Synthesize Research

## Quando usar

Depois de qualquer coleta de pesquisa — entrevista, workshop de dores, survey quantitativo, pesquisa dentro do produto — quando o material ainda são notas soltas, transcrição ou respostas brutas, e precisa virar decisão.

## O caso que molda esta skill

Conduzi pessoalmente escuta ativa com **dez clientes, num único dia**, para entender como um produto de crédito via investimento estava sendo percebido depois de evoluir de conceito. O achado que mais importou não foi estatístico — foi qualitativo: o termo que descrevia a evolução não aterrissava em ninguém, nem em quem já usava o produto base com fluência ("a cada tanto que boto, viro um tanto de crédito", resumiu um cliente). E o canal de comunicação estava tão fragmentado que parte da base achava que o benefício "tinha parado de funcionar" quando ele seguia ativo. Isso não aparece em nenhuma métrica de conversão. Só aparece porque alguém perguntou e ouviu de verdade.

A hipótese de entrada era que precisávamos vender melhor o benefício. Depois das dez conversas, o problema anterior a esse ficou visível: não dá para otimizar a mensagem de um produto que a base não sabe que existe.

**O contraponto quantitativo, do mesmo repertório:** uma pesquisa de PMF pela metodologia Sean Ellis, exibida direto na tela do benefício, para 5% da base elegível, com critério de pelo menos um acesso nos 15 dias anteriores. Régua definida antes: 40% de "muito desapontado(a)" é sinal de encaixe real. Deu 63%. Dez entrevistas e um survey de base respondem perguntas diferentes — e nenhum dos dois substitui o outro.

## Como eu trabalho

1. **Reunir o material bruto** — texto colado, arquivo, ou fonte conectada. Confirmo tipo de pesquisa, número de participantes, critério de elegibilidade da amostra, foco da investigação e o impacto de negócio que motivou a pesquisa, porque isso muda o que conta como achado relevante.
2. **Processar cada fonte** — extraio observação, citação direta, comportamento, dor, sinal positivo e contexto de cada entrevista ou resposta, antes de tentar agrupar qualquer coisa.
3. **Identificar temas** — codifico as observações, agrupo em temas, avalio frequência e severidade de impacto. Um achado dito por uma pessoa com muita convicção não pesa mais do que um achado dito por várias pessoas com menos ênfase — frequência e impacto são avaliados separado da intensidade de quem falou.
4. **Triangular quando possível.** Um achado qualitativo (entrevista) que bate com um achado quantitativo (survey, ticket de suporte) sustenta uma decisão de um jeito que nenhum dos dois sustenta isolado.
5. **Nomear o que a pesquisa não respondeu.** Toda síntese termina com o que ficou em aberto, inclusive quando o resultado principal foi bom — um número acima da régua responde "as pessoas querem", não "isso se sustenta".
6. **Gerar a síntese** (estrutura abaixo).

## Regra de proveniência dos números

Todo número na síntese carrega uma etiqueta: `medido` · `meta` · `estimativa` · `a confirmar`. Régua definida antes da coleta (o corte de 40%, por exemplo) é `meta`; resultado apurado é `medido`; extrapolação de amostra pequena para a base inteira é `estimativa` — e achado de entrevista qualitativa não vira percentual nunca, vira frequência declarada ("7 de 10 mencionaram").

## Estrutura da síntese

> Template pronto para preencher: [`templates/research-synthesis-template.md`](../../templates/research-synthesis-template.md)

- **Visão geral da pesquisa** — metodologia, perguntas de pesquisa, período, número de participantes e critério de elegibilidade da amostra.
- **Principais achados** (5-8) — cada um com: enunciado do achado, evidência (citação ou dado), frequência, impacto, nível de confiança.
- **Segmentos de usuário** — agrupamentos comportamentais distintos que emergiram, com características e necessidades próprias.
- **Áreas de oportunidade** — necessidade não atendida ou lacuna de capacidade que a pesquisa revelou.
- **Recomendações** — ação específica ligada a um achado nomeado, nunca uma recomendação genérica desconectada da evidência.
- **Perguntas abertas** — o que a pesquisa não respondeu e precisa de investigação futura.

## Erros comuns que evito

- Deixar um achado qualitativo forte (dito com muita convicção por uma pessoa) pesar mais do que um achado com maior frequência real.
- Transformar amostra qualitativa pequena em percentual, como se dez entrevistas fossem um survey.
- Misturar achado com recomendação sem deixar a evidência visível entre os dois.
- Ignorar o canal/comunicação como fonte de atrito — problema de produto às vezes é problema de as pessoas não entenderem que o produto já resolveu aquilo.
- Sintetizar só a fonte quantitativa e tratar entrevista como anexo decorativo, ou o inverso.
- Fechar a síntese sem dizer o que a pesquisa não respondeu.

## Follow-up

Depois da síntese, ofereço: refinar um achado específico, gerar persona a partir dos segmentos identificados, propor a próxima rodada de pesquisa para as perguntas que ficaram abertas, estressar os achados numa sessão de exploração (ver `product-brainstorming`) ou já transformar a recomendação priorizada em spec (ver `write-spec`).
