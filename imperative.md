---
aliases:
  - imperatively
---

Imperative programming is defining all the steps required to achieve something.

A good example for this is:
```javascript
const numbers = [0, 1, 2];
for(let i = 0; i < numbers.length; i++) {
	numbers[i] = numbers[i] * 2;
}

console.log(numbers); // [ 0, 2, 4 ]
```

The (preferred) other type of programming is called [[declarative]].