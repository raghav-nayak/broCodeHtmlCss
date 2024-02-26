`font-family`
- always give backup font
`font-size`
- px -> pixel
- em -> 1em = 100%
`font-weight`
- bold
`font-style`
- normal, italic, 


### google fonts
- check [google font site](https://fonts.google.com/)
- either you can use them as a link
	- e.g.
```html
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Sono:wght@200..800&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Sono:wght@200..800&family=Spline+Sans+Mono:ital,wght@0,300..700;1,300..700&display=swap" rel="stylesheet">
```

- or download them and store them in your code base
```css
@font-face {
    src: url(fonts/SplineSansMono-VariableFont_wght.ttf);
    font-family: Spline;
}

p{
    font-family: Spline,"lucida console", "courier new";
}
```

<hr>


html file
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> fonts demo </title>
    <link rel="stylesheet" href="15_style_fonts.css">

    <!-- <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Sono:wght@200..800&display=swap" rel="stylesheet">
    <link
        href="https://fonts.googleapis.com/css2?family=Sono:wght@200..800&family=Spline+Sans+Mono:ital,wght@0,300..700;1,300..700&display=swap"
        rel="stylesheet"> -->
</head>

<body>
    <h1> Lord of the code </h1>

    <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Saepe soluta harum, maiores architecto corrupti
        facilis, beatae, accusantium similique odio consectetur et iusto. Praesentium eos fuga natus ex nobis error
        esse!
    </p>

</body>

</html>
```

css file
```css
@font-face {
    src: url(fonts/Sono-VariableFont_MONO\,wght.ttf);
    font-family: Sono;
}

@font-face {
    src: url(fonts/SplineSansMono-VariableFont_wght.ttf);
    font-family: Spline;
}

h1 {
    font-family: Sono, Verdana, Arial, Helvetica, sans-serif;
}

p{
    font-family: Spline,"lucida console", "courier new";
    font-size: 1em;
    font-weight: bold;
    font-style: italic;
}
```
