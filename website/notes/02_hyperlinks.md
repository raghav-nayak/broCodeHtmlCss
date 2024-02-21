`<a href>`
- it is used for hyperlink any page 
- e.g. `<a href="https://google.com/">click me</a>`
<br>

`target`
- e.g. `target="_blank"` -> to open the page in new tab
- options are
	- `_self` 
		- default value
		- opens the linked document in the **same window or tab** as the current page.
		- useful for internal links that navigate within the same website.
	- `_blank`
		- the most common value and opens the linked document in a **new window or tab**
		- ideal for external links or content that shouldn't replace the current page.
	- `_parent`
		- opens the linked document in the **parent frame** of the current frame. 
		- Frames are rarely used in modern web development, so this value is less common. 
		- if the current frame has no parent, it acts like `_self`.
	- `_top`
		- opens the linked document in the **entire browser window**, effectively closing any existing frames and replacing them with the new content. 
		- not widely used but can be useful in specific situations, like opening a login page in a clean window.
<br>

`title`
- to add a text to show when you hover the link

we can use absolute and relative urls.
- absolute -> href="https://google.com/"
- relative -> href="lyrics.html"; this is another file in the same directory

you can send mail by using `href="mailto:test@example.com"`

```html
<!-- absolute link -->
<a href="https://google.com/" target="_top" title="Goes to Google">
	click me
</a>

<br>

<!-- relative link -->
<a href="lyrics.html">song lyrics</a>

<br>

<!-- send mail -->
<a href="mailto:test@example.com">email me</a>
```
