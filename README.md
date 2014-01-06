AdaptiveGrid
============

Fluid CSS grid framework which adapts to screen size. For example, if you needed a column of 50% to become full width on mobile you'd add the class smallest_to_100 to it.

Options
=======

Gutter Size
===========
The number of pixels between the columns.

Either: gut10, gut20 or gut30

Example:

For a gutter of 10px.

```css

<div class="grid gut10">
	<div class="col perc50"></div>
	<div class="col perc50"></div>
</div>

```

Column Sizes
============

The column widths of AdaptiveGrid are in percentages, opposed to set sizes, which means any column size is available. A few of the most common ones are available for you to code the majority of designs

Options: .perc100, .perc80, .perc70, .perc66, .perc50, .perc40, .perc33, .perc30, .perc25, .perc20, .perc16

Example:

For two columns of 50% and a full width column below them.

```css

<div class="grid gut10">
	<div class="col perc50"></div>
	<div class="col perc50"></div>
	<div class="col perc100"></div>
</div>

```

Adaptive Grid
=============

These set of classes allow you to easily control the behaviour of columns depending on the screen size without having to mess with the media queiries themselves.

| Class Name | Screen Size |
| ---------- | ----------- |
| Smallest   | lala |

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
