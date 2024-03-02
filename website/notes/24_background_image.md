`background-image: url(image path)` -> add an image

`background-repeat: no-repeat;`
- if you take a high resolution image, it will go beyond the page
- if you take less resolution image, it will be repeated till it fills the page; to avoid this use `no-repeat`

`background-position: center;` -> horizontal alignment

`background-attachment: fixed;` -> fixed or scrollable
 fixed with regard to the viewport ('fixed') 
 or scroll along with the element ('scroll') 
 or its contents ('local')

`background-size: cover;` -> image size
cover -> fill the image
contain -> crops the big image
auto -> original


<hr>


```css
body {
    background-image: url(./images/netflix.jpg);
    background-repeat: no-repeat;
    background-position: center; /* horizontal */
    background-attachment: fixed;
    background-size: cover; /* to fit the image in the screen */
}

```
