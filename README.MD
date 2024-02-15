# Dicionário de CSS Básico
## Do que se trata o CSS?
O CSS **informa** ao navegador como exibir a página web. Podemos usá-lo para definir **cor, fonte, tamanho** e outros aspectos dos elementos HTML.

## Sintaxe básica do CSS
```css
element {
    property: value;
}
```

Esse se trata de um **seletor de tipo**, onde colocamos o elemento e definimos um estilo para todos os elementos desse tipo.

Quando tivermos um mesmo estilo para vários seletores de tipos diferentes, podemos usar a seguine sintaxe de declaração:
```css
selector1, selector2 {
    property: value;
}
```

Outro tipo de seletor CSS que podemos usar é o **seletor de id** (identificador único), ele serve para que possamos estilizar um **elemento específico**. Sua sintaxe é a seguinte:
```css
#name-id{
    property: value;
}
```

Agora o tipo mais comum de seletor é o **seletor de classe**, um seletor de classe serve para estilizarmos elementos pertencentes a mesma classe, e diferente do `ìd` não é único. Sua sintaxe é a seguinte:
```css
.class-name {
    styles;
}
```

## Vinculação do CSS ao HTML
Para vincular uma folha de estilos ao nosso HTML, devemos adicionar ao elemento `<head></head>` uma tag chamada `<link>` os seguintes atributos: **href** com o valor do caminho de onde está localizada nossa folha de estilos, e **rel** com o valor `"stylesheet"`.

Além disso, é importante adicionarmos a seguinte tag `<meta>`:
`<meta name="viewport" content="width=device-width, initial-scale=1.0" />`

Esse metadado serve para que a estilização da página **pareça semelhante, independente do dispositivo**.

## Alinhamento de Texto
Para alinhar nossos elementos de texto do HTML, temos a propriedade `text-align`, que possui valores como **center, justify, right e left**.

## Background
Para estilizarmos o fundo ou corpo de um elemento, possuimos diversas propriedades:
- `background-color`: Que permite estilizar a cor do fundo do elemento;
- `background-image`: Que permite que o fundo de um elemento seja uma imagem.

```css
body {
    background-color: #000000;
    background-image: url(path to img);
}
```

## Largura dos elementos
Para tratarmos a largura de um elemento, devemos usar a propriedade `width`, com ela podemos definir exatamente a largura que o elemento vai ter e ocupar na página.

## Comentários em CSS
Sintaxe:
```css
/* Comentários */
```

## Margem de um Elemento
No CSS temos a propriedade `margin` que como seu próprio nome diz, define a margem do elemento, é como um **espaço invisível em torno do elemento**.

Um exemplo de uso para a `margin` é centralizar um elemento horizontalmente:
```css
#menu {
    margin-left: auto;
    margin-right: auto;
}
```

# Dicionário HTML

## Div
O elemento `<div></div>` é diferente dos elementos semânticos, ele é usado principalmente para **fins de layout de design** e organização do código.
```html
<div class="apresentacao_links">
    <a href=""> Google </a>
    <a href=""> Bing </a>
</div>
```

## Article
Elemetos `<article></article>` geralmente guardam elementos que possuem **informações relacionadas**. Por exemplo, o nome e o preço de um produto.
```html
<article>
   <p> Fiat Uno </p>
   <p> R$ 20.000,00 </p> 
</article>
<article>
   <p> Fiat Siena </p>
   <p> R$ 50.000,00 </p> 
</article>
```