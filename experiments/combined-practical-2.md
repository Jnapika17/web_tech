# Combined Practical 2: React Application and Components (Experiments 6 + 7)

## Aim
Create a React application and render reusable components with props and children.

## Steps
1. Render the application into the root DOM element.
2. Create a reusable component that accepts a title prop and children.
3. Render multiple instances with different content.

## Example
```jsx
import { createRoot } from "react-dom/client";

function Card({ title, children }) {
  return <section><h2>{title}</h2>{children}</section>;
}

function App() {
  return <Card title="Web Technology"><p>React practical</p></Card>;
}

createRoot(document.getElementById("root")).render(<App />);
```

## Result
Rendered a React app using reusable components, props, and children.
