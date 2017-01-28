Reference Doc
============
## Box Model

#### CSS
```css
html, body {
    height: 100%;
    box-sizing: border-box;
}

*, *:before, *:after {
    box-sizing: inherit;
}
```

-----
## Vertically Center Align Element

#### HTML
```html
<div class="my-element">
	This element will be aligned center (vertically).
</div>
```
#### CSS

```css
.my-element {
	position: relative;
    top: 50%;
    transform: translateY(-50%);
}
```


-------
## Padding and Margin

#### HTML
```html
<div class="my-element">
	This element has padding and margin.
</div>
```

#### CSS
```css
.my-element {
	padding: 10px;
	margin: 20px;
}
```
-------
## Fixed Positioning

#### HTML
```html
<div class="sidebar">
	This element's position is fixed and is stacked on the left side, with a width of 30%.
</div>
<div class="main-content">
	This element's position is fixed and is stacked on the right side, with a width of 70%.
</div>
```

#### CSS
```css
.sidebar {
	position: fixed;
	top: 0;
	left: 0;
	bottom: 0;
	width: 30%;
}

.main-content {
	position: fixed;
	top: 0;
	left: 30%;
	bottom: 0;
	width: 70%;
}
```
## Absolute Positioning

#### HTML
```html
<div class="parent">
	<div class="child">
	</div>
</div>
```

#### CSS
```css
.parent {
	position: relative;
	height: 100%;
	width: 100%;
}

.child {
	position: absolute;
	top: 100px;
	left: 100px;
	right: 100px;
	height: 250px;
}
```
----

----
## Background Image

#### HTML
```html
<div class="my-element">
	This element has a round border.
</div>
```

#### CSS
```css
.my-element {
	border: solid 1px #000000;
	border-radius: 4px;
}
```
-------

## Animation

#### HTML
```html
<div class="my-element animate fadeIn">
	This element is hidden (because opacity is 0). It will fade in after 0.5s.
</div>
```

#### CSS
```css
@keyframes fadeIn{
	0% {
		opacity: 0;
	}
	100% {
		opacity: 1;
	}
}

.animate {
	animation-fill-mode: forwards;
    animation-iteration-count: 1;
}

.fadeIn {
	animation-name: fadeIn;
	animation-duration: 1s;
	animation-delay: 0.5s;
}

.my-element {
	opacity: 0;
}
```
