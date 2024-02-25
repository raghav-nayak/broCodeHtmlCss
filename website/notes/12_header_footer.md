- semantic tags 
- describe their meaning to both browser and the users
- help us to organize the content
- useful to apply css properties within the these containers

`header`
- used to apply introductory content at the top of the page

`footer`
- used to show concluding content at the bottom of the page

`main`
- the actual page content goes here

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <header style="background-color: mediumpurple;">
        <h1> Welcome to Lord of the code website </h1>
        <a href=""> Home </a>
        <a href=""> About Us </a>
        <a href=""> Products </a>
        <a href=""> Contact Us </a>

    </header>

    <main>
        <h4> Some content </h4>
        <img src="images/elton_john_rocket_man.jpg" alt="rocket man cover image">
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime ut temporibus quidem a voluptas dicta
            adomnis hic repellendus, atque quos ipsa voluptatibus nostrum eligendi? Nobis dolore cupiditate natus! Eum!
        </p>
    </main>

    <footer style="background-color: mediumpurple;">
        <hr>
        author: Lord of the code <br>
        &copy; copyright not reserved <br>
        <small><a href=" mailto:support@lotc.com">support@lotc.com</a></small>
    </footer>
</body>

</html>
```
