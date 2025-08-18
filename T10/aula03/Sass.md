# Variáveis com Sass

As variáveis do `Sass` são muito boas pois ela tem uma manutenção fácil no algoritmo, elas são declarados com o `$` no começo.
```scss
$wd: 100px; // Declarei uma variável com o valor de 100px, que pode ter o valor mudado a qualquer HORA.
```

Você pode atribuir elas em classes, ids ou elementos como os exemplos a seguir:

## Scss/Sass
```scss
.exemplo {
    width: $wd; // o width da classe recebe 100px
}
```

## CSS

```css
.exemplo {
    width: 100px;
}
```

Temos dois tipos de variáveis de Sass, a primeira são as `Variáveis Globais` que podem ser acessadas em qualquer declaração, já o segundo são as `Variáveis Privadas` que só podem ser usadas em declarações específicas.

```scss
// Variável Global

$wid: 300px;
$hei: 150px;
$color-blue: blue;
```

```scss
// Variável Privada

@mixin private {
    $wdesp: 100px
    width: $wdesp;
}

.elemento {
    width: $wdesp; // Vai dar ERRO
}
```