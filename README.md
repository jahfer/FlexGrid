# FlexGrid
The FlexGrid framework is a responsive grid that allows developers to use a 6-column grid to layout their site, while providing easy, natural wrapping when the site is narrowed.

## Syntax
- The grid elements must be wrapped inside of a "container" class
- The first element in a row must contain the "first" class
- Multiple rows can be grouped together in order to define a consistent way to wrap and combine rows together when shifted from a 3-column layout to a 2-column one. 
*Note* the "group" class currently only works with "grid2" class elements inside it.

	<div class="container">
		<div class="grid1 first"></div>
		<div class="grid5"></div>

		<section class="group">
			<div class="grid2 first"></div>
			<div class="grid2"></div>
			<div class="grid2"></div>

			<div class="grid2 first"></div>
			<div class="grid2"></div>
		</section>
	</div>