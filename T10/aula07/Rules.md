# Rules (Regras) do Sass

## Importando arquivos Sass

Para você conseguir importar arquivos Sass, use `@import` ou `@use`. O `@import` está com seus dias contados pois o *Sass* adicionou `@use` pois é automatizada.
```scss
@use "sass:math";
@import "./sass/bgcolors"; /// Preferência para @use!
```

Quando você usa o `@use` deve se referir como objeto:
```scss
@use "./sass/bgcolors";

.div1 {
    @include Divs(bgcolors.$bg-red); /// nomedoarquivo.variável
}
```

Para chamar uma função use dessa maneira:
```scss
.div2 {
    @include Divs(bgcolors.funcao());
}
```

## `@return`

Ele retorna algo de uma `@function` ou `@mixin`

## `@mixin`

O mixin é tipo uma função só que você pode reutilizar no seu código Sass. Você pode colocar parâmetros!.

## Debug

O `@debug` só é visivel no terminal da IDE, no navegador não é possível ver no console!

## Aviso no Sass

Escreve um aviso no terminal, para mostrar algo por exemplo.

## Error no Sass

Mostra o error, como neste exemplo:
```scss
$status-msg: "Status da Compilação do Arquivo";
$archive: "_bgcolors.scss";
$status: () !global;

$colors: (
    'one': hsl(0, 100%, 50%),
    'two': hsl(60, 100%, 50%),
    'three': hsl(240, 100%, 50%)
);

@function Divs($back) {
    @if not map-has-key($colors, $back) {
        $status: "background-color: #{$back} (inexistente)";
        @error "#{$status-msg} #{$archive}: #{$status}";
        @return hsl(0, 0%, 0%);
    } @else {
        @return map-get($colors, $back);
    }
}
```