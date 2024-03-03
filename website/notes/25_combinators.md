combinators
- explain the relationships between listed selectors
`<space>` (descendant)
`>` (child)
`~` (general sibling)
`+` (adjacent sibling)

usage:
	selector `<combinator>` selector

e.g.
 `div > p`

all children are descendants but not all descendants are children.


<hr>
<br>

```html
<body>
    <div id="container">
        <p> This is 1st paragraph </p>
        <p> This is 2nd paragraph </p>
        <div>
            <p> This is 3rd paragraph </p>
        </div>
    </div>
    
    <p> This is 4th paragraph </p>
    <p> This is 5th paragraph </p>
</body>
```


```css
#container {
    border: 2px solid
}

/* descendent combinator */
#container p {
    background-color: yellow;
}

/* child combinator */
#container > p {
    background-color: red;
}

/* general sibling combinator */
#container ~ p {
    background-color: pink;
}

/* adjacent sibling combinator */
#container + p {
    background-color: blue;
}
```
