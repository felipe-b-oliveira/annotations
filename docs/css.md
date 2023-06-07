## CSS

### General

* **component.module.css**: When we use css module, only the component in the folder have the access to css file.

* **global.css**: When we don't use .module and only put the css extension the css file is available globally.

### CSS Patterns

* **OOCSS**: Each repeatable visual pattern is identified through a class. This patters tries to separate the structures and properties.

* **SMACSS**: Pattern based on the five css rules categories: base, layout, module, state e theme.

* **DRY CSS**: Pattern tha have the principle of don't repeat properties with equals values, when this occurs these properties must be grouped.

* **BEM**: CSS naming convention, has as the basic structure 'block, element and modifier'.

```html
  <div class="c-menu__item">
    <a href="#" class="c-menu__link c-menu__link--disabled">New Item</a>
  </div>
```
```css
.c-menu__link--disabled {}
```

### CSS Pre-Processors

* **SASS**: A popular css pre-processor, useful for styles organization, it implements some Object-Orientation concepts like heritage that helps in css organization (try to solves the !important problem)

* **SASS - '&'**: The symbol '&' in SASS indicates a element self reference. We can see this in the example above. In the example we are applying the 'margin-top' to all 'li' elements that also have another 'li' element above it.<br>

```css
li {
    & + li {
        margin-top: 20px;
    }
}
```

* **Box-Model**: 'border-box' -> Disregard the 'border' and 'padding' in the element total size. 'content-box' -> Sums the 'border' and 'padding' in the element total size. Because this behavior, usually this style is applyed to all elements.
