## The things I improved...

On the index.html
1. On the index.html page I reduced the file size of the images with third party programs to reduce loading speed.
2. I moved the files that were blocking the creation of the DOM to the bottom, load them asynchronously, or moved data to other files, for example, I inlined some of the css.
3. I also added css to the style.css so that the GPU will be used on the 'mover' class. The improves speed
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
7. I added strict mode to the main.js file so that my code is following the right protocols.

Running the code:

You can start the portfolio by launching the index.html file. This will provide you with a beautiful starting page for Cameron's portfolio. If you click on the pizza link it will direct you to the pizza shop page. Here you can see a number of pizza, depending on your screen size, moving around as you scroll.
If you go down the page a bit, or press the pizza button, you can choose a pizza size and the other pizza's will be changed to that size. Also note that random pizza's are generated each time you visit this shop's site.

