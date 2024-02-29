- `block-level`
	- starts on a new line
	- take up the full width available
	- you can specify the width and height to this.
	- e.g. `h1, div, p, form, header, footer`
- `inline`
	- does not start on a new line
	- width is limited to what is needed
	- if you provide width/height, it will not be applied
	- e.g. `span, a, img`


![](../src/images/element_display_block_inline_1.png)

<hr> 

`display`
- specifies if/how an element is displayed
- using `display`, you can change the display of the element

- `display: block;`
![](../src/images/element_display_block_inline_2.png)

- `display: inline-block;` -> div
![](../src/images/element_display_block_inline_3.png)

- `display: inline-block;` -> span
![](../src/images/element_display_block_inline_4.png)

- `display: inline-block;` -> div
![](../src/images/element_display_block_inline_5.png)

- `display: inline-block;` -> span
![](../src/images/element_display_block_inline_6.png)


- `display: none;` -> does not show the element at all
![](../src/images/element_display_block_inline_7.png)



you can also use `visibility` property with `display` property.
- `display: inline-block; visibility: hidden;` -> hidden but the space is taken by the elements

![](../src/images/element_display_block_inline_8.png)




<hr>


```html
<body>
    <div> div </div>
    <span> span </span>
    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aut ducimus itaque minima tenetur dolorum aliquam
    consequatur voluptatibus minus accusantium laboriosam cum, architecto sit rem voluptatum molestias beatae amet?
    Blanditiis, sed!
</body>
```


```css
div {
    background-color: red;
    width: 100px;
    height: 100px;
    /* display: block; */
    /* display: inline; */
    display: inline-block;
    visibility: hidden;
    /* display: none; */
}

span {
    background-color: green;
    width: 100px;
    height:  100px;
    /* display: block; */
    /* display: inline; */
    display: inline-block;
    /* display: none; */
}
```