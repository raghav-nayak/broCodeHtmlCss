We can use 
- names
	- refer [link](https://developer.mozilla.org/en-US/docs/Web/CSS/named-color)
	- e.g. `color: tomato;`
- rgb
	- refer [link](https://www.google.com/search?q=color+picker+css)
	- e.g. `color: rgb(240, 252, 3);`
- hexadecimal
	- e.g. `color: #03fc28;`
- hsl
	- **h**ue
		- a degree on the color wheel from 0 to 360. 
		- 0 is red, 
		- 120 is green, and 
		- 240 is blue.
	- **s**aturation
		- a percentage value.
		- 0% means a shade of gray, and 
		- 100% is the full color.
	- **l**ightness
		- Lightness is also a percentage value. 
		- 0% is black, and 100% is white.
	- e.g. `color: hsl(321, 54%, 43%)`

```css
body {
    background-color: slategray;
}

#p1 {
    color: tomato
}

#p2 {
    color: rgb(240, 252, 3)
}

#p3 {
    color: #03fc28;
}

#p4 {
    color: hsl(321, 54%, 43%)
}
```