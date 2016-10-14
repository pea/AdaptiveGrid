AdaptiveGrid
============

AdaptiveGrid is a fluid CSS grid framework which adapts to the screen size. It is customizable, letting you quickly create your own column and gutter sizes.

Example
=======

```html

<div class="grid gut10">
	<div class="col perc20 smallest-to-100 smaller-to-50 small-to-50 medium-to-50">
		<h1>Column 1</h1>
	</div>
	<div class="col perc80 smallest-to-100 smaller-to-50 small-to-50 medium-to-50">
		<h1>Column 2</h1>
	</div>
	<div class="col perc50 smallest-to-100">
		<h1>Column 3</h1>
	</div>
	<div class="col perc50 smallest-to-100">
		<h1>Column 4</h1>
	</div>
</div>

```

Options
=======

Gutter Size
===========
The number of pixels between the columns.

Either: gut5, gut10, gut15, gut20, gut30, gut40, gut50, gut60, gut70, gut100

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

These set of classes allow you to easily control the behavior of columns and gutter depending on the screen size without having to mess with the media queries themselves.

| Name       | Screen Size      | Example Column Class   | Example Gutter Class
| ---------- | ---------------- | -----------------------| --------------------
| smallest   | 0px to 480px     | .**smallest**\-to\-100 | .**smallest**\-to\-5
| smaller    | 481px to 600px   | .**smaller**\-to\-100  | .**smaller**\-to\-10
| small      | 601px to 767px   | .**small**\-to\-80     | .**small**\-to\-15
| medium     | 768px to 1023px  | .**medium**\-to\-50    | .**medium**\-to\-20 
| large      | 1024 to 1199px   | .**large**\-to\-33     | .**large**\-to\-30  
| larger     | 1200px and more  | .**larger**\-to\-20    | .**larger**\-to\-40

Column sizes can be edited via the variables $mobile-small-portrait-width, $mobile-small-landscape-width, $mobile-small-landscape-width, $mobile-large-width, $mobile-large-width, $mobile-large-width, $tablet-portrait-width, $tablet-landscape-width and $desktop-width.

**Example:** Both columns 100% on iPhone-sized screens

```html

<div class="grid gut10">
	<div class="col perc50 smallest-to-100"></div>
	<div class="col perc50 smallest-to-100"></div>
</div>
	
```

**Example:** First and second column 50% on iPad-sized screens

```html

<div class="grid gut10">
	<div class="col perc30 medium-to-50"></div>
	<div class="col perc70 medium-to-50"></div>
</div>
	
```

**Example:** You can add similar syntax to the gutter. For example:

```html

<div class="grid gut10 smallest-to-5">
	<div class="col perc30 medium-to-50"></div>
	<div class="col perc70 medium-to-50"></div>
</div>
```
	
Show and Hide
=============

Show and hide any element with .**size**-hide or **size**-show.

note: The -show option will hide the element by default.

**Example:** Show the second column and hide the first column between screen sizes of 768px to 1023px.

```html

<div class="grid gut10">
	<div class="col perc30 medium-to-50 medium-hide"></div>
	<div class="col perc70 medium-to-50 medium-show"></div>
</div>
	
```
