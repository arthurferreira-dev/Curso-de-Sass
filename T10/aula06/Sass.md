# Interpolação no Sass

A *interpolação* é um processo de analizar uma expressão ou uma string, com uma ou mais variáveis.

> [!TIP]
> A **Interpolação** é muito parecida com a **Concatenação**

## Exemplo em **Sass**
```scss
$inter: 'Sass';
/// Exemplo em interpolação em PHP: echo "A variável tem o valor " . $inter . "!";
@debug "Isso é um teste de Interpolação em Sass, valor da variável 'teste': #{$inter}";
```