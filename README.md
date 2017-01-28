Reference Doc
============
## Box Model

#### CSS
```css
.my-element {

	html, body {
	    height: 100%;
	    box-sizing: border-box;
	}
	
	*, *:before, *:after {
	    box-sizing: inherit;
	}
	
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
