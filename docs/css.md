## CSS

* **SASS**: Pré-processador de css, muito útil para manter uma organização dos estilos, principalmente pela possibilidade de implementação de herança, tal como na Orientação a Objetos.

* **SASS - '&'**: O '&' no SASS indica uma referência do elemento em questão a ele mesmo. No exemplo abaixo estamos aplicando 'margin-top' a todas as 'li' que também possuem uma li acima dela.<br>

```css
li {
    & + li {
        margin-top: 20px;
    }
}
```

* **Box-Model**: 'border-box' -> Desconsidera a 'border' e o 'padding' no tamanho total do elemento. 'content-box' -> Soma a 'border' e o 'padding' no tamanho total do elemento. Por isso geralmente esse estilo é aplicado para todos os elementos.

* **BEM**: Convenção de nomenclatura de css, tem como etsrutura básica 'bloco, elemento e modificador'.

```html
  <div class="c-menu__item">
    <a href="#" class="c-menu__link c-menu__link--disabled">Outro item</a>
  </div>
```
```css
.c-menu__link--disabled {}
```
