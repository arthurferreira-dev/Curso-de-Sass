# Aninhamento

No CSS é comum que se escreva elementos dentro de elementos assim:
```css
#elemento li {
    width: 100%;
}
```

Mas no Sass existe o Aninhamento que é um que nem escrever um elemento no outro, veja um exemplo pra tu entender:
```scss
#elemento {
    width: 100px;

    li { // Isso é um aninhamento
        width: 100%;

        elemento {
            // Da para fazer isso também
        }
    }
}
```