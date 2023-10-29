
A JavaScript extension that allows [[DOM]] creation with HTML like syntax.

For example it's used within [[React]]:
```javascript
const app = document.getElementById('app');
ReactDOM.render(<h1>Develop. Preview. Ship. 🚀</h1>, app);
// -------------|..................................| <--- this HTML like part is JSX
```

Browsers don't understand JSX out of the box, so a compiler is needed (eg. [[Babel]]) to transform JSX to regular JavaScript.

Apart from these [3 rules](https://react.dev/learn/writing-markup-with-jsx#the-rules-of-jsx) the syntax is the same as HTML:
1. Return a single root element
	- If you need two elements next to each other use an empty tag (called Fragment) as root:
```
<>
	<div>Elem 1</div>
	<div>Elem 2</div>
</> 
 ```
2. Close all the tags. Even self-closing tags like `<img>` has to be `<img />`.
3. Use camelCase for attributes. Note: `class` is a reserved word in JS so it becomes `className`

There is a [HTML to JSX converter](https://transform.tools/html-to-jsx).