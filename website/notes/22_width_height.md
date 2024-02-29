#div #border #padding 

by default height and width are automatically set.

`height: auto;`

you can use auto, %, px with height and width.

`div` is a block container. Even though there is extra space, it consumes entire width.

To make use of that space, `float` property can be used.
float: left; If you make it right, the first div will be on right, and second one will be on left.

while calculating element display, it will consider border and padding. We can use `box-sizing: border-box;` to make sure that border and padding are not used while calculating the size.

`max-width: 25%;`
max-width overrides the width property.

`min-width` overrides both `max-width` and `width` property.


max-height
min-height

viewport
`height: 100vh;` 100vh means 100 viewport; it will take entire viewing page

<hr>

<br>
```html
<body>
    <div class="container">
        <div class="box">
            <h2> This is #1 </h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis autem minima odit adipisci
                voluptatum,
                labore tempore hic id repudiandae cupiditate dicta deleniti neque facilis rem suscipit enim! Eaque, esse
                ratione.</p>
        </div>
        <div class="box">
            <h2> This is #2 </h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis autem minima odit adipisci
                voluptatum,
                labore tempore hic id repudiandae cupiditate dicta deleniti neque facilis rem suscipit enim! Eaque, esse
                ratione.</p>
        </div>
    </div>
</body>
```

```css
* { /* * means all elements */
    box-sizing: border-box; /* to make sure that border and padding are not used while calculating the size. */
}

.container {
    background-color: red;
    height: 100vh; /* 100vh means 100 viewport; it will take entire viewing page  */
}


.box {
    border: 2px solid;
    padding: 25px;
    /*box-sizing: border-box; /* to make sure that border and padding are not used while calculating the size. */

    height: auto;
    /* height: 200px; */
    /* height: 50%; */

    /* width: auto; */
    /* width: 200px; */
    width: 50%;

    float: left;

    text-align: center;

    min-width: 100%;
    max-width: 25%;

    min-height: 25%;
    

}
```
