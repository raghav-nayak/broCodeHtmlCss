pagination
- method by which a document is separated into pages, and numbers are given
- limiting the results

we can use javascript to move forward and backward. But in this example, we are just using html pages.

<hr>

**style**
```css
.pagination {
    text-align: center;
}

.pagination a{
    color: black;
    text-decoration: none; /* remove underline */
    padding: 8px 15px;
    display: inline-block;
}

.pagination a.active {
    background-color: rgb(52, 210, 52);
    font-weight: bold;
    border-radius: 5px;
}

.pagination a:hover:not(.active) {
    background-color: grey;
    border-radius: 5px;

}
```


**page 1**
```html
<div class="pagination">
        <a href=""> < </a> 
        <a href="28_pagination.html" class="active"> 1 </a>
        <a href="28_pagination_2.html"> 2 </a>
        <a href="28_pagination_3.html"> 3 </a>
        <a href="28_pagination_4.html"> 4 </a>
        <a href="28_pagination_5.html"> 5 </a>
        <a href="28_pagination_2.html"> > </a>
    </div>
```

**page 2**
```html
    <div class="pagination">
        <a href="28_pagination.html"> < </a> 
        <a href="28_pagination.html"> 1 </a>
        <a href="28_pagination_2.html"  class="active"> 2 </a>
        <a href="28_pagination_3.html"> 3 </a>
        <a href="28_pagination_4.html"> 4 </a>
        <a href="28_pagination_5.html"> 5 </a>
        <a href="28_pagination_3.html"> > </a>
    </div>
```

**page 3**
```html
    <div class="pagination">
        <a href="28_pagination_2.html"> < </a> 
        <a href="28_pagination.html"> 1 </a>
        <a href="28_pagination_2.html"> 2 </a>
        <a href="28_pagination_3.html" class="active"> 3 </a>
        <a href="28_pagination_4.html"> 4 </a>
        <a href="28_pagination_5.html"> 5 </a>
        <a href="28_pagination_4.html"> > </a>
    </div>
```

**page 4**
```html
    <div class="pagination">
        <a href="28_pagination_3.html"> < </a> 
        <a href="28_pagination.html"> 1 </a>
        <a href="28_pagination_2.html"> 2 </a>
        <a href="28_pagination_3.html"> 3 </a>
        <a href="28_pagination_4.html" class="active"> 4 </a>
        <a href="28_pagination_5.html"> 5 </a>
        <a href="28_pagination_5.html"> > </a>
    </div>
```

**page 5**
```html
    <div class="pagination">
        <a href="28_pagination_4.html"> < </a>
        <a href="28_pagination.html"> 1 </a>
        <a href="28_pagination_2.html"> 2 </a>
        <a href="28_pagination_3.html"> 3 </a>
        <a href="28_pagination_4.html"> 4 </a>
        <a href="28_pagination_5.html" class="active"> 5 </a>
        <a href="28_pagination_5.html"> > </a>
    </div>
```