```javascript
function checkAge(){
	if (age>18) ? true : confirm('Did parents allow you?');
}


```
? = return 
: or return

```javascript
function checkAge(age) { 
	return (age > 18) || confirm('Did parents allow you?'); 
}

```

```javascript
function checkAge(age) { 
	if (age > 18) { 
		return true; 
	} else { 
		return confirm('Did parents allow you?'); 
	} 
}
```

