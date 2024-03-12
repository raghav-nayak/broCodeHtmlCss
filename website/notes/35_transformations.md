`transform`
possible values
- translateX()
	- move the element in X axis
	- translateX(**int**px)
		- +ve to right, -ve to left
	- translateX(**int**%)
		- based on the percentage of width of the element
 - translateY() -> vertical or y axis
 - translate(x, y) -> x and y axis
	 - x can be +/- px

 - rotateX(**int**deg) -> rotate the element in x axis
 - rotateY(**int**deg) -> rotate the element in y axis
 - rotateZ(**int**deg) => z axis

 - scaleX(**int**) -> n times  ; x axis
 - scaleY(**int**) -> n times  ; y axis
 - scale(**int**) -> n times  ; x axis and y axis
 - scale(**int**, **int**) -> m and n times  ; x axis and y axis

 - skewX(**int**deg) -> tilt in degree in X axis
 - skewY(**int**deg) -> tilt in degree in Y axis
 - skew(**int**deg, **int**deg) -> tilt in degree in X axis and Y axis

You can combine multiple transformations into one.
e.g. `transform: translate(100%) rotateZ(90deg) scale(0.75);`

you can apply this to id, class, images


<hr>

```html
<body>
    <div class="box" id="box1"> Hi </div>
    <div class="box" id="box2"> Hi </div>
    <div class="box" id="box3"> Hi </div>

    <img src="./images/elton_john_rocket_man.jpg" alt="">

</body>
```

<br>

```css
body {
    margin: 0;
}

/* #box1 {
    width: 250px;
    height: 250px;
    border: 5px solid;
    font-size: 13em;
    text-align: center;
    background-color: aqua;

    /* transform: translateX(100%);
    transform: translateY(100%); */
    
    /* transform: rotateX(180deg); */
    /* transform: rotateY(180deg); */
    /* transform: rotateZ(23deg); */

    /* transform: scaleX(3) */
    /* transform: scaleY(3) */
    /* transform: scale(1); */

    /* transform: skewX(45deg); */
    /* transform: skewY(45deg); */
    /* transform: skew(35deg, 60deg); 

    transform: translate(100%) rotateZ(90deg) scale(0.75);
} */


.box {
    width: 250px;
    height: 250px;
    border: 5px solid;
    font-size: 13em;
    text-align: center;

    transform: translateX(100px) rotateZ(45deg) scale(1.2);
}

#box1 {
    background-color: red;
}
#box2 {
    background-color: yellow;
}
#box3 {
    background-color: green;
}

img {
    transform: translateX(100%) rotateZ(180deg) scaleX(2);
}
```

