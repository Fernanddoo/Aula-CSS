# CSS

O CSS, ou Cascading Style Sheets (Folhas de Estilo em Cascata), é a linguagem que usamos para dar estilo, cor, e vida às nossas páginas da web. Enquanto o HTML estrutura o conteúdo, o CSS cuida da aparência.

Com o CSS, você pode controlar cores, fontes, espaçamentos, tamanhos, e muito mais.

## Como funciona o CSS?

A sintaxe do CSS é composta por três partes principais: o seletor, a propriedade e o valor.

```css
seletor {
    propriedade: valor;
}
```

- **Seletor:** Aponta para o elemento HTML que você deseja estilizar. Pode ser uma tag, uma classe, ou um ID.

- **Propriedade:** É o atributo de estilo que você deseja alterar, como color (cor do texto) ou font-size (tamanho da fonte).

- **Valor:** É a configuração que você atribui à propriedade. Por exemplo, blue para a propriedade color, ou 16px para font-size.

## Como adicionar o CSS em uma página HTML??

Existem 3 maneiras para adicionar o CSS em um HTML:

1. CSS Externo:

```html
<link rel="stylesheet" href="style.css">
```

2. CSS Interno:

```html
<style>
  p {
    color: green;
  }
</style>
```

3. CSS Inline:

```html
<h1 style="color: red;">Meu Título</h1>
```

## Quais os estilos mais comuns e utilizados no CSS??

1. **Estilos de Texto e Fontes**

- **color:** Define a cor do texto.
- **font-family:** Especifica a família da fonte a ser usada.
- **font-size:** Controla o tamanho do texto.
- **font-weight:** Define a "espessura" da fonte (negrito, fina, etc...).
- **text-align:** Alinha o texto horizontalmente (esquerda, direita, centro, justificado).
- **text-decoration:** Adiciona ou remove decorações do texto (como sublinhado).

2. **Cores e fundos**

- **background-color:** Define a cor de fundo de um elemento.
- **background-image:** Aplica uma imagem como fundo de um elemento.
- **background-repeat:** Controla como a imagem de fundo se repete.
- **background-size:** Define o tamanho da imagem de fundo.

3. **Espaçamento e Box Model**

- **margin:** Define os espaçamentos **Externos** de um elemento (margem).
- **padding:** Define os espaçamentos **Internos** de um elemento (borda).

4. **Dimensões e Bordas**

- **width:** Define a largura de um elemento.
- **height:** Define a altura de um elemento.
- **border:** Forma abreviada para definir espessura, estilo e cor de uma borda.
- **border-radius:** Permite arredondar os cantos da borda de um elemento.

## Exemplo prático

index.html:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Primeira Página com CSS</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="cartao">
        <h1>Olá, Mundo do CSS!</h1>
        <p>Esta é a minha primeira experiência estilizando uma página com CSS. Estou aprendendo sobre seletores, propriedades e valores.</p>
        <a href="#">Saiba Mais</a>
    </div>
</body>
</html>
```

style.css:

```css
body {
    background-color: #f4f4f4;
    font-family: Arial, sans-serif;
}

.cartao {
    width: 80%;
    margin: 40px auto;
    padding: 20px;
    background-color: white;
    border: 1px solid #ddd;
    border-radius: 8px;
}

h1 {
    color: #333;
    text-align: center;
}

p {
    font-size: 16px;
    line-height: 1.6;
}

a {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    background-color: #007BFF;
    color: white;
    text-decoration: none;
    border-radius: 5px;
}
```

## Flexbox e Grid

Layout é a forma como organizamos os elementos em uma página. Queremos criar colunas? Alinhar itens lado a lado? Centralizar algo perfeitamente na tela? Para tudo isso, usamos Flexbox ou Grid.

## Flexbox: Alinhamento em uma dimensão

Pense no Flexbox quando você precisa organizar elementos em uma única linha ou em uma única coluna. Ele é perfeito para alinhar itens em um menu de navegação, distribuir cartões de produtos lado a lado ou centralizar um bloco de conteúdo.

Para começar a usar o Flexbox, você precisa de dois elementos: um contêiner (o elemento pai) e os itens dentro dele (os elementos filhos).

Para ativar, basta adicionar flex ao contêiner:

```css
.container {
    display: flex;
}
```

## Propriedades mais comuns do Flexbox (Aplicando em contêiner):

- **flex-direction:** Define a direção do eixo principal.
- **justify-content:** Alinha os itens ao longo do eixo principal.
- **align-items:** Alinha os itens ao longo do eixo transversal.
- **gap:** Adiciona um espaçamento consistente entre os itens flexíveis.

## Grid

Pense no Flexbox quando você precisa organizar elementos em uma única linha ou em uma única coluna. Ele é perfeito para alinhar itens em um menu de navegação, distribuir cartões de produtos lado a lado ou centralizar um bloco de conteúdo.

Para ativar, basta adicionar grid ao contêiner:

```css
.container {
    display: grid;
}
```

## Propriedades mais comuns do Grid (Aplicando em contêiner):

- **grid-template-columns:** Define o número de colunas do grid.
- **grid-template-rows:** Define o número de linhas do grid.
- **gap:** Adiciona um espaçamento entre as linhas e colunas. Pode ser **column-gap** ou **row-gap** também.

# Unidade fr:

A unidade fr representa uma fração do espaço disponível no contêiner. Ao utilizar:

```css
.galeria {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}
```

Estamos criando 3 colunas de tamanho igual que ocupam todo o espaço disponível.

## Flexbox vs. Grid: Quando usar cada um?

- **Use flexbox:** Para componentes e alinhamentos em uma dimensão. Ótimo para menus, listas de itens, e para alinhar elementos dentro de um componente.
- **Use grid:** Para o layout geral da página e para qualquer coisa que precise de alinhamento em duas dimensões (linhas e colunas ao mesmo tempo).

## Vamos jogar e aprender mais??

[Flexbox Froggy](https://flexboxfroggy.com/#pt-br)
[Flexbox Zombies](https://mastery.games/flexboxzombies) - Precisa de conta!!!