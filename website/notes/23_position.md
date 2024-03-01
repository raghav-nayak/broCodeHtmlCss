`position`
- relative -> positioned relative to where it normally should be

```css
position: relative;
top: 100px; /* pushed downwards 100px*/
left: 100px; /* pushed right 100px */
---
top: -100px; /* pushed upwards 100px */
left: -100px; /* pushed left 100px */
```

<br>

- fixed -> positioned relative to the viewport; good for banners

```css
position: fixed;
right: 0px;
bottom: 0px;
```

<br>

- absolute -> positioned relative to nearest ancestor
```css
position: absolute;
right: 50px;
bottom: 50px;
```

if div is within another div, the inner div(fixed) will move relative to outer div(relative/fixed).

```css
position: sticky;
    top: 0px;
```

<br>

- sticky -> positioned based on scroll position
similar to sticky with scrollable option


<br>

- static -> default position for an element
default position


<hr>

```css
#box1 {
    width: 200px;
    height: 200px;
    background-color: aquamarine;

    /* position: relative; */
    /* top: 100px; /* pushed downwards 100px */
    /* left: 100px;  /* pushed right 100px


    /* position: absolute;
    right: 0px;
    bottom: 0px; */

    /* position: sticky;
    top: 0px; */

    position: static;

    
}

#box2 {
    width: 100px;
    height: 100px;
    background-color: red;
    position: static;
    right: 50px;
    bottom: 50px;
}

```