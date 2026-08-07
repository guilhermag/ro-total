# Ragnarok Online — Jornada de Lore

## Objetivo

Este repositório acompanha uma primeira experiência guiada pela lore de **Ragnarok Online**, usando o **RO LATAM** como plataforma principal de jogo e o **kRO/Gravity** como referência primária para continuidade narrativa e canon.

O objetivo não é otimizar PvP, WoE, economia ou endgame competitivo. O personagem existe principalmente como veículo para explorar o mundo, completar quests narrativas, visitar lugares importantes e acompanhar a história em uma ordem adequada para uma primeira experiência.

## Regra principal: não dar spoilers

Antes de responder qualquer pergunta de lore relacionada a este projeto:

1. Consultar `estado/PROGRESSO.md`.
2. Consultar `estado/CONHECIMENTO.md`.
3. Consultar `estado/MISTERIOS.md`.
4. Considerar como conhecidas apenas as informações liberadas até o último capítulo concluído.
5. Se a resposta depender de conteúdo futuro, dizer apenas que a questão será esclarecida adiante, sem antecipar a resposta.
6. Nunca usar conhecimento de capítulos futuros para reinterpretar explicitamente eventos passados antes da hora.

## Princípios do projeto

### 1. Ordem narrativa acima da ordem de patch

A jornada prioriza a melhor ordem para uma primeira experiência, não necessariamente a ordem exata em que cada conteúdo foi lançado.

Quando necessário, conteúdos retrospectivos como EDDA, memórias ou versões antigas de locais serão posicionados no ponto em que produzirem melhor compreensão sem estragar revelações futuras.

### 2. kRO define a espinha dorsal

A linha narrativa principal deve seguir o conteúdo oficial da Gravity/kRO sempre que possível.

O RO LATAM é a plataforma usada para vivenciar essa história, mas diferenças de implementação, tradução, disponibilidade ou ordem de conteúdo devem ser registradas sem redefinir o canon.

### 3. RO LATAM é a rota jogável

Cada capítulo deve verificar, no momento em que for preparado:

- se o conteúdo existe atualmente no RO LATAM;
- como a quest começa;
- requisitos de nível;
- pré-requisitos;
- NPCs relevantes;
- instâncias necessárias;
- itens obrigatórios;
- limitações práticas causadas por versão, bots, economia ou conteúdo em grupo.

Se uma parte histórica não estiver disponível no LATAM, ela deve ser reconstruída por fontes confiáveis e marcada como conteúdo histórico/indisponível.

### 4. Lore e mecânica são separadas

Grind não deve ser tratado como narrativa.

Cada capítulo pode marcar trechos como:

- `💬 Diálogo importante` — não pular.
- `👀 Preste atenção` — detalhe importante para o futuro, sem explicar o motivo.
- `🛠️ Trecho mecânico` — pode ser feito da forma mais rápida possível.
- `⭐ Side story recomendada` — conteúdo opcional com valor narrativo alto.
- `💤 Opcional` — pouco valor para a lore principal.
- `📜 Arquivo histórico` — conteúdo antigo removido/alterado no servidor atual.
- `⚠️ Diferença LATAM/kRO` — divergência relevante de versão ou tradução.

### 5. O guia deve acompanhar o conhecimento do jogador

Arquivos de personagens, facções, lugares e mistérios devem conter apenas informações já descobertas.

Não transformar esses arquivos em uma wiki completa do universo antes da hora.

## Fluxo de trabalho de cada capítulo

Quando o usuário pedir o próximo capítulo:

1. Ler o estado atual do projeto.
2. Identificar o capítulo seguinte em `INDICE.md`.
3. Pesquisar fontes atuais e confiáveis para a rota do RO LATAM.
4. Verificar divergências de versão.
5. Preparar o capítulo usando `templates/CAPITULO_TEMPLATE.md`.
6. Não registrar como concluído antes de o usuário confirmar que terminou.
7. Após a conclusão, atualizar:
   - `estado/PROGRESSO.md`;
   - `estado/CONHECIMENTO.md`;
   - `estado/MISTERIOS.md`;
   - `notas/PERSONAGENS.md`;
   - `notas/FACCOES.md`;
   - `notas/LUGARES.md`;
   - `estado/PERSONAGEM.md`, quando necessário.

## Hierarquia de fontes

Consultar `referencias/FONTES.md` para regras completas.

Resumo:

1. Gravity / kRO / GNJOY oficiais.
2. RO LATAM oficial.
3. iRO / WarpPortal oficial.
4. Wikis técnicas consolidadas.
5. Bancos de dados e arquivos comunitários.
6. Discussões da comunidade, apenas como apoio.

## Estrutura do repositório

```text
ragnarok-lore/
├── README.md
├── INDICE.md
├── CHANGELOG.md
├── estado/
│   ├── PROGRESSO.md
│   ├── PERSONAGEM.md
│   ├── CONHECIMENTO.md
│   └── MISTERIOS.md
├── capitulos/
├── notas/
│   ├── PERSONAGENS.md
│   ├── FACCOES.md
│   ├── LUGARES.md
│   └── GLOSSARIO.md
├── referencias/
│   ├── FONTES.md
│   └── DIVERGENCIAS.md
├── templates/
│   └── CAPITULO_TEMPLATE.md
└── assets/
```

## Convenções de nomes

Capítulos:

```text
000-introducao.md
001-criacao-do-mundo.md
002-coracao-de-ymir.md
...
```

Usar três dígitos para manter ordenação lexical correta.

## Git

O repositório pode ser versionado normalmente.

Sugestão de commits:

```text
chore: initialize lore project
chapter: add chapter 001 creation of the world
progress: complete chapter 001
lore: update known characters after chapter 023
sources: document LATAM/kRO divergence in Biolabs
```

## Critério de sucesso

A jornada está funcionando quando o jogador consegue responder:

- onde está na história;
- o que já descobriu;
- quais perguntas continuam sem resposta;
- o que precisa fazer no jogo em seguida;
- quais partes são canon confirmado e quais dependem de tradução/interpretação.

O objetivo final é terminar com um registro pessoal da descoberta de Rune-Midgard, e não apenas uma lista de quests concluídas.
