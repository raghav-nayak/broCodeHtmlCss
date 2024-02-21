
https://www.youtube.com/watch?v=HGTJBPNC-Gw

HTML - Hyper Text Markup Language

CSS - Cascading Style Sheets

Most project return their home page as `index.html` 

We need live server extension on vscode.

`<!DOCTYPE html>` -> declaration that this is html 5 file.

most tags are a pair of tags.

headers
- 5 types from h1 to h5

paragraphs
- using `<p>`
- two paragraphs are separated by line breaks.
- even if your content spans over multiple lines(with line-breaks) within paragraph tag, it will show it in a single line.
- if you want to retain line-breaks , use `<pre>`(pre-formatted text) instead of `<p>`

`<br>` -> break; self closing tag
`<hr>` -> horizontal rule; self closing tag
`<!-- -->` -> comments; not displayed


```html
<!DOCTYPE html>
<html>

<head>
    <title>

    </title>
</head>

<body>
    <h1> This is an h1 heading </h1>
    <h2> This is an h2 heading </h2>
    <h3> This is an h3 heading </h3>
    <h4> This is an h4 heading </h4>
    <h5> This is an h5 heading </h5>
    <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Amet, reprehenderit? Minus voluptatem repellendus
        nulla quae nam natus assumenda voluptas quis neque vitae iure, dolore quod tempore dicta culpa quasi sapiente!
    </p>
    <br>
    <hr>
    <pre>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Amet, reprehenderit? Minus voluptatem repellendus


        nulla quae nam natus assumenda voluptas quis 
        neque vitae iure, dolore quod tempore dicta culpa quasi sapiente!
    </pre>

    <!-- this is a comment -->
</body>

</html>
```
