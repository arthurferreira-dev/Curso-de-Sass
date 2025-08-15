# O que e Por que usar um Pré-Processador CSS?

Os pré-processadores dão uma roupagem para o CSS, evita repitir linhas de estilo e convertem para CSS para que o navegador entenda

## Lista de Pré-Processadores
* PostCSS
* Less
* Sass

## Lista de Sites para você usar e testar seus arquivos Sass/Scss
* [Sass Playground](https://sass-lang.com/playground/)
* [JS Fiddle](https://jsfiddle.net)

No *Sass* é possível usar **Variáveis Globais** que nem do CSS, elas não precisam do `:root` para serem declaradas e precisam começar com `$` não com `--`

<img src="/imgs/variaveis-sass.png" alt="Sass Playground">

Também podemos meio que "dividir" em partes, com a função do *Sass* o `@mixin <nome do mixins>` e podemos incluir isso em qualquer coisa nele com o `@includes`

<img src="/imgs/mixin-includes-sass.png" alt="Sass Playground">