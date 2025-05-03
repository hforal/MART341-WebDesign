1. 3+ Pages
The site is built with four distinct HTML files—index.html (Home), destinations.html (Destinations), activities.html (Activities), and interactive.html (Interactive Map)—all sharing the same “Explore America” branding, typography, and color palette. Each page’s <nav> bar includes links to the other three (plus a dropdown for the Interactive Map), ensuring that users can move seamlessly from one page to another without broken links or inconsistent menus.

2. Framework Integration
We’ve included Bootstrap 5 via CDN in every page’s <head> (<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css">), giving us access to its responsive grid, navbars, utility classes, and JavaScript components. This provides a solid foundation for mobile‑first layouts and consistent spacing, alignment, and breakpoints across the site.

3. Framework Styling Elements
On top of Bootstrap’s core, we use its navbar component for the top menu, grid classes (.row / .col-md-4) for our card layouts, and card components for the Destinations and Activities entries. Buttons (.btn .btn-primary) and utilities (like .text-center, .shadow-sm) come straight from Bootstrap, ensuring visual consistency while reducing custom CSS.

4. HTML5 Canvas
The interactive.html page includes a <canvas id="mapCanvas"> element sized via CSS to fill up to 800×600 px. We then draw a map image behind the scenes, either by setting it as the canvas background or by loading a hidden <img> and painting it onto the canvas, demonstrating use of HTML5 Canvas for custom graphics.


5. JavaScript Functionality
In interactive.html, a small script waits for the map image to load, then draws it into the canvas context. We attach a click event listener to the <canvas> so that whenever a user clicks, the script draws a colored marker (a filled and stroked circle) at the click coordinates. This interactivity shows how JavaScript can dynamically modify the canvas and respond to user actions.