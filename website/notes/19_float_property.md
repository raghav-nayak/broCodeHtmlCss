`float`
- allows other elements to flow around it
- we use `float: right;` or `float: left;`

`display: flow-root;` -> to make images contained within the border of the body; otherwise the image goes beyond the border

<hr> 

```html
<body>
    <img src="./images/lotr_logo.png" height="200px" id="img1">

    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Hic, perferendis beatae vel amet possimus fugiat alias
        sunt eos aperiam maxime quisquam cupiditate magni praesentium reprehenderit ipsam! Saepe laborum illo ipsum.</p>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Hic, perferendis beatae vel amet possimus fugiat alias
        sunt eos aperiam maxime quisquam cupiditate magni praesentium reprehenderit ipsam! Saepe laborum illo ipsum.</p>

    <img src="./images/lotr_ring.jpeg" height="200px" id="img2">

    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Hic, perferendis beatae vel amet possimus fugiat alias
        sunt eos aperiam maxime quisquam cupiditate magni praesentium reprehenderit ipsam! Saepe laborum illo ipsum.</p>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Hic, perferendis beatae vel amet possimus fugiat alias
        sunt eos aperiam maxime quisquam cupiditate magni praesentium reprehenderit ipsam! Saepe laborum illo ipsum.</p>
</body>
```


```css
body {
    border: 3px solid;
    display: flow-root; /* to make images contained within the border of the body*/
}

#img1 {
    float: right;
    margin-right: 10px;
}

#img2 {
    float: left;
    margin-left: 10px;
}
```


html output:
![html output](../src/images/element_float.png)