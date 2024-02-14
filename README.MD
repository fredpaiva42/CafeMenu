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

## Vinculação do CSS ao HTML
Para vincular uma folha de estilos ao nosso HTML, devemos adicionar ao elemento `<head></head>` uma tag chamada `<link>` os seguintes atributos: **href** com o valor do caminho de onde está localizada nossa folha de estilos, e **rel** com o valor `"stylesheet"`.

Além disso, é importante adicionarmos a seguinte tag `<meta>`:
`<meta name="viewport" content="width=device-width, initial-scale=1.0" />`

Esse metadado serve para que a estilização da página **pareça semelhante, independente do dispositivo**.

## Alinhamento de Texto
Para alinhar nossos elementos de texto do HTML, temos a propriedade `text-align`, que possui valores como **center, justify, right e left**.

## Background
Para estilizarmos o fundo ou corpo de um elemento, possuimos a propriedade `background-color`.

## Div
Apesar de ser um elemento HTML, o elemento `div` é diferente dos elementos semânticos, ele é usado principalmente para **fins de layout de design**.

## Largura dos elementos
Para tratarmos a largura de um elemento, devemos usar a propriedade `width`, com ela podemos definir exatamente a largura que o elemento vai ter e ocupar na página.