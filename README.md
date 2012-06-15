# FlexGrid
FlexGrid is a responsive grid that allows developers to use a 12-column grid to layout their site, while providing automatic content reflow for different browser widths. The reflow is controlled by the `.group` class, which developers can use to designate areas of related content that can be reshuffled. If grouping is not designated, the grid columns are scaled evenly by the browser width. 

*Ex. Defining a 4-column row as a `.group` will split the content into two 2-column rows when viewed on a tablet.* 

Typography has also been slightly optimized to make sure columns are within the optimal reading range of 50-70 characters per line.

[See the demo »](http://dev.jahfer.com/flexgrid/)

## Syntax
- The grid elements must be wrapped inside of a "container" class
- The first element in a row must contain the "first" class

```html
<div class="container">
	<!-- keeps same ratio for tablet and desktop -->
	<div class="grid2 first"></div>
	<div class="grid10"></div>

	<!-- columns inside columns -->
	<div class="grid12 first">
		 <div class="grid9 first"></div>
		 <div class="grid3"></div>
	</div>

	<!-- changes from 3-column on desktop to 2-column on tablet -->
	<section class="group">
		<div class="grid4 first"></div>
		<div class="grid4"></div>
		<div class="grid4"></div>

		<div class="grid4 first"></div>
		<div class="grid4"></div>
	</section>
</div>
```