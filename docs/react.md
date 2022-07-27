## React

* **Source Map:** Possibilita ver o código da aplicação mesmo no arquivo bundle gerado pelo Webpack. **Atenção para a segurança!** <https://www.capscode.in/blog/how-to-hide-reactjs-code-from-browser#env-file-in-reactjs>

* **Programação Funcional - Imutabilidade**: Conceito da programação funcional na qual o React se inspirou, diz que não devemos alterar o objeto original, para trabalharmos com eles, devemos criar cópias desse objeto com as alterações que queremos.

```js
const listaDeFrutas = ['maçã', 'pêssego', 'goiaba']

const novaListaDeFrutas = [...listaDeFrutas, 'banana']
```

* **Refresh Webpack Plugin**: Mantém alterações no state para fins específicos.
