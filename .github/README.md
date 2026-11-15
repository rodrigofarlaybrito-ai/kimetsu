# Kimetsu Mod (Forge 1.20.1)

Mod feito por fã, inspirado em Kimetsu no Yaiba. Requer Minecraft 1.20.1 e Forge 47.x.

## Como gerar o .jar (sem instalar nada)

1. Crie um repositório no GitHub e envie todo o conteúdo desta pasta (inclusive a pasta `.github`).
2. Abra a aba **Actions**, escolha o workflow **Build mod** e aguarde uns 3 a 5 minutos.
3. Entre na execução concluída e baixe o artefato **kimetsumod-jar**. Dentro dele está o `.jar`.
4. Coloque o `.jar` na pasta `mods` do Minecraft com Forge 1.20.1.

Para compilar localmente: JDK 17 + Gradle 8.1.1, e rode `gradle build`. O jar sai em `build/libs/`.

## O que o mod tem

- **14 espadas Nichirin**, uma por respiração: Água, Chamas, Trovão, Vento, Pedra, Névoa, Amor, Serpente, Som, Inseto, Flor, Sol, Lua e Fera.
- **5 formas por respiração** (70 no total). Cada forma é de um tipo: corte em linha, giro em área, avanço, salto ou buff.
- **Sistema de fôlego**: usar uma forma gasta fôlego (0 a 100), que recupera sozinho. A barra aparece na action bar.
- **Oni**: regenera rápido, queima no sol, recebe só 40% do dano de armas comuns, e a Nichirin causa 1,5x de dano, bloqueia a regeneração e decapita com pouca vida. Cada oni nasce com uma Arte Demoníaca de Sangue (veneno, lentidão, confusão ou fogo).
- **Hashira**: aliado com Nichirin aleatória que ataca oni. Nasce por ovo de spawn.
- **Roupas (v2)**:
  - **Uniforme de Caçador** (quepe, uniforme, calça, botas). Set completo: Velocidade I.
  - **Haori de Hashira**, um para cada respiração (14 cores). Vai no lugar do peitoral. Haori + resto do uniforme: Força I e Velocidade II.
  - **Roupa de Oni** (chifres, manto, calça, botas). Set completo: Força I e Visão Noturna, mas Fraqueza sob o sol.
  - Oni e hashiras também usam essas roupas: hashiras nascem de uniforme + haori da própria respiração, e metade dos oni nasce com a roupa de oni (8% de chance de dropar cada peça).
- **Rei dos Oni (chefe)**: 400 de vida, barra de chefe, tentáculos em área, invoca oni, e entra em fase 2 abaixo de 50% de vida (mais rápido, regenera mais e bate mais forte). Só a Nichirin impede a regeneração e causa dano cheio. Nasce só pelo ovo de spawn. É um personagem original inspirado no vilão da obra, renomeie em `lang` se quiser.
- **Conquistas**: 11 avanços em árvore (de Areia Escarlate até Mestre das Respirações, Uniforme Completo, Posto de Hashira, Disfarce Demoníaco e Fim da Noite Eterna).
- Receitas das roupas: uniforme = lã preta no formato de armadura; haori = peitoral do uniforme + corante da respiração + lã branca (sem forma); roupa de oni = lã preta + Sangue de Oni.
- Receitas: Areia de Ferro Escarlate (areia + redstone + pepita de ferro, rende 2), fundida em barra. Cada espada leva 2 barras de ferro escarlate, 1 graveto e 1 corante da cor da respiração (veja `data/kimetsumod/recipes`).
- Textos em português (BR) e inglês.

## Como usar

- **Botão direito** com a espada: usa a forma selecionada.
- **Shift + botão direito**: troca de forma.

## Otimização

Texturas de 16x16 (itens) e 64x64 (mobs), modelos vanilla reaproveitados, sem blocos entity, sem scans por tick (o fôlego atualiza 2x por segundo) e partículas em quantidade limitada.

## Ainda não incluído

Luas Superiores e Inferiores, personagens individuais, construções (estruturas em NBT), mais artes demoníacas e nomes oficiais das formas de Amor, Som, Inseto, Flor, Sol, Lua e Fera (hoje aparecem como "Forma N" e podem ser editados em `assets/kimetsumod/lang`).
