---
aliases:
  - declaratively
---




Declarative programming is only dealing with "what we would like to achieve" and leaves the "how" on the language itself or to [[library|libraries]].

A good example for this is:
```javascript
let numbers = [0, 1, 2];
numbers = numbers.map((number) => number * 2);

console.log(numbers); // [ 0, 2, 4 ]

```

The other type of programming is called [[imperative]].