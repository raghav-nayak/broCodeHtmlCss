`overflow`
- sets the desired behavior when content does not fit in the parent element box(overflows)
- options:
	- visible -> shows as it is
	- hidden -> hides the overflowed text; but you can copy the entire text when you select it
	- clip -> similar to hidden. But used with `overflow-clip-margin`
		- e.g. `overflow-clip-margin: 13px;` -> overflows 13px, rest will be hidden
	- scroll -> provides scrollbar both horizontal and vertical
	- auto -> similar to scroll, but if it is not needed, then won't be displayed.

<hr>

```html
<body>
    <div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem officiis dolores cum. Sed, quisquam quam quos
            facilis corrupti sequi sint, vero fugiat consectetur blanditiis deleniti consequuntur illo quo numquam.
            Quis?</p>
    </div>
</body>
```


```
div {
    border: 2px solid;
    height: 75px;
    overflow: visible;
    overflow: hidden;
    overflow: clip;
	overflow-clip-margin: 13px;
	overflow: scroll;
    overflow: auto;
}
```