# Experiment 7: React Components, Props, and Children

## Aim
Create reusable components that display values passed through props and children.

## Steps
1. Define a function component that accepts props.
2. Render it more than once with different values.
3. Pass nested content and display it through `children`.

## Example
```jsx
function Card({ title, children }) {
  return <section><h2>{title}</h2><div>{children}</div></section>;
}

function App() {
  return <Card title="Topics"><p>React components</p></Card>;
}
```

## Result
Created reusable components with dynamic props and child content.
