# PM OS

Um conjunto de skills de IA + templates que uso no meu dia a dia como Product Manager em fintech (Neon, PicPay). Não é uma lista genérica de "boas práticas de produto" — são as ferramentas que eu mesmo construí, testei e uso de fato, adaptadas para que qualquer PM possa baixar o repositório e rodar com o próprio LLM.

Cada skill carrega um pouco do meu processo real: como eu meço resultado (e admito quando ele é misto), como eu decido roadmap sem ter histórico de dados, como eu negocio escopo com parceiro externo, como eu conduzo entrevista de descoberta. A ideia não é te dar um framework abstrato — é te dar o framework com a cicatriz de quem já usou.

Mais contexto sobre os casos que embasam essas skills está no meu portfólio (seção Personal Projects → PM Toolkit).

## O que tem aqui

```
pm-os/
├── .claude-plugin/
│   └── plugin.json
├── skills/
│   ├── write-spec/                  # escrever PRD/spec com escopo defensável
│   ├── roadmap-update/              # atualizar e repriorizar roadmap sob incerteza
│   ├── design-experiment/           # desenhar a medição antes de ligar o experimento
│   ├── metrics-review/              # revisão de métricas com proveniência clara do número
│   ├── pricing-unit-economics/      # se o benefício se sustenta financeiramente
│   ├── competitive-brief/           # benchmark competitivo estruturado
│   ├── synthesize-research/         # sintetizar pesquisa qualitativa em achados acionáveis
│   ├── manage-external-dependency/  # dependência de parceiro como escopo, não como risco
│   ├── stakeholder-update/          # comunicação de status por audiência
│   ├── sprint-planning/             # planejamento de sprint com capacidade realista
│   └── product-brainstorming/       # parceiro de pensamento pra explorar problema/solução
└── templates/                       # um template de preenchimento por skill
```

Cada pasta em `skills/` tem um `SKILL.md`: instruções que ensinam um LLM a executar aquele tipo de trabalho do jeito que eu executo.

**`templates/` tem um template por skill** (PRD, roadmap, plano de sprint, desenho de experimento etc.), todos no mesmo formato de preenchimento: `[placeholder]`, instrução curta em itálico e a etiqueta de proveniência já visível onde ela importa. Usar não é obrigatório — cada skill carrega a estrutura do entregável dentro do próprio `SKILL.md`, e o template só evita reescrever o esqueleto do zero. O índice de qual template serve qual skill está em [`templates/README.md`](templates/README.md).

## Como usar

**Claude Code ou Cowork (plugin):**
Clone o repositório e instale a pasta como plugin local, ou copie a pasta `skills/` inteira para dentro de `.claude/skills/` do seu projeto. Cada skill é reconhecida automaticamente pelo nome e pela descrição no frontmatter do `SKILL.md`.

**Claude.ai (skills de conta/projeto):**
Se sua conta tiver skills customizadas habilitadas, suba o `SKILL.md` da skill que quiser usar diretamente nas configurações de skills.

**Qualquer outro LLM:**
Abra o `SKILL.md` da skill desejada e cole o conteúdo como instrução de sistema (ou no início da conversa) antes de pedir o trabalho. O conteúdo foi escrito para ser autossuficiente — não depende de nenhuma ferramenta específica da Anthropic.

## Inspiração e diferença em relação ao original

A estrutura de pastas (`skills/<nome>/SKILL.md`) segue a convenção do repositório open-source [`anthropics/knowledge-work-plugins`](https://github.com/anthropics/knowledge-work-plugins), especificamente o plugin de Product Management. Usei aquele repositório como referência de formato — mas o conteúdo de cada skill aqui foi reescrito a partir do meu próprio processo de trabalho, não é uma cópia.

## Licença

MIT — usa, adapta, redistribui. Se usar como base, um crédito é sempre bem-vindo, mas não é obrigatório.
