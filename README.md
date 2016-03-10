AdaptiveGrid
============

AdaptiveGrid is a fluid CSS grid framework which adapts to the screen size. It is customizable, letting you quickly create your own column and gutter sizes.

Example
=======

```css

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

Either: gut10, gut20 or gut30

**Example:**

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

Options: .perc100, .perc80, .perc70, .perc66, .perc60, .perc55, .perc50, .perc45, .perc40, .perc33, .perc30, .perc25, .perc20, .perc16, .perc10

**Example:**

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

| Name       | Screen Size      | Example Class
| ---------- | ---------------- | -------------
| smallest   | 0px to 480px     | .**smallest**\_to\_100
| smaller    | 481px to 600px   | .**smaller**\_to\_100
| small      | 601px to 767px   | .**small**\_to\_80
| medium     | 768px to 1023px  | .**medium**\_to\_50
| large      | 1024 to 1199px   | .**large**\_to\_33
| larger     | 1200px and more  | .**larger**\_to\_20

**Example:** Both columns 100% on iPhone-sized screens

```css

<div class="grid gut10">
	<div class="col perc50 smallest_to_100"></div>
	<div class="col perc50 smallest_to_100"></div>
</div>
	
```

**Example:** First and second column 50% on iPad-sized screens

```css

<div class="grid gut10">
	<div class="col perc30 medium_to_50"></div>
	<div class="col perc70 medium_to_50"></div>
</div>
	
```

Adding New Column and Gutter Sizes
=======================

To create a new column size, add to the $column_sizes SCSS variable.

$column_sizes: **5** 10 16.66666666666667 20 25 30 33.3333333333 40 45 50 55 60 66.6666666666 70 80 100;

To add a new gutter size, add to the $gutter_sizes SCSS variable.

$gutter_sizes: 5 10 15 20 **25** 30 40 50;
