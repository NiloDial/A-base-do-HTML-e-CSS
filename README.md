# A Base do HTML e CSS

# HTML

A sigla HTML significa *Hypertext Markup Language*, o HTML é uma ferramenta web que utilizamos para inserir conteúdos dentro de um site, o HTML não é um linguagem de programação, mas utilizamos ele junto com uma linguagem, o JavaScript, por exemplo. Para adicionar conteúdos corretamente dentro de sites usando as tags do HTML, existe uma tag para cada tipo de conteúdo, título `<h1>`, parágrafo `<p>`, imagens `<img>` e muito mais.

### COMENTÁRIOS

O uso de comentários é muito útil para documentar e explicar algumas partes do seu HTML, para qualquer pessoa que acesse o arquivo consiga identificar tudo que está acontecendo dentro dele, até para você mesmo conseguir identificar partes especificas do arquivo, ajuda bastante principalmente quando o arquivo tem bastante conteúdo, uma páginas com mais de 3 sessões já acumula bastante HTML. Para conseguir comentar dentro do HTML sem prejudicar o seu código usamos:

`<!— —>`

`<!— Comentário —>` 

### TAG

Utilizamos tags para conseguir adicionar diferentes tipos de conteúdos dentro do HTML, as diferentes tags servem para identificar os diferentes conteúdos que podemos adicionar na estrutura dos sites, essa identificação serve para nossa interpretação na hora de construir o site e principalmente para a interpretação dos “navegadores” que vão reproduzir nosso site, eles precisam interpretar a variedade de conteúdo que adicionamos no site, outra informação importante é que as tags tem uma anatomia:

- Abertura da tag | `<h1>`
- Fechamento da tag | `</h1>`

- Conteúdo | `Olá mundo!`

- Elementos | `<h1>Olá mundo!</h1>`

- Atributos | `id = “titulo01”`

- Elemento com Atributo | `<h1 id = “Título01”>Olá mundo!</h1>`

Críamos um elemento `h1` (Título) com um conteúdo dentro `Olá mundo!` com um atributo de identificação `id` , nem todo elemento precisa ter atributo, da mesma forma que também podemos fazer um elemento sem conteúdo, geralmente fazemos elementos sem conteúdos para adicionar eles posteriormente usando JavaScript.

### TAGS SEM CONTEÚDO

Também existe tags que não tem conteúdo, somente atributos, tags fechadas nela mesma, como a tag img `<img src=” ” alt=” ”/>` conseguimos configurar essa tag apenas usando os atributos, outro exemplo é a tag `<br/>` que usamos para quebrar linhas. 

### FLUXO DO HTML

O fluxo do HTML em sua grande maioria é baseado em blocos, blocos de conteúdo, ele por padrão adiciona uma tag em baixo da outra, formando `blocks` de conteúdo, mas também existem as tags `inline` que ocupam apenas o espaço do conteúdo, nesses casos se adicionar duas tags `inline` como a tag `<a>` o HTML vai deixar uma ao lado da outra, mas se adicionar duas tags do tipo `block` como uma `<div>` o HTML vai adicionar uma em baixo da outra, que é o padrão.

### ANINHAMENTO DE TAGS

Aninhamento de tags é usar uma tag dentro da outra, por exemplo, podemos fazer um parágrafo `<p>` e dentro dele colocar uma palavra em negrito, usando a tag `<strong>`, ficaria assim:

`<p>`

Lorem Ipsum is simply dummy text of the printing and typesetting industry. `<strong>`**Lorem**`</strong>` Ipsum has been the industry's standard dummy text ever since the 1500s.

`</p>`

### ATRIBUTOS HTML

Como já expliquei anteriormente atributos são informações extras que passamos dentro de uma tag, pode ser atributos de configuração/conteúdo, como o exemplo do atributo `<img src=” ” />` que recebe o link de uma imagem por exemplo, e essa imagem vai ser exibida dentro da tag `<img>` , outro exemplo é o atributo de identificação `id = “ ”` que coloca um id dentro da tag, esse id pode ser usado para localizar a tag em outra parte do nosso código. A quantidade de atributos disponíveis para o HTML é gigante, recomendo olhar a documentação, mas naturalmente vamos aprendendos as principais conforme o uso no dia a dia.  [Site com os atributos globais.](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Global_attributes)

### ELEMENTOS DE CONTEÚDO

### SEMÂNTICA

O HTML tem uma semântica, é importante que você respeite ela, tanto para um melhor aproveitamento da ferramenta, quanto para questões externas, como o SEO, um site bem organizado e seguindo a semântica correta tem um ranqueamento melhor nos motores de busca. Então use a tag `<h1>` para título, `<p>` em parágrafos, `<button>` em botões… Existe uma tag para cada elemento base de um site. 

### FORMATAÇÃO BÁSICA DE TEXTO

`<strong>` **Negrito**

`<em>` *Itálico*

`<mark>` Grifado

`<s>` ~~Riscado~~

### LISTAS

Conseguimos montar listas dentro do HTML, podemos montar lista ordenada e não ordenada, exemplo:

`<ul>` NÃO ORDENADA

`<li> Lista 01 </li>`

`<li> Lista 02 </li>`

`<li> Lista 03 </li>`

`</ul>` 

`<Ol>` ORDENADA

`<li> Lista 01 </li>`

`<li> Lista 02 </li>`

`<li> Lista 03 </li>`

`</Ol>` 

### ELEMENTOS ESTRUTURAIS

Usamos uma estrutura padrão dentro do arquivo `.html`, precisamos seguir a estrutura para que o código funcione corretamente e os motores de busca identifiquem os dados do site corretamente. 

`<html>`

`<head>` Configurações da página

`<meta charset=”utf-8”>`

`<title> Estrutura HTML </title>`

`</head>`

`<body>` Corpo da página, onde o conteúdo é inserido

`<h1> Estrutura HTML </h1>`

`<p> Um arquivo HTML precisa seguir uma estrutura padrão. </p>`

`</body>`

`</html>`

### MAIS TAGS ESTRUTURAIS

`<header>` Cabeçalho do site

`<main>` Conteúdo principal

`<aside>` Conteúdo secundário

`<footer>` Rodapé do site

`<nav>` Navegação, links

`<section>` Sessões da página

`<article>` Construção de artigo

`<div>` Caixa/grupo de conteúdo - Block

`<span>` Caixa/grupo de conteúdo - Inline

> Confira o exercício 01 em > Base do HTML > ex01

Nesse exercício usamos os elementos básicos do HTML para montar uma estrutura simples, como não usamos CSS nesse exercício o conteúdo não tem nenhuma estilização.
> 

---

# CSS

CSS significa Cascading Stylesheet, um arquivos de estilo que aplica estilos em cascata, é com o CSS que conseguimos estilizar o arquivo HTML. A quantidade de propriedade disponíveis no CSS é gigantesca, assim como no HTML, não da para simplesmente decorar tudo, por isso sempre precisamos acessar a documentação para aprender novas coisas. [Documentação](https://devdocs.io/css)

### COMENTÁRIO

Para conseguir deixar comentários dentro do seu código CSS sem quebrar nenhuma linha de estilização, usamos:

`/* */`

`/* Comentário */` 

### ANATOMIA

Para escrever uma estilização para um elemento precisamos montar o código usando um padrão de anatomia para o CSS.

O conjunto do estilo, chamamos de declaração, e ele começa com o Seletor, abrimos as `{ }`, e dentro delas colocamos as propriedades, com os seus respectivos valores.

`h1 {` Seletor

`color: red;` Propriedade com valor

`font-size: 60px` Propriedade com valor

`}` 

### SELETORES

Basicamente os seletores são os elementos do HTML que nós referenciamos dentro do CSS para aplicar os estilos, e para fazer isso usamos as tags do HTML, mas também conseguimos usar o atributos das tags, como o atributo id dentro de uma tag HTML. Alguns exemplos de seletores que pegamos dentro do HTML:

`<p>` | Tipo/Elemento/Tag

`id = ” txt1 ”` | id

`class = ” txt-branco ”` | Classe

`Title = ” t-base ”` | Qualquer atributo dentro do elemento

`*` | Universal 

Para referenciar esses seletores dentro do arquivo CSS:

`p { }` | Colocamos apenas o tipo

`#txt1 { }` | Usamos o “#” no id

`.txt-branco { }` | Usamos o “.” na classe

`[title ou title=”t-base”] { }` | Usamos as [ ] e o atributo dentro

`* { }` | Colocamos apenas o tipo “*”

### CASCATA

Dentro da cascata vale lembrar que o estilo que o CSS vai considerar, vai ser sempre o último aplicado, logo se você criar dois seletores `<p>` e aplicar uma cor X no primeiro e uma cor Y no segundo, o CSS vai puxar a cor do segundo, que no caso, foi o ultimo estilo adicionado para esse seletor. E vale lembrar que o efeito cascata vai aplicar essa mesma cor em todos os elementos HTML `<p>`.

### ESPECIFICIDADE

Conseguimos fugir do exemplo anterior com a especificidade, usando o conceito de peso dos seletores, um elemento `<p>` tem um peso 1, já um seletor `.class` tem um peso 10 e por fim, o seletor `#id`, tem um peso 100. Nesse caso o CSS não vai considerar o último estilo aplicado, ele vai considerar qual seletor tem o maior peso, mesmo que um elemento `<p>`, com um estilo de cor foi o último aplicado no arquivo CSS, mas esse mesmo elemento esta sendo novamente referenciado no CSS com um seletor `#id`, o CSS vai considerar a cor do seletor `#id`, porque tem o peso maior. 

E para conseguir um peso ainda maior, conseguimos combinar os seletores, exemplo, criamos um elemento `<p>` no HTML, e adicionamos uma classe e um id, podemos dentro do CSS usar o seletor `p #text .text { }`, nesse caso aumentamos a especificidade, e vai ser o elemento com maior peso na cascata.

Conseguimos ir mais longe na especificidade usando o atributo `style = ” “` diretamente no elemento do HTML, exemplo `<P style=”color: red;”> </p>` , mas isso não é recomendado, porque o estilo vai ficar fixo no elemento, e podemos acabar esquecendo que fizemos isso no HTML, na hora de estilizar dentro do CSS vamos ter problema com esse elemento especifico, poque ele vai ficar travado com a estilização que fizemos diretamente no HTML.

### BOX MODEL

O conceito de Box Model do CSS trata todos os elementos HTML como caixas, com conteúdo, largura, altura, bordas, preenchimentos e margens. Entender o Box Model é fundamental para o design de páginas web.

### ATRIBUTOS BASE

Como eu falei no início do bloco de conteúdo sobre CSS, a quantidade de atributos disponíveis para a estilização de uma página web é gigantesca, não da para decorar todos os atributos disponíveis, mas algum deles sempre usamos, então separei algum baseado no exercício 02 para não sair da nossa cabeça:

Estrutura

`width` | Define largura do elemento.

`height`| Define altura do elemento.

`margin` | Espaçamento dos 4 lados de um elemento.

`margin-top` | Espaçamento superior de um elemento para outro.

`margin-bottom` | Espaçamento inferior de um elemento para outro.

`padding` | Preenchimento interno dos 4 lados de um elemento para outro.

`box-sizing` | Define como a largura e a altura totais de um elemento são calculadas.

`border-radius` | Aplica um arredondamento nas bordas do elemento.

`vertical-aling` | Define o alinhamento vertical de uma caixa.

`div:nth-child(2)` | Editar um elemento filho especifico, nesse caso esta pegando uma div, que é o segundo (2) filho do elemento pai. 

Fonte

`font-family` | Define a fonte utilizada

`line-height` | Altera o espaçamento entre as linhas de um texto

`text-aling` | Alinha o texto horizontalmente

`font-size` | Define o tamanho da fonte

Cor

`color` | Adiciona cor nas fontes.

`background-image` | Adiciona uma imagem como fundo.

`background-size` | Define o tamanho da imagem de fundo do elemento.

`background-color` | Adiciona uma cor de fundo.

![ex2.png](https://i.ibb.co/wzDngrb/img-1.png)

> Confira o exercício 02 em Base do CSS > ex02.

No exercício 02 usamos os conceitos básicos do CSS para construir nossa primeira página estilizada, fizemos uma página de receitas, usamos a hierarquia de textos dentro do HTML, criamos uma lista, manipulamos imagem e criamos um background para o fundo da página usando uma imagem.
> 

### LAYOUT POSITION

Position no CSS, serve para posicionar elementos no layout. As propriedades do Position são: Relative, Absolute, Fixed e Sticky, por padrão o position dos elementos é static.

Conseguimos mover os elementos para o topo, baixo, esquerda e direita, também conseguimos alterar a altura do elemento com o `z-index`, um elemento com `z-index: 1`, fica por cima de outros com `z-index: 0`. Quanto maior o número mais “Alto” o elemento.

`Relative` - Conseguimos mover o elemento a partir da posição original dele.

`Absolute` - O elemento “flutua” por toda área visível do site, se ele estiver dentro de uma caixa com position relative, ele vai se conter a flutuar somente dentro dessa caixa, geralmente sempre usamos absolute com o relative no seu elemento pai, ou seja, um elemento absoluto vai ser relativo ao pai dele.

`Fixed` - O elemento fica fixo na tela, em relação a toda área visível do site. Usamos ele para fazer um botão de WhatsApp fixo no canto do site por exemplo.

`Sticky` - O elemento fica fixo, mas quando o pai tem scroll ele fica relativo ao pai e faz o scroll junto.

### VARIÁVEIS

Assim como no JS, usamos variáveis para armazenar informações dentro do CSS, exemplo, criamos a variável da seguinte maneira:

Variável de cor.

`—bg-base: blue` 

E usamos essa variável assim:

`P {`

`Background-color: var(—bg-base)`

`}` 

![ex3.png](https://i.ibb.co/6rnSkFk/img-2.png)

> Confira o exercício 03 em Base do CSS > ex03

Usamos os mesmos conceitos do exercício 02 pra criar esta página, nesse exemplo usamos mais manipulação de imagens, alinhamento e estilização de elementos filhos como os itens de uma lista.
> 

### PSEUDO-CLASSES E PSEUDO-ELEMENTS

Uma Pseudo-classes CSS é uma palavra-chave adicionada aos seletores que especificam um estado especial do elemento selecionado. Por exemplo, `:hover` pode ser usado para alterar o cor de um botão quando o usuário passa o cursor sobre ele.

Um pseudo-elements CSS é uma palavra-chave adicionada a um seletor que permite que você estilize uma parte específica do elemento selecionado. Por exemplo, o pseudo-elements `::first-line` aplica o estilo apenas na primeira linha de um parágrafo.

### FLEXBOX

Usamos o Flexbox para conseguir manipular mais facilmente os elementos, por padrão o HTML coloca os elementos em blocos, um em baixo do outro, com o Flexbox conseguimos manipular mais facilmente esses  elementos do tipo `block`, transformando em `Inline` , adicionar espaçamento entre os elementos e muito mais…

![ex4.png](https://i.ibb.co/yFYHZg5/img-3.png)

> Confira o exercício 04 em FlexBox e Grid > ex04 

A base desse exercício foi o uso do FlexBox para conseguir organizar os elementos um ao lado do outro e conseguir criar a galeria de fotos.
> 

### GRID

 O Grid funciona de forma parecida com o FlexBox, mas com foco em colunas e linhas. O Grid é composto de 2 principais grupos, o container (pai) e os itens (filhos), ele funciona como se fosse uma tabela.

![ex5.png](https://i.ibb.co/4Rz5G8G/img-4.png)

> Confira o exercício 05 em FlexBox e Grid > ex05.

O foco desse exercício foi usar o Grid para a construção do site de noticias, toda organização de layout foi feita usando o Grid.
> 

### FLEXBOX OU GRID

Não tem uma ferramenta melhor que a outra, as duas ferramentas servem para manipular e organizar elementos em mais de uma direção na sua página, vai ter casos onde o Grid funciona melhor e outros casos onde o FlexBox funciona melhor, tudo vai depender da facilidade de aplicação dentro de determinada situação no design da página, na maioria das vezes vamos acabar usando os dois na mesma página… Existem muitos atributos para o FlexBox e Grid, então é recomendado analisar os exercícios para ver cada atributo e sua funcionalidades, no exercício 06 por exemplo, usei FlexBox para fazer as tags de tecnologias na sessão “home” e usei Grid para montar os cards da sessão “Meu trabalho”…

![ex6.png](https://i.ibb.co/HzzB3GF/img-5.png)

> Confira o exercício 06 em FlexBox e Grid > ex06.

A ideia aqui é mostrar que podemos unir o uso do FlexBox com o Grid, mesmo que eles tenham funções parecidas dentro do CSS, no dia a dia vamos acabar usando as duas ferramentas, em conjunto, é normal acabar usando as duas ferramentas até mesmo dentro de uma única sessão.
> 

---

# FORMULÁRIOS

Formulários como você já deve saber, se trata de campos onde deixamos nossos dados, colocamos e-mail, senhas, mensagens, números de telefone e muito mais, praticamente toda estrutura web tem pelo menos um input (Elemento de formulário) no meio da sua estrutura, qualquer site com um sistema de login tem vários inputs. Basicamente usamos os formulários para transportar dados que o usuário colocou no sistema, podemos usar esses dados dentro da própria aplicação, ou enviar eles para outro lugar da internet, vamos entender mais como os formulários funcionam no HTML.

### BOTÃO

Com o botão conseguimos fazer muitas coisas no ambiente web, o botão por padrão tem a função de enviar dados, automaticamente ele vem com o type `submit` , mas conseguimos alterar isso, por exemplo, usando o tipo `reset` para limpar o campo preenchido.

### ATRIBUTOS BOTÃO

Conseguimos aplicar atributos nos botões como o atributo `autofocus` que já vai deixar o botão selecionado quando a página carregar, `disabled` deixa o botão desativado, `nome = " "`  para colocar um nome no botão e `value = " "` para colocar um valor no botão, quando os dados forem enviados as informações dentro de `nome` e `value` serão enviadas junto com os dados digitados manualmente pelo usuário.

### INPUT

Input é os campo onde digitamos os dados que serão enviados, podemos criar muitos tipos de input, os atributos básicos que precisamos colocar em um input é o `type` e o `name` , é com o type que selecionamos qual tipo de input vamos usar, um input que aceita texto ou input que aceita números, e-mail, telefone entre outros, como eu disse, existem muitos tipos diferentes de input. usamos inputs diferentes para que o usuário tenha mais facilidade de digitar as informações e que a gente tenha mais facilidade de receber essas informações, por exemplo, quando vc digita em um input de número de celular, automaticamente o teclado do seu celular abre no modo numérico, quando é um input de texto ele abre no teclado normal, da mesma forma que facilita para o usuário, facilita para o desenvolvedor que recebe os dados na formatação correta. 

Também conseguimos usar atributos nos inputs, podemos usar os atributos:

`value` | Deixa o valor como informação padrão no input | Disponível para input do tipo `color` `checkbox` 

`autocomplete` | Ajuda o usuário tentando completar o que esta sendo digitado

`autofocus` | Deixa por padrão o input selecionado

`desabled` | Desabilita o input

`readonly` | Não permite que use o input, se tiver um valor padrão ele não vai poder ser editado

`form` | Permite que você conecte o input que esta fora do form usando o id de um form

`required` | Torna o preenchimento do input obrigatório

`placeholder` | Deixa uma informação no fundo do input, exemplo “digite seu nome aqui”

`max` | Definir numero máximo | Disponível para input do tipo `number` `range` 

`min` | Definir numero mínimo | Disponível para input do tipo `number` `range` 

`step` | Define o passo da contagem, um em um, dois em dois… | Disponível para input do tipo `number` `range` 

`multiple` | Usado para enviar mais de uma informação, separado por “,” | Disponível para input do tipo `email` `file` 

`minlength` | Define a quantidade mínima de caracteres | Disponível para input do tipo `email` `text` `password` 

`maxlength` | Define a quantidade máxima de caracteres | Disponível para input do tipo `email` `text` `password` 

`pattern` | Estruturar uma padrão de dados aceitos, exemplo só aceita e-mail com @empresax.com | Disponível para input do tipo `email` `password` 

`inputmode` | Permite informar para o sistema qual o tipo de informação esta sendo enviada para abrir o teclado no tipo número ou texto.  | Disponível para input do tipo `password` 

`accept` | Informa qual tipo de arquivo é aceito | Disponível para input do tipo `file` 

`checked` | Deixa o elemento marcado automaticamente | Disponível para input do tipo `checkbox` 

Para selecionar o tipo de input usamos os types:

`text` | Envia texto

`number` | Envia números, permite os atributos

`email` | Usado para validar se é um e-mail

`password` | Envio de senhas

`file` | Permite enviar arquivos

`range` | Selecionar em um slide bar

`color` | Selecionar cores

`checkbox` | Selecionar caixas

`radio` | Selecionar apenas uma opção

`hidden` | Input que não é visível, usado para taguear o usuário por exemplo

Esses são os inputs e atributos básicos, mas existem mais, é importante sempre olhar a documentação para aprender novos. 

### LABEL

Basicamente o Label é o título do input, dessa forma o título do input fica atrelado a ele, isso é muito importante principalmente na acessibilidade.

### TEXTAREA

TextArea cria um campo de texto, uma área que permite escrever mais de uma linha sem problemas.

### SELECT

Select serve para selecionar valores, podemos configurar para ser possível selecionar apenas um valor ou mais, criamos as opções de valores usando o `<option>` .

### FIELDSET

Permite fazer agrupamento de inputs, útil para separar partes diferentes de um formulário muito grande.

![ex07.png](https://i.ibb.co/tMF0d6w/img-6.png)

> Confira o exercício 07 em Formulários > ex07.

Nesse exercício praticamente usamos todos os conhecimentos que adquirirmos anteriormente, mas o foco aqui é o uso dos elementos do HTML direcionados para os formulários, usamos os inputs principais que a maioria dos formulários tem.
> 

![ex08.png](https://i.ibb.co/Hh5VCR8/img-7.png)

> Confira o exercício 08 em Formulários > ex08.

No exercício 08 nos aprofundamos mais nas opções de formulário, como por exemplo o uso do  elemento switch, e as opções de select.
> 

---

# CSS FUNCTIONS

CSS Functions, são funções aplicadas como valores em propriedades CSS. Elas estão divididas em categorias como transformação, matemática, filtros, cores, degradês, formatos, funções de referência, entre outras. Essas funções são diferentes das pseudo-funções e funções de importação. Cada função tem argumentos específicos para definir seu comportamento. Algumas functions css são:

### TRANSFORM

A função transform é usada para movimentação, rotação e tamanho, conseguimos usar em elementos como uma div, aplicando:

`transform: translate()` | movimentação

`transform: rotate(10deg)` | rotação

`transform: scale()` | tamanho

### MATH

As funções matemáticas servem para fazer cálculos básicos dentro do CSS, como soma e subtração, exemplo podemos usar na estilização de uma div `calc(20% + 10rem)` , também existem outras funções matemáticas mais complexas como por exemplo a de comparação de `min()` e `max()` entre outras, lembrando que é sempre válido olhar a documentação para se manter atualizado das opções disponíveis.

### FILTER

Filter serve para editar elementos principalmente imagens, é possível fazer edições como aplicar `blur()`, alterar o brilho com `brightness()` ou até mesmo alterar a opacidade `opacity()` do elemento e usar o famoso efeito de sombra com o `drop-shadow()` e muito mais.

### COLORS

Usamos a função color para adicionar cores nos elementos usando o `rgb()`, `hsl()` e `color-mix()` para misturar cores diferentes.

### GRADIENT

Serve para aplicar gradiente no elemento, usamos `linear-gradient()`, para fazer um gradiente linear para alguma direção, podemos indicar a direção como por exemplo `to right` ou informas os graus com `deg`. Podemos fazer um gradiente radial, formato se circulo, com `radial-gradient()` , também existem outras funções.

### SHAPE

O shape funciona como uma mascará em cima do elemento, podemos usar o `circle()` que aplica uma mascara no formato de circulo ou `polygon()` para criar outras formas.

### REFERENCES

Usamos essa função para basicamente pegar informações de outros lugares, como a `var()` que buscamos uma variável que criamos em outro lugar ou a `url()` para usar um elemento de imagem por exemplo.

### OUTRAS

Novamente vale lembras que existem muitas outras funções no CSS, até mesmo mais funções das que já foram comentadas dentro dos tópicos a cima, sempre precisamos olhar a documentação para ver as possibilidades que podemos usar em diferentes projetos, levando em consideração que não da para decorar tudo.

---

# RESPONSIVIDADE

Responsividade é a capacidade do layout se adaptar a diferentes tamanhos de telas e diferentes dispositivos, por exemplo, nós conseguimos usar um site no celular graças a responsividade que ajusta todos os elementos para que se adaptem ao tamanho da tela do seu celular.

### CSS MEDIA QUERIES

O CSS Media Queries é uma ferramenta que permite adaptar o design de uma página conforme o dispositivo do usuário, como desktop ou mobile.

### SINTAXE

Para ativar os elementos de responsividade usamos os breakpoints, que funcionam como gatilhos para ativar a mudança no layout, exemplo, usamos a medida de `width: 500px` para trocar a cor de fundo da página, quando a página chegar no tamanho de 500px de largura a cor vai ser trocada.  Normalmente usamos esses gatilhos para trocar o tamanho dos elementos do site, para que se encaixem em diferentes tamanhos de telas. Um exemplo real dessa aplicação é colocar o breakpoint na largura de 500px, e usar isso como gatilho para o titulo da página ficar com a fonte menor e ter uma leitura mais tranquila para quer acessar o site pelo celular.

![ex09.png](https://i.ibb.co/SJFPW7N/img-8.png)

> Confira o exercício 09 em Responsividade > ex09.

Nesse exercício usamos os conceitos básicos de responsividade, criamos o site base, o projeto Zingen e deixamos ele responsivo para os celulares, fizemos um recurso bem interessante nos botões, colocamos gradiente em botões com bordar arredondadas (Não é possível fazer isso “nativamente” no CSS).
> 

![ex10.png](https://i.ibb.co/f1X53Gw/img-9.png)

> Confira o exercício 10 em Responsividade > ex10.

O objetivo desse exercício foi deixar o projeto Travelgram responsivo para dispositivos mobile.
> 

![ex11.png](https://i.ibb.co/KN4C2sj/img-10.png)

> Confira o exercício 11 em Responsividade > ex11.

O objetivo desse exercício foi deixar o projeto Tech News responsivo para dispositivos mobile.
> 

![ex12.png](https://i.ibb.co/CmpDKXq/img-11.png)

> Confira o exercício 12 em Responsividade > ex12.

O objetivo desse exercício foi deixar o projeto Estrelas do Amanhã responsivo para dispositivos mobile. Finalizando assim a responsividade de alguns projetos anteriores.
> 

---

# CSS ANIMATION E TRANSITION

O CSS com o passar dos anos se tornou uma ferramenta muito poderosa de estilização dentro da Web, conseguimos fazer animações e transições apenas usando o CSS, animação nada mais é do que um efeito com inicio e fim, existem muitas animações dentro do CSS, podemos ver várias delas no site https://animista.net/.

### TRANSITION

Transição é um efeito de suavidade para trocar o valor de um elemento no HTML, como por exemplo trocar a cor de fundo de uma div, depois que um botão foi pressionado, ou trocar o formato de um botão depois que ele foi pressionado, sem a transição o elemento muda de forma imediata, abrupta, com a transição tudo acontece de forma suave e linear, e existem muitas transições diferentes dentro do CSS.

Para aplicar as transições usamos uma gatilho, como o hover, e a sintaxe é a seguinte:

`transition-property:` | Escolher qual propriedade vai ser aplicada a transição.

`transition-duration:` | Determinar quanto tempo vai durar a transição.

`transition-delay:` | Determina um tempo de espera para a transição começar.

`transition-timing-function:` | Seleciona uma curva de aceleração para a transição, podemos usar o lenar, ease, ease-in, ease-out, ease-in-out e mais.

### ANIMATION

Animação basicamente é a mudança de um elemento dentro de uma linha do tempo, assim como funciona nas transições, mas na animações conseguimos fazer coisas mais complexas.

Usamos os keyframes para montar a linha do tempo, damos uma nome para o keyframe e colocamos o estado de inicio e fim da animação, exemplo:

```jsx
@keyframes move {
	from {
		transform: translateY(0)
	}
	to {
		transform: translateY(300px)
	}
}
```

Dessa forma estamos aplicando um keyframe que vai mover o elemento verticalmente 300px para baixo, vale lembrar que alinha do tempo começa em 0% e vai até 100%, from(**início**), to(**fim**). Podemos substituir o from e to pela porcentagem que desejamos.

E para esse linha do tempo funcionar precisamos colocar na estilização do elemento o nome e a duração, exemplo:

`animation-name: move;` | Usamos o nome do keyframe.

`animation-duration: 1s;` | Colocamos a furação da animação.

`animation-delay: ;` | Aplicar um tempo de espera para a animação começar.

`animation_fill-mode: ;` | Define como a animação aplica estilos ao seu destino antes e depois de sua execução.

`animation-direction: ;` | Determina a direção da linha do tempo.

`animation-iteration-count: ;` | Seleciona quantas vezes a animação vai ser executada, podendo ser infinita com infinite.

`animation-play-state: ;` | Ativa ou desativa uma animação, a partir de um gatilho como o hover.

Por fim, conseguimos usar também a animation timeline para controlar a animação com o scroll da página ou a view, que na minha opinião é um dos recursos mais interessantes da animação.

Colocamos dentro da estilização do elemento:

`animation-timeline: scroll();` | A timeline é controlada pelo scroll.

`animation-timeline: views();` | A timeline é controlada pelo espaço de visualização da página, inicia quando visualizamos o elemento e finaliza quando ele não aparece mais na nossa visualização. 

As animações estão ficando cada vez mais completas no CSS, mas nem todas são compatíveis com todos os navegadores, então é sempre interessante pesquisar na documentação a disponibilidade dessas animações e até mesmo pesquisar novos recursos de animação.

![ex13.png](https://i.ibb.co/qRgLSpy/img-12.png)

> Confira o exercício 13 em Animation e Transition > ex13.

Aqui começamos a fazer nossas primeiras animações e transições, criamos recursos bem legais como a entrada da imagem na hero, barra escrolando o nome “Patins” em um background mudando de cor e muito mais.
> 

![ex14.png](https://i.ibb.co/zh2syr0/img-13.png)

> Confira o exercício 14 em Animation e Transition > ex14.

Nesse exercício pegamos o projeto e deixamos responsivo para a visualização mobile.
> 

![ex15.png](https://i.ibb.co/tZ7JNT4/img-14.png)

> Confira o exercício 15 em Animation e Transition > ex15.

O projeto usa o mesmo princípio do anterior com a diferença de usar algumas animações e transições diferentes, o projeto também teve sua versão responsiva no ex16.
> 

---

# CONSIDERAÇÕES FINAIS

Com todo esse conhecimento já é possível começar a desenvolver os seus primeiros projetos usando HTML e CSS, e também você já tem conhecimento suficiente para explorar bibliotecas de estilização, elas facilitam seu processo de desenvolvimento, exemplo, existem bibliotecas feitas especialmente para formulários, outras que te ajudam na responsividade…

Eu venho de um contexto do Web Design, trabalho com o desenvolvimento no-code e sei que esse conhecimento em HTML e CSS me ajudou muito, acho que todo Web Designer precisa entender o mínimo dessas ferramentas, já que na pratica usamos elas diariamente nos nossos projetos, mas fazemos usando usando um page builder.

Espero que todo esse resumo tenha te ajudado de alguma forma :)
