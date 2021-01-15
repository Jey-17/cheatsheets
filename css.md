# CSS

### selectors: 

Are for applying specific styles to an HTML element. Mostly, its best to use classes in CSS.

```CSS
header {
    /* These styles will apply to every <header> on the page */
}

.class {
    /* Each element like: <div class="class"></div> */
}
```


### units 

There are different units that can be used in CSS:

```css
.class{
    height: 100px; /* pixel units */
    height: 100%; /* percentage of the parent element */
    height: 100vh; /* percentage of the entire window */
    height: 1rem; /* responsive to the font-size of HTML */
}

```

### some common CSS rules:

```css
.class{
    /* basic styles */
    height: 1rem;
    width: 1rem;
    margin: 1rem 2rem 1rem 2rem;  /* spacing OUTSIDE the element; if one, all; if two, top-bottom and left-right, if four, top, right, bottom, left */
    margin-right: 2rem; /* spacing just to the right */
    padding: 1rem; /* spacing INSIDE the element */

    background: magenta;
    background: #FFAAFF; /* hexadecimal */
    background: rgba(100, 0,1 00, 0.5); /* red, green, blue, transparency (1-0.0) 
}