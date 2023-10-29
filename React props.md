
The [[React component]] can accept an object as parameter. This is the `props` object.

For example let's pass part of the `title` as a parameter and access it using [[Object destructuring]]:
```html
<div id="app"></div>

<script type="text/javascript">

  const element = document.getElementById("app");

  function Header({ title }) {
    return (<h1>{{ title }} Develop. Preview. Ship. 🚀</h1>)
  }


   ReactDOM.render(<Header title="React 💙" />, element)
</script>
```