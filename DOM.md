
Document Object Model.

An object representation of the HTML elements.

DOM is built by the browser based on the HTML elements. This structure is then further modified by Javascript.

For example this HTML with embedded Javascript declares a new title component in an [[imperative]] way:
```html
<!-- index.html -->
<html>
  <body>
    <div id="app"></div>

    <script type="text/javascript">
      // Select the div element with 'app' id
      const app = document.getElementById('app');

      // Create a new H1 element
      const header = document.createElement('h1');

      // Create a new text node for the H1 element
      const headerContent = document.createTextNode(
        'Develop. Preview. Ship. 🚀',
      );

      // Append the text to the H1 element
      header.appendChild(headerContent);

      // Place the H1 element inside the div
      app.appendChild(header);
    </script>
  </body>
</html>
```

... results in this DOM structure:
```html
<html>
  <body>
    <div id="app">
	    <h1>Develop. Preview. Ship. 🚀</h1>
    </div>

    <script type="text/javascript">
      // ... (content skipped for brevity)
    </script>
  </body>
</html>
```