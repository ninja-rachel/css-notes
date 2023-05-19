The [`grid-template`](https://developer.mozilla.org/docs/Web/CSS/grid-template) property is a shorthand for `grid-template-rows`, `grid-template-columns` and `grid-template-areas`. The rows are defined first, along with the value of `grid-template-areas`. Column sizing is added after a `/`.

```css
.container {    
	display: grid;    
	grid-template:      "head head head" 		
	minmax(150px, auto)      "sidebar content content" auto      
	"sidebar footer footer" auto / 1fr 1fr 1fr;
}
```