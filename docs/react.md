## React / React Native / Next / Gatsby

### **Next.js**

Framework React que utiliza algumas ferramentas Javascript baseadas em Rust que possibiltam o uso de algumas fetaures do backend para processas itens no front.

### **React**

* **Source Map:** Possibilita ver o código da aplicação mesmo no arquivo bundle gerado pelo Webpack. **Atenção para a segurança!** <https://www.capscode.in/blog/how-to-hide-reactjs-code-from-browser#env-file-in-reactjs>

* **Programação Funcional - Imutabilidade**: Conceito da programação funcional na qual o React se inspirou, diz que não devemos alterar o objeto original, para trabalharmos com eles, devemos criar cópias desse objeto com as alterações que queremos.

```js
const listaDeFrutas = ['maçã', 'pêssego', 'goiaba']

const novaListaDeFrutas = [...listaDeFrutas, 'banana']
```

* **Refresh Webpack Plugin**: Mantém alterações no state para fins específicos.

#### **React / Performance**

* **Divisão de Código/Code Splitting**: Técnica de dividir o código em arquivo menores, permitindo que a aplicação carregue o conteúdo parcialmente na medida em que os recursos são requisitados.

Na maioria das vezes a divisão do código deve ser feita ao nível da rota, mas também pode ser usado para as partes 'lazy load' da aplicação na qual o carregamento é feito aos poucos também.

* **Otimização de Componentes e States** 
    - Não coloque tudo em um único state. divida o state global em múltiplas 'stores' de acordo com onde o state será usado.
    - Mantenha o state o mais próximo possível de onde será utilizado.
    - Se houver um cálculo custoso no state, utilize uma função inicializadora de state ao invés de executá-lo diretamente, porque essa função será executada apenas uma vez.

```js
// instead of this which would be executed on every re-render:
const [state, setState] = React.useState(myExpensiveFn());

// prefer this which is executed only once:
const [state, setState] = React.useState(() => myExpensiveFn());
```
