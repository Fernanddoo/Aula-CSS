# CSS

O CSS, ou Cascading Style Sheets (Folhas de Estilo em Cascata), é a linguagem que usamos para dar estilo, cor, e vida às nossas páginas da web. Enquanto o HTML estrutura o conteúdo, o CSS cuida da aparência.

Com o CSS, você pode controlar cores, fontes, espaçamentos, tamanhos, e muito mais.

## Como funciona o CSS?

A sintaxe do CSS é composta por três partes principais: o seletor, a propriedade e o valor.

'''css
seletor {
    propriedade: valor;
}
'''

- Seletor: Aponta para o elemento HTML que você deseja estilizar. Pode ser uma tag, uma classe, ou um ID.

- Propriedade: É o atributo de estilo que você deseja alterar, como color (cor do texto) ou font-size (tamanho da fonte).

- Valor: É a configuração que você atribui à propriedade. Por exemplo, blue para a propriedade color, ou 16px para font-size.

## Como adicionar o CSS em uma página HTML??

Existem 3 maneiras para adicionar o CSS em um HTML:

1. CSS Externo:

'''html
<link rel="stylesheet" href="style.css">
'''

2. CSS Interno:

'''html
<style>
  p {
    color: green;
  }
</style>
'''

3. CSS Inline:

'''html
<h1 style="color: red;">Meu Título</h1>
'''

## Quais os estilos mais comuns e utilizados no CSS??

1. Estilos de Texto e Fontes

- color: Define a cor do texto.
- font-family: Especifica a família da fonte a ser usada.
- font-size: Controla o tamanho do texto.
- font-weight: Define a "espessura" da fonte (negrito, fina, etc...).
- text-align: Alinha o texto horizontalmente (esquerda, direita, centro, justificado).
- text-decoration: Adiciona ou remove decorações do texto (como sublinhado).

2. Cores e fundos

- background-color: Define a cor de fundo de um elemento.
- background-image: Aplica uma imagem como fundo de um elemento.
- background-repeat: Controla como a imagem de fundo se repete.
- background-size: Define o tamanho da imagem de fundo.

3. Espaçamento e Box Model 

- margin: Define os espaçamentos *Externos* de um elemento (margem).
- padding: Define os espaçamentos *Internos* de um elemento (borda).

4. Dimensões e Bordas

- width: Define a largura de um elemento.
- height: Define a altura de um elemento.
- border: Forma abreviada para definir espessura, estilo e cor de uma borda.
- border-radius: Permite arredondar os cantos da borda de um elemento.

## Exemplo prático

index.html:

'''html
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
'''

style.css:

'''css
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
'''

## Flexbox e Grid

Layout é a forma como organizamos os elementos em uma página. Queremos criar colunas? Alinhar itens lado a lado? Centralizar algo perfeitamente na tela? Para tudo isso, usamos Flexbox ou Grid.