margins -> space around the elements

As you can see in the inspect element in the browser,
- padding -> space between element and border
- margin -> area outside the border

```css
body {
    margin:0px
}
```

`margin`
- you can specify margin and it will take care of all the four direction margins
- you can specify the directions too. e.g. `margin-left`
- you can also auto

<hr>


```html
<div class="box" id="box1">Box 1</div>
<div class="box" id="box2">Box 2</div>
```

```css

.box {
    border: 5px solid;
    font-size: 5em;
    width: 50 px;
    height: 250px;
    margin: auto; /* the element will be in the middle */
}

#box1 {
    background-color: red;
}

#box2 {
    background-color: yellow;
    margin-left: auto; /*The margin of this element will take as much as possible */
}
```