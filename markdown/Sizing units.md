
### Numbers

``` css
p {  
font-size: 24px;  
line-height: 1.5;  
}
```
Numbers have meaning depending on their context.For example, when defining `line-height`, a number is representative of a ratio if you define it without a supporting unit:
In this example, `1.5` is equal to **150%** of the `p` element's **computed pixel font size**. This means that if the `p` has a `font-size` of `24px`, the line height will be computed as `36px`.

### Percentage
If you set a `transform` value as a percentage, **it is based on the element with the transform set.** In this example, the `p` has a `translateX` value of `10%` and a `width` of `50%`. First, calculate what the width will be: `150px` because it is **50% of its parent's width**. Then, take `10%` of `150px`, which is `15px`.
```css
div {
	width: 300px;
	height: 100px;
}

div p {
	width: 50%; /* calculated: 150px */
	transform: translateX(10%); /* calculated: 15px */
}
```



