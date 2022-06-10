# HTML5
- Criado em 1991 por Tim Berners-Lee
- Possui 5 versões, sendo a mais atual o HTML5, lançado em 2014.

## Elemento HTML
```
<h1 class="titulo">Título</h1>
```
Um elemento HTML é formado por tag de abertura (`<h1>`), dentro da tag de abertura eu posso usar atributos (`class="titulo"`), e dentro das tags eu posso colocar um conteúdo (`Título`), e por último a tag de fechamento (`</h1>`)

_Existem elementos no HTML que não possuem tag de fechamento._

## Estrutura básica do HTML
```
<!DOCTYPE html>
<html>
    <head>
        <meta>
        <title></title>
    </head>
    <body>
    </body>
</html>
```

_A primeira linha de um documento HTML (`<!DOCTYPE html>`), apesar de parecer um elemento HTML, apenas diz ao navegador que ele está lidando com um arquivo do tipo HTML5._

`<html>`
A tag html é a raiz do documento, todos os elementos HTML devem estar dentro dela. É dentro dela que informamos ao navegador qual é o idioma do nosso documento. Para português brasileira usamos pt-BR.

`head`
A tag head contém elementos que serão lidos pelo navegador, como os metadados - um exemplo é o charset, que é a codificação de caracteres e a mais comum é a UTF-8, os links de arquivos externos, como o do CSS e o título da página.

`<body`
É dentro da tag body que colocamos todo o conteúdo visível ao usuário: textos, imagens, vídeos.

## Semântica

A semântica permite descrever mais precisamente o nosso conteúdo.

`<section>`
Representa um seção genérica de conteúdo quando não houver um elemento mais específico para isso.

`<header>`
É o cabeçalho da página ou de uma seção da página e normalmente contém logotipos, menus, campos de busca.

`<article>`
Representa um conteúdo independente e de maior importância dentro de uma página, como um post de blog, uma notícia em uma barra lateral ou bloco de comentários. Um article pode conter outros elementos, como header, cabeçalhos, parágrafos e imagens.

`<aside>`
É uma seção que engloba conteúdos relacionados ao conteúdo principal, como artigos relacionados, biografia do autor e publicidade. Normalmente são representadas como barra laterais.

`<footer>`
Esse elemento representa o rodapé do conteúdo ou de parte dele, pois ele é aceito dentro de vários elementos, como article e section e até do body. 

`<h1>-<h6>`
São os títulos usados na página. Eles são utilizados para marcar a importância dos títulos, sendo `<h1>` o mais importante e  `<h6>` o menos. O ideal é usar apenas um `<h1>` por página, pois ele representa o objetivo da sua página.

## Textos e links

`<p>`
Representa um parágrafo, mas ele não suporta apenas texto, podemos adicionar imagens, código, vídeos e vários outros tipos de conteúdo dentro dele.

`<a>`
Significa anchor/âncora, ele representa um hyperlink, e ele interliga vários conteúdos e páginas na web.
O elemento `<a>` possui vários atributos, dentre eles está o _href_ e o _target_.
_href_ é usado para representar o hyperlink para onde a âncora aponta, pode ser uma página do seu ou outro site, email ou telefone, usando o prefixo mailto: e tel:, respectivamente.

_target_ ajuda a abrir os links em outra aba do navegador usando o valor __blank_.

exemplo: `<a href="mailto:email@email.com" target="_blank">email@email.com</a>`

## Imagens
`<img>`
O elemento img é usado para adicionar imagens, ele **não possui tag de fechamento**.

É um elemento simples que possui apenas dois atributos, _src_ e _alt_.

O _src_ é obrigatório, é nele que é informado o caminho da imagem que se quer mostrar na página.

Já o _alt_ é opcional, mas é altamente recomendado por melhorar a acessibilidade. Ele mostra a descrição da imagem caso ela não carregue e leitores de tela usam esse atributo para descrever a imagem.

## Listas
As listas servem para agrupar uma coleção de itens. 

`<ul>`
Cria uma lista não ordenada, ou seja, a ordem dos elementos não importam, e é representada com pontos, círculos ou quadrados.

`<ol>`
Serve para criar listas ordenadas, em que a ordem dos elementos importa, portanto elas são representadas com números, algorismos romanos ou letras.

`<li>`
É um item dentro de uma lista. Ele pode conter vários tipos de conteúdos, como parágrafos, imagens e até outras listas.