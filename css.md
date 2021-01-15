# CSS

### selectors

Are for applying specific styles to an HTML element. Mostly, its best
to use classes in CSS.

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


### some common CSS rules

```css
.class {
    /* basic styles */
    height: 1rem;
    width: 1rem;
    margin: 1rem 2rem 1rem 2rem;  /* spacing OUTSIDE the element; if one, all; 
    if two, top-bottom and left-right, if four, top, right, bottom, left */
    margin-right: 2rem; /* spacing just to the right */
    padding: 1rem; /* spacing INSIDE the element */
    border: 1px solid white; 
    border-radius: 100%; /* 100% will make a circle */

    /* colors */
    background: magenta;
    background: #FFAAFF; /* hexadecimal */
    background: rgba(100, 0,1 00); /* red, green, blue*/
    background: rgba(100, 0,1 00, 0.5); /* red, green, blue, opacity (1-0.0) */
    background: url(https://my.image.png);
    color: green; /* for text color */

    /* text */
    font-size: 1rem;
    font-family: Helvetica, Arial; /* can do list so if can't find, checks next */
    font-weight: bold; /* bold, normal */
    text-align: center;

    /* layouts */
    display: flex; /* flex, block, none */
    position: relative; /* or absolute. If "absolute" is used, then you can 
    also use "top," "left," "bottom," and "right" rules to position your 
    element precisely */
}
```


### hover 

```css
.class {
    background: white; 
}

.class:hover { /* styles change when you hover the element */
    background:blue;
}
```


### flexbox 

The best way to do layouts! 

```css
.class {
    display: flex;
    flex-direction: row; /* or column */
    align-items: flex-start; /* or "center," "space-between," "space-around," 
    or "flex-end" */
    justify-content: wrap;
}
```


### media queries 

Here is a standard responsive design media query setup. After putting this in 
your CSS, you are able to use `rem` units anywhere in your site, and they will
be automatically responsive. 

```css
/* mobile */
html {
    font-size:14px;
}

/* tablet */
@media only screen and (min-width: 480px) {
    html {
        font-size:16px;
    }
}

/* desktop */
@media only screen and (min-width: 768px) {
    html {
        font-size:18px;
    }
}

/* x-large */
@media only screen and (min-width: 1024px) {
    html {
        font-size:20px;
    }
}
```