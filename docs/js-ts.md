## Javascript / Typescript

* **Filter(Boolean)**: Retorna somente se a condição for verdadeira, ignorando os valores "falsy" como null e undefined.

```js
isDevelopment && new ReactRefreshWebpackPlugin(), 
new HtmlWebpackPlugin({
    template: path.resolve(__dirname, 'public', 'index.html')
})
].filter(Boolean),
```

* **Operador '??'**: Nova funcionalidade do Javascript, tendo o seu uso mais comum quando queremos atribuir um valor padrão a algo. Se um valor 'a' é 'defined' então retorna 'a', se o valor 'a' é 'undefined' então retornamos 'b': 

```js
result = a ?? b 

// é igual a

result = (a !== null && a !== undefined) ? a : b
```

* **Operador '&&'**: Executa um código dada uma determinada condição somente se esta for verdadeira. É como uma validação ternária que só retorna verdadeiro.

```js
isDevelopment && console.log("Ambiente de Desenvolvimento")
```

* **[TS] Tipagem de Função**: A função handleClick recebe um parâmetro do tipo 'NUMBER' e não retorna nada 'VOID'.

```ts
handleClick: (id: number) => void;
```
