## The things I improved...

On the index.html
1. On the index.html page I reduced the file size with third party programs to reduce loading speed.
2. I moved the files that were blocking the creation of the DOM to the bottom, load them asynchronously, or moved data to other files, for example, I inlined some of the css.
------------------------------------------------------------------------------------------------------------------------------
On the views section of this beautiful portfolio:

In the main.js I changed the following functions and made the following adaptations:
function rezise pizza:
1. Removed the determineDX function altogether. Values were staying the same. Changes are now based on the values in the sizeSwitcher function.
2. Changed the changePizzaSizes(size) function to iterate through the divs and change only the style.width based on the new value. I also put some variable creation outside the loop, saves memory.
3. Created a function isScroll to generate pizzas only when there is a scroll.
4. Created a function requestTick to check if there is a scroll change, if so the browser can update the pizzaPositions
5.  Therefore also the function updatePositions is slightly altered
6. The eventListener is changed so that we calculate the amount of pizza that can be on the screen and only print the pizza's nececarry

