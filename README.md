# FlexGrid
FlexGrid is a responsive grid that allows developers to use a 12-column grid to layout their site, while providing automatic content reflow for different browser widths. The reflow is controlled by the `.group` class, which developers can use to designate areas of related content that can be reshuffled. If grouping is not designated, the grid columns are scaled evenly by the browser width. 

*Ex. Defining a 4-column row as a `.group` will split the content into two 2-column rows when viewed on a tablet.* 

Typography has also been slightly optimized to make sure columns are within the optimal reading range of 50-70 characters per line.

## Syntax
- The grid elements must be wrapped inside of a "container" class
- The first element in a row must contain the "first" class

*IMPORTANT: `.group` currently only works with `.grid3` and `.grid4` columns. If you have a suggestion for how to handle columns of other sizes, let me know!*

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