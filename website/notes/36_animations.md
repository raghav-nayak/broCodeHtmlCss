`keyframes` 
	- `to`
	- `from`
	- percent%

`animation-name`
- takes `keyframes`

`animation-duration`
- takes duration in seconds e.g. 1s

`animation-iteration-count`
- number of times 
- take a number or `infinite`

`animation-direction`
- direction of the animation 
- `normal`, `reverse`, `alternate`, `alternte-reverse`

`animation-play-state:`
- `paused`, `running`
- useful with combination of javascript

`animation-timing-function`
- change the speed
- `ease-in-out`, `ease-out`, `linear` (same speed throughout)
- `step(n)` -> step function to take n steps to complete the animation
- `cubic-bezier()`



we can use pseudo classes too.


```html
<body>
    <div id="box"> Hi </div>
    <img src="./images/lotr_ring.jpeg">
</body>
```

```css
#box {
    width: 250px;
    height: 250px;
    background-color: red;
    font-size: 13em;
    text-align: center;
    /* animation-name: slideDown; */
    /* animation-name: rotateZ; */
    /* animation-name: shrink; */
    /* animation-name: fade; */
    /* opacity: 0;
    animation-name: fadeIn; */

    animation-name: colorChange;
    /* animation-name: glow; */
    animation-duration: 2s;
    animation-iteration-count: 2;
    /* animation-iteration-count: infinite; */
    animation-direction: reverse;
    animation-play-state: running;
    animation-timing-function: ease-in-out;
    /* animation-timing-function: steps(10); */
    animation-timing-function: cubic-bezier();
}

img {
    animation-name: slideLeft;
    animation-duration: 2s;
    animation-iteration-count: 2;
    animation-direction: reverse;
    animation-play-state: running;
    animation-timing-function: ease-in-out;
}

/* #box:hover{
    animation-name: glow;
    animation-duration: 2s;
} */

/* 
active -> when we left click and hold the element
#box:active{
    animation-name: glow;
    animation-duration: 2s;
} */

@keyframes slideLeft {
    /* from{transform: translateX(100px)} */
    from{transform: translateX(300%)} /* from 3 times the size of the element; right to left */
}


@keyframes slideRight {
    /* from{transform: translateX(100px)} */
    to{transform: translateX(300%)} /* from 3 times the size of the element; left to right*/
}

@keyframes slideUp {
    /* from{transform: translateX(100px)} */
    from {transform: translateY(300%)} /* from 3 times the size of the element; bottom to top */
}

@keyframes slideDown {
    /* from{transform: translateX(100px)} */
    to {transform: translateY(300%)} /* from 3 times the size of the element; top to bottom */
}

@keyframes rotateX {
    100% {transform: rotateX(360deg)} /* rotate on the X axis */
}

@keyframes rotateY {
    100% {transform: rotateY(360deg)} /* rotate on the Y axis */
}

@keyframes rotateZ {
    50% {transform: rotateZ(360deg)} /* rotate on the Z axis ; 50% means rotate 180 and then reverse */ 
}

@keyframes grow {
    100% {transform: scale(2, 2)} /* size increases by 200% */
}

@keyframes shrink {
    50% {transform: scale(0.5, 0.5)} /* size decreases by 50% */
}

@keyframes fade {
    50% {opacity: 0;} /* opacity changes to 0 means fade out when element's opacity is 1*/
}

@keyframes fadeIn {
    50% {opacity: 1;} /* opacity changes to 1 means shows when the element's opacity is 0 */
}

@keyframes colorChange {
    0% {background-color: yellow;}
    20% {background-color: orange;}
    40% {background-color: pink;}
    80% {background-color: blue;}
    100% {background-color: purple;}
}

@keyframes glow {
    50% { box-shadow: 0px 0px 50px yellow;}
}
```
