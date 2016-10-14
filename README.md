AdaptiveGrid
============

AdaptiveGrid is a fluid CSS grid framework which adapts to the screen size. It is customizable, letting you quickly create your own column and gutter sizes.

Example
=======

```html

<div class="grid gut10">
	<div class="col perc20 smallest_to_100 smaller_to_50 small_to_50 medium_to_50">
		<h1>Column 1</h1>
	</div>
	<div class="col perc80 smallest_to_100 smaller_to_50 small_to_50 medium_to_50">
		<h1>Column 2</h1>
	</div>
	<div class="col perc50 smallest_to_100">
		<h1>Column 3</h1>
	</div>
	<div class="col perc50 smallest_to_100">
		<h1>Column 4</h1>
	</div>
</div>

```

Options
=======

Gutter Size
===========
The number of pixels between the columns.

Either: gut5, gut10, gut15, gut20, gut30, gut40, gut50, gut60, gut70, gut100;

Editable via the $gutter-sizes variable.

**Example:**

For a gutter of 10px.

```html

<div class="grid gut10">
	<div class="col perc50"></div>
	<div class="col perc50"></div>
</div>

```

Add 'outergut' to the .grid element to apply this gutter size to perimeter of the grid.

Column Sizes
============

The column widths of AdaptiveGrid are in percentages, opposed to set sizes, which means any column size is available. A few of the most common ones are available for you to code the majority of designs

Options: .perc100, .perc80, .perc70, .perc66, .perc60, .perc55, .perc50, .perc45, .perc40, .perc33, .perc30, .perc25, .perc20, .perc16, .perc10

Editable via the $column-sizes variable;

**Example:**

For two columns of 50% and a full width column below them.

```html

<div class="grid gut10">
	<div class="col perc50"></div>
	<div class="col perc50"></div>
	<div class="col perc100"></div>
</div>

```

Adaptive Grid
=============

These set of classes allow you to easily control the behavior of columns depending on the screen size without having to mess with the media queiries themselves.

| Name       | Screen Size      | Example Class
| ---------- | ---------------- | -------------
| smallest   | 0px to 480px     | .**smallest**\_to\_100
| smaller    | 481px to 600px   | .**smaller**\_to\_100
| small      | 601px to 767px   | .**small**\_to\_80
| medium     | 768px to 1023px  | .**medium**\_to\_50
| large      | 1024 to 1199px   | .**large**\_to\_33
| larger     | 1200px and more  | .**larger**\_to\_20

These sizes can be edited via the variables $mobile-small-portrait-width, $mobile-small-landscape-width, $mobile-small-landscape-width, $mobile-large-width, $mobile-large-width, $mobile-large-width, $tablet-portrait-width, $tablet-landscape-width and $desktop-width.

**Example:** Both columns 100% on iPhone-sized screens

```html

<div class="grid gut10">
	<div class="col perc50 smallest_to_100"></div>
	<div class="col perc50 smallest_to_100"></div>
</div>
	
```

**Example:** First and second column 50% on iPad-sized screens

```html

<div class="grid gut10">
	<div class="col perc30 medium_to_50"></div>
	<div class="col perc70 medium_to_50"></div>
</div>
	
```

You can add similar syntax to the gutter. For example:

```html

<div class="grid gut10 smallest-to-5">
	<div class="col perc30 medium_to_50"></div>
	<div class="col perc70 medium_to_50"></div>
</div>
	
Show and Hide
=============

Use .**size**-hide or **size**-show to show of hide any element (note: The -show option will hide the element by default). For example:

```html

<div class="grid gut10">
	<div class="col perc30 medium_to_50 medium-hide"></div>
	<div class="col perc70 medium_to_50 medium-show"></div>
</div>
	
```
