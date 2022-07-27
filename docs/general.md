## Anotações Gerais

* **SASS**: Pré-processador de css, muito útil para manter uma organização dos estilos, principalmente pela possibilidade de implementação de herança, tal como na Orientação a Objetos.

* **SASS - '&'**: O '&' no SASS indica uma referência do elemento em questão a ele mesmo. No exemplo abaixo estamos aplicando 'margin-top' a todas as 'li' que também possuem uma li acima dela.<br>

```css
li {
    & + li {
        margin-top: 20px;
    }
}
```
