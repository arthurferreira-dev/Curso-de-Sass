# Módulos Incorporados

Módulos são arquivos, cada folha de estilo é um módulo. Por padrão o Sass traz módulos padrões nos seus arquivos.

## Utilizando Módulos Incorporados no Sass

Para utilizar basta colocar `@use "sass:nomedomodulo"`.

```scss
@use "sass:string";
```

Vou deixar uma tabela dos módulos disponíveis:

| Para que serve? | @use do Módulo |
| --------------- | -------------- |
| Modifica as Cores | `@use "sass:color";` |
| Guarda e modifica elementos em uma list | `@use "sass:list";` |
| Ajuda no mapeamento de elementos | `@use "sass:map";` |
| Operações Matemáticas | `@use "sass:math";` |
| Ajuda a utilizar melhor os `@mixins` | `@use "sass:meta";` |
| Seletor que retorna um valor Booleano | `@use "sass:selector";` |
| Transformação de Strings | `@use "sass:string";` |

## Mais informações sobre os Módulos Sass

[Documentação do Sass na parte de Módulos](https://sass-lang.com/documentation/modules/)