# CSS Tutorial

### Propriedades do Container Flexbox
A primeira coisa que precisamos fazer é definir um contêiner como um item flexível, para isto basta adicionar a propriedade **display: flex.**

### flex-direction
Ajuda a definir a direção dos **flex-itens** dentro do **contêiner.**

Por padrão, o valor desta propriedade é **row**, o que faz alinhar em linha os elementos, mas temos outros valores possíveis nesta propriedade:

* **column:** os itens ficam em uma única coluna, de cima para baixo.
* **column-reverse**: os itens ficam em uma única coluna, mas baixo para cima.
* **row-reverse:** organiza da direita para esquerda
* **row:** organiza da esquerda para direita

### flex-wrap
Ajuda a definir se um container deve quebrar os itens flexíveis em uma nova linha.

Por padrão, todos os elementos vão ocupar uma única linha, utilizando a largura disponível do contêiner, em alguns casos, pode ser necessário quebrar os elementos em uma nova linha para distribuir melhor os elementos e para isso, temos alguns valores:

* **wrap**: quebra os itens para uma nova linha, de cima para baixo.
* **no-wrap**: todos os itens serão mantidos na mesma linha, não haverá quebra.
* **wrap-reverse:** quebra os itens para uma nova linha, mas de baixo para cima.

### flex-flow
Ajuda a definir os valores de **flex-direction** e **flex-wrap** em uma única propriedade.

Esta propriedade é só um atalho, você pode definir as propriedades separadas, mas caso ache útil, pode combinar os valores, primeiro o valor de **flex-direction**, depois **flex-wrap**.

### justify-content

Ajuda a definir o alinhamento dos itens flex dentro do container em relação **flex-direction.**

Está propriedade é útil para distribuir itens quando temos espaço sobrando, ou precisamos definir que os itens fiquem alinhados no inicio e no fim do container, no centro ou que tenham um espaço entre eles.

Os principais valores desta propriedade são:

* **flex-start**: Os itens são agrupados no início.
* **flex-end**: Os itens são agrupados no final.
* **center**: Os itens são centralizados.
* **space-between**: Adiciona um espaçamento igual entre os itens e posiciona o primeiro elemento no inicio da linha e o último no final, grudados na borda do container.
* **space-around**: Também adiciona um espaçamento entre os itens, mas elementos que ficam ao centro, recebem o dobro do espaçamento.

### align-items
Ajuda a definir o alinhamento dos itens em relação ao eixo cruzado do container.

Está propriedade é muito utilizada para alinhar **verticalmente** um item **flex**. 

Os principais valores desta propriedade são:

* **flex-start**: Os itens são alinhados no inicio.
* **flex-end**: Os itens são alinhados no fim.
* **center**: Os itens são alinhados ao centro.
* **stretch**: Os itens são esticados de forma igual, preenchendo o container.
* **baseline**: Os itens são alinhados seguindo a linha base do seu texto.

### align-content
Ajuda a definir o alinhamento das linhas de um container.

Ao aplicar está propriedade, o container precisa ter um tamanho maior que a altura das linhas para que o efeito seja percebido.

* **normal**: As linhas não recebem nenhum tipo de alinhamento, é o valor padrão.
* **flex-start**: As linhas são posicionadas no inicio.
* **flex-end**: As linhas são posicionados no fim.
* **stretch**: As linhas são distribuídas de
* **center**: As linhas são posicionadas ao centro.
* **space-between**: As linhas são distribuídas com um espaçamento igual. A primeira linha fica posicionada no inicio do container (top) e a última no fim (bottom).
* **space-around**: As linhas também ganham um espaçamento igual ao space-between, mas é adicionado um espaçamento dobrado entre os itens.

### gap, row-gap e column-gap
Ajuda a definir e controlar o tamanho exato de espaçamento entre os itens **Flex**.

Um aviso relevante, estas propriedades também funcionam em layouts com **CSS Grid**.

Vamos aos valores desta propriedade:

* **gap**: Personaliza o espaçamento para linhas e colunas de um elemento.
* **row-gap**: Personaliza o espaçamento apenas para linhas.
* **column-gap**: Personaliza o espaçamento apenas para colunas.

### Propriedades do Flex Item

Os Flex Items são elementos os filhos de um elemento Flex.

### order
Ajuda a definir a ordem que os elementos aparecem na tela, sempre do menor para o maior.

Por padrão, a ordem dos elementos é a ordem que os elementos foram criados no HTML.
ex: **order: 2**;

### flex-grow
Ajuda a definir se um Flex Item pode expandir se necessário.

Por padrão um Flex Item tem o **valor 0** definido nesta propriedade, mas você pode atribuir um valor numérico para representar uma proporção.

Por exemplo, um item que tem **flex-grow** igual a **2** e outro **flex-grow 1**, vai expandir e ocupar o dobro de espaço do outro item, está regra também pode ser usada para mais itens.
ex: **flex-grow: 2**;

### flex-shrink
Ajuda a definir se um item flexbox deve encolher dentro de um container se necessário.

Por padrão, o valor desta propriedade é **0**.
ex: **flex-shrink: 3**;

### flex-basis
Ajuda a definir o tamanho inicial de um Flex Item antes do espaço sobrando for distribuído.

Por padrão, esta propriedade tem o valor auto, isto indica que o elemento vai ocupar o espaço necessário para seu conteúdo, mas você pode definir um tamanho fixo.
ex: **flex-basis: 100px**;

### align-self
Ajuda a definir o alinhamento especifico de um único item dentro do container.

Por padrão, está propriedade tem o valor auto, os valores possíveis são iguais ao align-items.

* **flex-start**: O item é alinhado no inicio.
* **flex-end**: O item é alinhado no fim.
* **center**: O item é alinhado ao centro.
* **stretch**: O item é esticado, preenchendo todo o container.
* **baseline**: O item é alinhado seguindo a linha base do seu texto.

### flex
Ajuda a definir os valores de flex-grow, flex-shrink e flex-basis em uma única propriedade.

Por padrão, o valor desta propriedade é none, mas você pode definir da seguinte forma:
ex: **flex: 2 3 100px**;
ex: **flex: 1**;

### Seletor:
* **:active** a:active Seleciona o link ativo
* **::after** p::after Insere algo após o conteúdo de cada elemento 
* **::before** p::before Insere algo antes do conteúdo de cada elemento 
* **:checked** input:checked Seleciona cada elemento <input> marcado
* **:default** input:default Seleciona o elemento padrão <input>
* **:disabled** input:disabled Seleciona cada elemento <input> desabilitado
* **:empty** p:empty Seleciona cada elemento que não tem filhos (incluindo nós de texto)
* **:enabled** input:enabled Seleciona cada elemento <input> habilitado
* **:first-child** p:first-child Seleciona cada elemento que é o primeiro filho de seu pai
* **::first-letter** p::first-letter Seleciona a primeira letra de cada elemento 
* **::first-line** p::first-line Seleciona a primeira linha de cada elemento 
* **:first-of-type** p:first-of-type Seleciona cada elemento que é o primeiro elemento  de seu pai
* **:focus** input:focus Seleciona o elemento de entrada que tem foco
* **:fullscreen** :fullscreen Seleciona o elemento que está no modo de tela cheia
* **:hover** a:hover Seleciona links ao passar o mouse
* **:in-range** input:in-range Seleciona elementos de entrada com um valor dentro de um intervalo especificado
* **:indeterminate** input:indeterminate Seleciona elementos de entrada que estão em um estado indeterminado
* **:invalid** input:invalid Seleciona todos os elementos de entrada com um valor inválido
* **:lang(language)** p:lang(it) Seleciona cada elemento com um atributo lang igual a "it" (italiano)
* **:last-child** p:last-child Seleciona cada elemento que é o último filho de seu pai
* **:last-of-type** p:last-of-type Seleciona cada elemento que é o último elemento de seu pai
* **:link** a:link Seleciona todos os links não visitados
* **::marker** ::marker Seleciona os marcadores dos itens da lista
* **:not(selector**) :not(p) Seleciona todo elemento que não é um elemento
* **:nth-child(n)** p:nth-child(2) Seleciona cada elemento que é o segundo filho de seu pai
* **:nth-last-child(n)** p:nth-last-child(2) Seleciona cada elemento que é o segundo filho de seu pai, contando a partir do último filho
* **:nth-last-of-type(n)** p:nth-last-of-type(2) Seleciona cada elemento que é o segundo elemento de seu pai, contando a partir do último filho
* **:nth-of-type(n)** p:nth-of-type(2) Seleciona cada elemento que é o segundo elemento de seu pai
* **:only-of-type** p:only-of-type Seleciona cada elemento que é o único elemento de seu pai
* **:only-child** p:only-child Seleciona cada elemento que é o único filho de seu pai
* **:opcional** input:opcional Seleciona elementos de entrada sem atributo "obrigatório"
* **:out-of-range** input:out-of-range Seleciona elementos de entrada com um valor fora de um intervalo especificado
* **::placeholder** input::placeholder Seleciona elementos de entrada com o atributo "placeholder" especificado
* **:read-only** input:read-only Seleciona elementos de entrada com o atributo "readonly" especificado
* **:read-write** input:read-write Seleciona elementos de entrada com o atributo "readonly" NÃO especificado
* **:required** input:required Seleciona elementos de entrada com o atributo "required" especificado
* **:root** :root Seleciona o elemento raiz do documento
* **::selection** ::selection Seleciona a parte de um elemento que é selecionado por um usuário
* **:target** #news:target Seleciona o elemento #news ativo atual (clicado em um URL contendo esse nome de âncora)
* **:valid** input:valid Seleciona todos os elementos de entrada com um valor válido
* **:visited** a:visited Seleciona todos os links visitados
