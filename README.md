AdaptiveGrid
============

Fluid CSS grid framework which adapts to screen size. For example, if you needed a column of 50% to become full width on mobile you'd add the class smallest_to_100 to it.

Options
=======

Gutter Size
===========
The number of pixels between the columns.

Example:

```css

<div class="grid gut[10/20/30]">

```

```css

<div class="grid gut10">
	<div class="col perc50 smallest_to_100">
		<div class="inner"></div>
	</div>
	<div class="col perc50 smallest_to_100">
		<div class="inner"></div>
	</div>
	<div class="col perc50 smallest_to_100">
		<div class="inner"></div>
	</div>
	<div class="col perc50 smallest_to_100">
		<div class="inner"></div>
	</div>
</div>
	
```
