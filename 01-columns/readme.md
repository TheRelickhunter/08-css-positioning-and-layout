# 01-columns-columns

### Author details
##### #24 Andrea Zappa
***

<h4>Requirements</h4>

- Create a page with
1. Header, footer, sidebar, and two main columns
- Header and footer
2. Should stay in place when the page scrolls
- The sidebar and two columns
3. Should fill the rest of the page, vertically and horizontally
4. Should expand proportionally when window is resized
- One of the columns should contain
5. An image and a caption placed on top of the image
- Use semantic HTML5 elements
- Fill the page with meaningful content
    
<h4>My solution</h4>

1. Done.
2. ```<header>``` is fixed with ```position:fixed``` .
3. I use the viewport width measure unit in the width of sidebar and columns and ```float:left``` which lay out the page according the model given. 
   Choosing the viewport width in addition to float will not put any block element one below other as the default block element do.
5. A ```figure``` positioned relative to its container remain even in the flow, and allow the ```figcaption``` be placed absolute on top, by taking the top-left coordinates referring to the ```figure``` top-left corner.