
```javascript
let result; 
if (a + b < 4) { 
	result = 'Below'; 
} else { 
	result = 'Over'; 
}

```

``` javascript
let result = (a + b < 4) ? 'Below' : 'Over';
```

```javascript
let message; 
if (login == 'Employee') { 
	message = 'Hello'; 
} else if (login == 'Director') {
	message = 'Greetings'; 
} else if (login == '') { 
	message = 'No login'; 
} else { 
	message = ''; 
}
```

```javascript
let message = (login == 'Employee') ? 'Hello' : 
	(login == 'Director') ? 'Greetings' : 
	(login == '') ? 'No login' : 
	'';
```


