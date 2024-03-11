
```css
.container {
    display: flex;
    flex-direction: row;
}
```

options for `flex-direction`
- row e.g. 1, 2, 3, 4
- row-reverse: e.g. 4, 3, 2, 1
- column: displayed in column
- column-revers: displayed in column in reverse order

`justify-content`
- Aligns flex items along the main axis of the current line of the flex container.
- possible values
	- `flex-start` (left aligned)
	- `flex-end` (right aligned)
	- `center`
	- `space-between` (occupies entire line with even spaces between items; left and right items are at extreme end)
	- `space-evenly` (similar to `space-between` but left and right items have equal space before and after respectively)
	- `space-around` (similar to `space-evenly` but not equal space i.e. the space is less than in-between items)

`align-items`
possible values
- `flex-start` (at the top of the container or div)
- `flex-end` (at the bottom of the container or div)
- `center` 
- `baseline` 

`flex-wrap`
by default, all the elements in the container are displayed on the same line. That means there will be truncation if there are many items.
We use `flex-wrap` to change the behavior
Possible values
- `wrap` - works like word wrap; i.e. if there are more elements, those will be moved to the next line
- `wrap-reverse` - it will start at the last line, the remaining elements will be pushed last but one line and so on
- `no-wrap` - will not wrap the elements
It is usually used with `align-content`

`align-content`
similar to `align-items`
Possible options
- `flex-start` (at the top of the container or div)
- `flex-end` (at the bottom of the container or div)
- `center` 
- `space-evenly`
- `space-between`

`column-gap`
- to add vertical(column) gap between two elements in the container 

`row-gap`
- to add horizontal(row) gap between two elements in the container

`align-self`
- applied to a single element
Possible values (vertical alignment)
- start 
- end
- center

`order`
you can change the order of the elements in the container
it takes integer values
1 -> end
-1 -> beginning


<hr>
<br>
```html
<body>
    <div class="container">
        <div class="box" id="box1"> 1 </div>
        <div class="box" id="box2"> 2 </div>
        <div class="box" id="box3"> 3 </div>
        <div class="box" id="box4"> 4 </div>
        <div class="box" id="box1"> 1 </div>
        <div class="box" id="box2"> 2 </div>
        <div class="box" id="box3"> 3 </div>
        <div class="box" id="box4"> 4 </div>
    </div>
</body>
```

```css
.container {
    display: flex;
    /* flex-direction: row; */
    border: 10px solid black;
    height: 90vh;
    /* justify-content: space-evenly; */
    align-items: baseline;
    /* flex-wrap: wrap;
    align-content: flex-start;
    column-gap: 1em;
    row-gap: 1em; */
}

.box {
    width: 150px;
    height: 150px;
    font-size: 8em;
    text-align: center;
    border-radius: 15px;
}

#box1 {
    background-color: red;
    /* align-self: end; */
    order: 1;
}

#box2 {
    background-color: yellow;
    order: -1;
}

#box3 {
    background-color: greenyellow;
}

#box4 {
    background-color: blue;
}
```