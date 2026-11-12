# Experiment 6: React Elements, ReactDOM, and the Virtual DOM

## Aim
Render a React element into a web page.

## Steps
1. Create a React project using the class or project setup provided.
2. Add a root element to the HTML document.
3. Render a React element into that root.
4. Change the rendered content and observe the UI update.

## Example
```jsx
import { createRoot } from "react-dom/client";

const root = createRoot(document.getElementById("root"));
root.render(<h1>Hello, React!</h1>);
```

## Result
Rendered a React element and observed React update the page.
