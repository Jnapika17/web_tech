# Experiment 5: Interactive Web Pages Using JavaScript

## Aim
Respond to user actions and update page content with JavaScript.

## Steps
1. Add an input, a button, and an output element.
2. Listen for a button click.
3. Read the input value and display a greeting in the output element.

## Example
```html
<input id="name" aria-label="Name">
<button id="greet">Greet</button>
<p id="output"></p>
<script>
  document.querySelector("#greet").addEventListener("click", () => {
    const name = document.querySelector("#name").value;
    document.querySelector("#output").textContent = `Hello, ${name}!`;
  });
</script>
```

## Result
Built a page that updates its content in response to user interaction.
