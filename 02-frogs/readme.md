# 02-alien-frogs

### Author details
##### #24 Andrea Zappa
***

<h4>Requirements</h4>

 Create a page full of all possible combinations of aline frogs
1. Frogs should fill the page from left to right
2. Frogs should wrap if there isn't enough space
3. All frogs should change their eye color to black when touched
4. The HTML should be valid and complete
5. In the readme.md explain your CSS code
6. Do all the work in CSS, the HTML should only include elements of this type:
```
<div class="frog type1 small">--</div>
<div class="frog type2 small">--</div>
<!-- etc... -->
```
<h4>My solution</h4>

1. Structure in HTML there's four types of frogs: 
   ```.frog green small``` , ```frog orange small```, ```frog orange big```, ```frog green big```
   Each of these elements has a float property to the left.
2. The ```float``` property give the required result by itself if the ```width``` is set so the left side of next element will be placed in that case to the right side of the current element, otherwise the next elements will overlaps the current elements similar to a stack unless a width is defined.
3. Thanks to the ```class``` attribute in HTML there's the possibility to build a sort of hierachy when applying a style, in facts offer me a great solution to solve that.
At the end of css file I've set many css selectors to every ```eye``` in any frog element styled with black background and white content when the mouse hover the entire frog, to do that:
```
.frog.green.big:hover .left-eye, 
.frog.green.big:hover .right-eye {
     background-color: black;
    color:white;
}
```
As usual it's interpreted from right to left so it mean "apply the background and color to the left an right eye when mouse is hovering the frog".