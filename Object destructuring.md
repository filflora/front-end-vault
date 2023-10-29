
Object destructuring is a JavaScript expression that makes it possible to access keys of an object with the same name.

For example:
```javascript
const fruit = {
    name: "apple",
    color: "red"
};

function logFruitProperies(fruit) {
	const { name, color } = fruit;

	console.log("The fruit is called", name, "and its color is", color);
	// The fruit is called apple and its color is red.
}
```


See also: Array destructuring