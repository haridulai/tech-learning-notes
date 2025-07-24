# createRoot

## What I learned
- Importing react in a static web page - index.html
```html
    <div id="root"></div>
```

- index.jsx: to import createRoot, create a root with the div with id of "#root" 
- render markup to the root
```jsx
  import { createRoot } from "react-dom/client"
  const root = createRoot(document.getElementById("root"))
  root.render(<h1>Hello, React</h1>)
```

### Alternative index.jsx examples

Using document.querySelector("#root")
```jsx
  import { createRoot } from "react-dom/client"
  const root = createRoot(document.querySelector("#root"))
  root.render(<p>Hello from the world of React</p>)
```

Chaining the methods together
```jsx
  import { createRoot } from "react-dom/client"
  createRoot(document.querySelector("#root")).render(<p>Hello from the world of React!</p>)
```

Importing entire ReactDOM library
```jsx
  import ReactDOM from "react-dom/client"
  ReactDOM.createRoot(document.querySelector("#root")).render(<p>Hello from the world of React!</p>)
```
