
check [fontawesome.com](fontawesome.com) for icons. 
You can customize these icons.

You need to get the kit after logging in. After that you can search for your icon and use them using `<i>` tag

```html
<head>
    <script src="https://kit.fontawesome.com/88f05daeb4.js" crossorigin="anonymous"> </script>
</head>

<body>
    <div class="icons">
        <a href="">
            <i class="fa-solid fa-house fa-5x"></i>
        </a>
        <a href="https://twitter.com/">
            <i class="fa-brands fa-twitter fa-5x"></i>
        </a>
        <a href="https://youtube.com">
            <i class="fa-brands fa-youtube fa-5x"></i>
        </a>
        <a href="https://tiktok.com/">
            <i class="fa-brands fa-tiktok fa-5x"></i>
        </a>
    </div>
</body>
```

<br>
<hr>
<br>

```css
.icons {
    text-align: center;
}

.icons a {
    text-decoration: none;
    margin-right: 20px;
}

.fa-solid.fa-house {
    color: grey;
}

.fa-solid.fa-house:hover {
    color: black
}

.fa-brands.fa-twitter {
    color: rgb(0, 119, 255);
}

.fa-brands.fa-twitter:hover {
    color: black
}

.fa-brands.fa-youtube {
    color: red;
}

.fa-brands.fa-youtube:hover {
    color: black;
}

.fa-brands.fa-tiktok {
    color: pink;
}

.fa-brands.fa-tiktok:hover {
    color: black;
}
```