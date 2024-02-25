cascading style sheets

There are 3 ways we can apply CSS
1. Inline
	- within any tag, you add CSS within `style` attribute
	- e.g. `<p style="color: white;">`

2. Internal
	- used within `head` tag, specifying different styles for different tags within `style` tag
	- e.g.
```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS introduction</title>
    <style>
        body {
            background-color: black;
        }

        h1 {
            color: white;
        }

        p {
            color: white;
        }
    </style>
</head>
```

3. External
	- most popular
	- all the styling will be in a separate file
	- we use `link` tag for linking the css file and html file
	- e.g. `<link rel="stylesheet" href="13_style.css">`
	- if you want to apply a property to all the similar tags e.g. all `<p>` tags, then you just need to give `p {}`
	- you can also use ids, e.g. `p1 {}`
	- you can use class also. for this, you need to use .classname
	- unlike inline and internal, you can apply external css to more than one html file.


```css
body {
    background-color: black;
}

h1 {
    color: white;
}

p {
    color: white;
} 


#p1{
    color: white;
}

#p2{
    color: red;
}

#p3{
    color: green;
}

#p4{
    color: yellow;
}

.odd {
    color: blue
}

.even {
    color: orange
}
```

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS introduction</title>
    <link rel="stylesheet" href="13_style.css">
</head>

<body>
    <h1> Sample website </h1>

    <p id="p1" class="odd">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illo esse beatae labore quia qui
        voluptatibus ab cum
        nisi ipsa. Cupiditate consequatur voluptatum quo praesentium distinctio autem. Provident ipsa esse in!
    </p>

    <p id="p2" class="even">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illo esse beatae labore quia qui
        voluptatibus ab cum
        nisi ipsa. Cupiditate consequatur voluptatum quo praesentium distinctio autem. Provident ipsa esse in!
    </p>

    <p id="p3" class="odd">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illo esse beatae labore quia qui
        voluptatibus ab cum
        nisi ipsa. Cupiditate consequatur voluptatum quo praesentium distinctio autem. Provident ipsa esse in!
    </p>

    <p id="p4" class="even">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illo esse beatae labore quia qui
        voluptatibus ab cum
        nisi ipsa. Cupiditate consequatur voluptatum quo praesentium distinctio autem. Provident ipsa esse in!
    </p>
</body>

</html>
```