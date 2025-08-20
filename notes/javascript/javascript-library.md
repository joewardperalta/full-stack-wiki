# What is a JavaScript Library

A **JavaScript library** is a collection of prewritten JavaScript code that provides developers with reusable fucntions, utilities, and components. Instead of writing everything from scratch, you can "call" these ready-made pieces of code to solve common problems faster.

Think of it as a **toolbox**:

- Without a library you'd need to build every tool yourself (like a hammer, screwdriver, etc.).
- With a library you already have those tools ready, so you can focus on building the house (the actual application).

## Why Use a Library Instead of Vanilla JavaScript?

JavaScript can do everything by itself, but libraries are used because they:

1. **Save Time** - You don't need to reinvent the wheel for common tasks.
2. **Simplify Complex Tasks** - For example, manipulating the DOM (HTML elements) or handling state is much easier.
3. **Cross-Browser Compatibility** - Libraries implement efficient, well-tested solutions.
4. **Community Support** - Popular libraries are maintained and improved by thousands of developers.

### Example: Vanilla JS vs React

Let's say you want a button that increases a counter when clicked.

#### Vanilla JavaScript

```html
<button id="btn">Click me</button>
<p id="count">0</p>

<script>
  let count = 0;

  document.getElementById("btn").addEventListener("click", () => {
    count++;
    document.getElementById("count").innerText = count;
  });
</script>
```

#### React

```jsx
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <>
      <button onClick={() => setCount(count + 1)}>Click me</button>
      <p>{count}</p>
    </>
  );
}
```

With React, the logic is **cleaner and reusable**, and React automatically updates the UI when state changes.

## In Summary

- A **JavaScript library** is a collection of reusable code.
- It's used to save time, simplify tasks, and ensure efficient, maintainable code.
