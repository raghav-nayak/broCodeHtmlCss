keywords added to a selector

e.g.
when I `hover` a button, font size of the button is increased

link
active
hover
visited

`not` is used as negation

`nth-child()`
- you can give 
	- a number
	- odd
	- even
	- Xn - e.g. 3n -> every third element -> 3,6,9
	- Xn + offset - e.g. 3n+1 -> 1,4,7

<hr>

<br>
```html
<body>
    <a href="https://google.com"> google </a>

    <ul>
        <li> This is #1 </li>
        <li> This is #2 </li>
        <li> This is #3 </li>
        <li> This is #4 </li>
        <li> This is #5 </li>
        <li> This is #6 </li>
        <li> This is #7 </li>
        <li> This is #8 </li>
        <li> This is #9 </li>
        <li> This is #10 </li>
    </ul>

    <div id="greet"> Hover here
        <p> Hello </p>
    </div>
</body>
```


```css
a:link {
    color: rgb(183, 255, 0);
}

a:hover {
    color: green;
    font-size: 1.4em;
}

a:active {
    color: blue;
    font-size: 2em;
}

a:visited {
    color:grey;
}



li:hover {
    background-color: greenyellow;
}

li:not(:hover) {
    background-color: grey;
}

li:nth-child(3n) {
    background-color: peru;
}


#greet p {
    background-color: lightblue;
    padding: 10px;
    display: none;
}

#greet:hover p {
    display: block;
}
```