When you create a grid using `grid-template-rows` and `grid-template-columns` you create what is known as the **explicit grid**. This is a grid that you have defined and given size to the tracks.

Sometimes you will have items which display outside this explicit grid. 
For example, you might define column tracks and then add several rows of grid items without ever defining row tracks. The tracks would be auto sized by default. You also might place an item using `grid-column-end` that is outside of the explicit grid defined. In both of these cases grid will create tracks to make the layout work, and these tracks are referred to as the **implicit grid**.

Most of the time it will make no difference if you are working with an implicit or explicit grid. However, with line-based placement you may run into the main difference between the two.

Using negative line numbers you can place items from the end line of the explicit grid. This can be useful if you want an item to span from the first to the last column line. In that case you can use `grid-column: 1 / -1`. The item will stretch right across the explicit grid.

This only works for the explicit grid however. Take a layout of three rows of auto-placed items where you would like the very first item to span to the end line of the grid.

You might think that you can give that item `grid-row: 1 / -1`. In the demo below you can see that this doesn't work. The tracks are created in the implicit grid, there is no way to reach the end of the grid using `-1`.

[[grid cell]]