## React / React Native / Gatsby

### **React**

It's a Javascript lib that uses concepts from funcional programming to manage the web DOM through effects in in the elements of it.

#### **React | Concepts**

* **Functional Programming - Imutability**: A Functional Programming concept, when working on this concept we are not allowed to modify the original object/array
itself but instead, we should always work based on a copy of the original item.

```js
const fruitsArray = ['apple', 'peach', 'guava']

const newFruitsArray = [...fruitsArray, 'banana']
```

* **React HOC - High Order Components**: Works the same ways of Javascript HOF. In React this technique allow us to create reusable components extending its features.
We have a function that receives one component as parameter and returns a new component that encapsulates the original component. We can use to add the pagination
feature to a component that render a list of itens for example.

```js
import React, { useState } from 'react';

const withPagination = (Component) => {
  return (props) => {
    const [currentPage, setCurrentPage] = useState(1);

    const handlePageChange = (page) => {
      setCurrentPage(page);
    }

    return (
      <Component
        {...props}
        currentPage={currentPage}
        onPageChange={handlePageChange}
      />
    );
  }
}

const ItemList = (props) => {
  return (
    <div>
      {/* Shows itens list */}
      {/* Shows the pagination controls */}
    </div>
  );
}

const PagedItemList = withPagination(ItemList);
```

#### **React | Observations**

* **Source Map:** Allows to see the application code even in the bundle file created by Webpack! **Security alert!** <https://www.capscode.in/blog/how-to-hide-reactjs-code-from-browser#env-file-in-reactjs>

#### **React | Performance Tips**

* **Code Splitting**: Web development technique where we split the code in smaller files allowing the application to have a faster loading time. In the most
cases the code splitting should be made at the route level, but we can also use as a 'lazy loading' to load elements on demand.

* **States and Components Otimization** 
    - In Redux or others global state managers, is a good pratice to split the global state when possible in mutiple stores according to where we have to use
    these states (usually in big applications).
    - We should keep states close as possible to where it will be used.
    - If there is a costly logic in the state, use a state initializer function instead of executing it directly, because this function will be executed only once.

```js
// instead of this which would be executed on every re-render:
const [state, setState] = React.useState(myExpensiveFn());

// prefer this which is executed only once:
const [state, setState] = React.useState(() => myExpensiveFn());
```
