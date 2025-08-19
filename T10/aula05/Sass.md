# Funções e Mixins

Uma das coisas mais importantes em Sass são as funções e os mixins, as funções podem ser chamadas assim:
```scss
@function funcao() {
    // Passe algo aqui...
}
```

Elas semprem tem que ter os `()` pois podem receber parâmentros, já os mixins ajudam a reutilizar e evitar repetições no css.
```scss
@mixin inputEx {
    $w: 265px;
    $h: 37.5px;
    width: $w;
    height: $h;
}

input {
    @include inputEx();
}
```

As funções são uma forma de deixar mais organizado seus algoritmos em Sass, elas tem `@if` e o `@else` com operadores como <= ou >=, etc e tem como dar um return na função usando o `@return`.

## Extra

Vou te ensinar a como importar um arquivo Sass para outro arquivo Sass!

<img src="/imgs/import-sass.png" alt="Import com Sass">

```scss
@import "Functions/inputs"; // Ele não precisa de extensão pois o próprio Sass sabe que esse arquivo é com Sass

```