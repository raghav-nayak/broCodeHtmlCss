`text-shadow`
- horizontal offset, vertical offset, blur(optional), color
	- e.g. `text-shadow: 1px 1px;` , `text-shadow: 1px 1px 5px red;`
- you can give multiple shadows by repeating the same values
	- e.g. `text-shadow: 1px 1px 5px red, -1px -1px 5px green;`

`box-shadow`
- you can use the same thing like `text-shadow`
- used for div

```html
<body>
    <div id="box1">
    </div>
</body>
```

```css
h1 {
    text-shadow: 1px 1px 5px red, -1px -1px 5px green ;
}

#box1{
    width: 100px;
    height: 100px;
    background-color: lightgray;
    box-shadow: 1px 1px 5px red;
}
```