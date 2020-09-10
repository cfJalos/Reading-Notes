[Home page](https://cfjalos.github.io/Reading-Notes/)
## Responsive Web Design and Regular Expressions

### CSS Grid Garden

CSS Grid Garden is a tuturial found [HERE](https://cssgridgarden.com/), which walks users through CSS grid and how to use it.

Using the `grid-column-start` property tells the css where to start a certain action. 

Using `grid-column-start` will span one column.

To extend an item across multiple columns, use `grid-column-start` along with `grid-column-end`.

You can use these properties from right-to-left or from left-to-right. Use negative values to indicate counting columns from left-to-right.

The `span` keyword can be used in the `grid-column-end` or `grid-column-start` property to indicate how long an item should span as well.

Instead of using `grid-column-start` and `grid-column-end`, you can use `grid column: a / b` as shorthand, where a is the `grid-column-start` value and b is the `grid-column-end` value.

The `span` keyword can also be used with the shorthand `grid-column` property.

The `grid-row-start` property can be used to indicate which row an item should be positioned on. This property is used similarly to the `grid-column-start` and `grid-column-end` properties. 

Similarly, the shorthand for `grid-row-start` is `grid-row`.

To set a position both vertically and horizontally, `grid-column` and 'grid-row` can be used together.

The shorthand for using both `grid-column' and `grid-row` together is: `grid-area`.

`grid-area` accepts four values separated by slashes (`grid-row-start`, `grid-column-start`, `grid-row-end`, `grid-column-end`).

Additionally, `grid-area` can be used multiple times to overlap an area.

The `order` property allows items to be placed in a specific order, overriding the item's source code order. 

By default, all grid items have an `order` of 0, which can be set to any positive or negative value. 

The grid itself can also be customized with the `grid-template-columns` and `grid-template-rows` properties. 

Use the `repeat` function for a shorthand version of the `grid-template-columns` and `grid-template-rows` properties.