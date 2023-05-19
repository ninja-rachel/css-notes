It’s common that an object method needs to access the information stored in the object to do its job.

For instance, the code inside `user.sayHi()` may need the name of the `user`.

**To access the object, a method can use the `this` keyword.**

The value of `this` is the object “before dot”, the one used to call the method.

For instance:
```javascript

let user = { 
	name: "John", 
	age: 30, 
	sayHi() { // "this" is the "current object"
		alert(this.name);
	} 
}; 
	user.sayHi(); // John
```
