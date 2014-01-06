AdaptiveGrid
============

Fluid CSS grid framework which adapts to screen size. For example, if you needed a column of 50% to become full width on mobile you'd add the class smallest_to_100 to it.

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

Options: .perc100, .perc80, .perc70, .perc66, .perc50, .perc40, .perc33, .perc30, .perc25, .perc20, .perc16

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
| smallest   | 0px to 480px     | .**smallest**`_to`_100
| smaller    | 481px to 600px   | .**smaller**_to_100
| small      | 601px to 767px   | .**small**_to_80
| medium     | 768px to 1023px  | .**medium**_to_50
| large      | 1024 to 1199px   | .**large**_to_33
| larger     | 1200px and more  | .**larger**_to_20

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
