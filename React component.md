
UI interface building block (like LEGO). 

Sometimes a component could be reused.

Components are functions with a [[JSX]] return value.

For example this is a "Header" component within a [[React]] app created in the element with `id="app"` attribute.

```html
<div id="app"></div>

<script type="text/javascript">

  const element = document.getElementById("app");

  function Header() {
    return (<h1>Develop. Preview. Ship. 🚀</h1>)
  }


   ReactDOM.render(<Header />, element)
</script>
```

**Note**: the component function name is capitalized to distinguish it from simple functions.


Components can be nested into each other just like in HTML. This nested structure is called `Component tree`.

