`border-style`
- solid
- dashed
- dotted
- hidden
- double
- inset -> with inner shadow
- outset -> with outer shadow
- ridge
- none
`border-width` -> thickness; e.g. 5px
`border-color` -> refer [color](obsidian://open?vault=Documents&file=Obsidian%20Vault%2F1%20Personal%2Ftechnical%2Fcourses%2FOther%20JS%2FBro%20Code%20-%20HTML%20%26%20CSS%20Full%20Course%2F14.%20colors)
`border-radius` -> rounded borders; max 20px

```css
h1 {
    border-style: solid;
    border-width: 3px;
    border-color: hsl(273,100%,55%);
    border-radius: 15px;
}
```


there is a shorthand to do border-style, width and color.
`border: 3px solid hsl(273,100%,55%);`

you have other properties like
`border-bottom`

```css
h1 {
    /* border-style: solid;
    border-width: 3px;
    border-color: hsl(273,100%,55%); */

    border: 3px solid hsl(273,100%,55%);
    border-radius: 15px;
}

p {
    border-bottom: 3px solid red;
    border-top: 3px solid blue;
    border-left: 3px dotted orange;
    border-right: 3px solid green
}
```
