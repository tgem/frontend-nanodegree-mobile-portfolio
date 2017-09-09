## Website Performance Optimization portfolio project

To start, simply open index.html in the browser and than click on the pizzeria to see the optimized version of Cam's pizzeria.

The following optimizations have been performed:

**index.html**

* The analytics script is now loaded asynchronously
* print.css is loaded with media="print" so that it's only render-blocking for printing
* web font usage has been removed

**Cam's pizzeria**

* Forced synchronous layout was removed by querying offsetWidth only outside of the loop
* Scrolling was made more performant by performing sine calculations outside of the loop over all .mover elements
