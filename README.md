# FlexGrid
FlexGrid is a responsive grid that allows developers to use a 12-column grid to layout their site, while providing automatic content reflow for different browser widths. The reflow is controlled by the `.group` class, which developers can use to designate areas of related content that can be reshuffled. 

*For example: defining a 4-column row as a `.group` will split the content into two 2-column rows.* 

If grouping is not designated, the grid columns are scaled evenly by the browser width. 

## Syntax
- The grid elements must be wrapped inside of a "container" class
- The first element in a row must contain the "first" class
- Multiple rows can be grouped together in order to define a consistent way to wrap and combine rows together when shifted from a 3-column layout to a 2-column one. 
*Note* the "group" class currently only works with "grid4" class elements inside it.

```html
<div class="container">
	<div class="grid2 first"></div>
	<div class="grid10"></div>

	<section class="group">
		<div class="grid4 first"></div>
		<div class="grid4"></div>
		<div class="grid4"></div>

		<div class="grid4 first"></div>
		<div class="grid4"></div>
	</section>
</div>
```