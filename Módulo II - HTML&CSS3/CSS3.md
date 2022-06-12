# CSS3
- Criado após o HTML para formatar as páginas web.
- Cria regras de estilo para elementos ou grupo de elementos.
- Uma regra CSS é representada por um seletor ou um grupo de seletores que vem do HTML, no exemplo abaixo usamos o `<a>`, então dentro de um par de chaves adicionamos as declarações, as declarações são formadas por uma propriedade `color` e um valor `red`.

```css
a {
    color: red;
}
```
Quando vamos aplicar uma regra a vários seletores de uma vez, separamos eles por vírgulas.

### ID e Classe
ID: é representado pelo símbolo # seguido do nome para esse ID.

```
No HTML:
<a ID="profile"></a>

No CSS:
#profile{
 color: red;
}
```
Class: representada de forma parecida com o ID, mas é precedida por um ponto.
```
No HTML:
<a class="profile"></a>

No CSS:
.profile{
 color: red;
}
```

###### Nota
O ID só pode ser usado uma vez em uma página HTML, já a classe não tem restrições.

### Box-model
Quando estamos criando o layout de um site o navegador representa cada elemento HTML como uma caixa retangular. Como o CSS nós alteramos a aparência dessa caixa. Essa caixa é composta por 4 áreas: content, padding, border e margin.

- **Margin:** são espaçamentos entre elementos;
- **Border:** são as bordas da caixa;
- **Padding:** é o espaçamento entre as bordas e o conteúdo, a diferença para a margin é que declarações de imagens de fundo funcionam nele;
- **Content:** é o conteúdo que o seu bloco representa, um texto, uma imagem, um vídeo.

### Padding e Margin
Usados para atribuir tamanhos para o _box_. Existem algumas formas de fazer isso.

A caixa possui um eixo Y e um eixo X
O eixo Y representa as partes superior e inferior
O eixo X representa os lados esquerdo e direito 

A primeira forma de colocar valor paras as partes superior e inferior e depois para os lados esquerdo e direito é declarando apenas dois valores

```css
div{
    padding: 10px 5px;
}
```
O valor 10px refere ao eixo Y e o valor 5px ao eixo X.

A segunda forma é atribuindo um valor para cada lado do _box_.
``` css
div{
    padding: 15px 10px 5px 0;
}
```
Os valores são definidos no sentido horário, ou seja o valor 15px é o parte superior, o valor 10px é o lado direito, o valor 5px é o parte inferior e o 0 é o lado esquerdo.

###### Nota
Quando o valor for 0 não precisa colocar unidade.

A terceira forma é usando as propriedades especificas para cada lado.
``` css
div{
    padding-top: 15px;
    padding-left: 10px;
    padding-bottom: 5px;
    padding-right: 0;
}
```

### Definir cores
A definição de cores pode ser feita de 3 formas:
1. Pelo nome da cor em inglês (red);
2. Pelo código hexadecimal (#ffffff);
3. Usando apenas o atalho _background_

### Border
As bordas do _box_ possui três propriedades, largura, cor e estilo.

A largura pode ser usada com várias unidades, como px, em e mm.
A cor pode ser definido da mesma forma como citado tópico _Definir cores_.
O estilo é representado por palavras, como:
**solid:** mostra uma borda simples e reta;
**dotted:** são bolinhas com um pequeno espaçamento entre elas;
**dashed:** forma uma linha tracejada;

``` css
div{
    border: solid 1px color: red;
}
```
As propriedades especificas são _border-width_ para a largura, _border-color_ para a cor e _border-style_ para o estilo.

**border-radius**
É uma propriedade que permite arrendondar os cantos de um elemento. Podemos usar várias unidades, mas as mais comuns são o pixels e a porcentagem.

Colocando apenas um valor mudamos todos os cantos do elemento. Mas seguindo a mesma regra do padding e margin (superior, direita, inferior e esquerda), conseguimos alterar ca da canto separadamente. 


### Estilização de textos
`font-family` altera a fonte do nosso texto, podemos usar uma fonte que esteja instalada no nosso computador ou da internet.

`font-size` altera o tamanho do texto, podemos várias unidades de medidas, as mais comuns são o pixels, em e rem.

`font-style` altera o texto para itálico.

