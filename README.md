## Website Performance Optimization portfolio project

To start, simply open index.html in the browser and than click on the pizzeria to see the optimized version of Cam's pizzeria.

The following optimizations have been performed:

**index.html**

* The analytics script is now loaded asynchronously
* print.css is loaded with media="print" so that it's only render-blocking for printing
* web font usage has been removed
* reference to pizza.jpg has been changed to a reference to a compressed 100x75px version of the image

**Cam's pizzeria**

* Forced synchronous layout was removed by querying offsetWidth only outside of the loop
* Scrolling was made more performant by performing sine calculations outside of the loop over all .mover elements
* replaced uses of querySelector by getElementById, querySelectorAll by getElementsByClassName
* during pizza creation, reference to pizzasDiv is acquired only once outside of the loop
* reference to movPizzas is acquired only once outside of the loop
* .mover class was given CSS properties translateZ and backface-visibility
