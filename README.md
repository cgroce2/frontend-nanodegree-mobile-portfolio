## Website Performance Optimization portfolio project

My project for the Udacity Website Performance Optimization course.

I completed this project using techniques to optimize HTML, CSS and JavaScript in order to improve website page speed and user experience for both mobile and desktop.

Goal of Part 1:

1. Identify and perform optimizations to achieve an improved PageSpeed score using PageSpeed Insights.
2. Identify and perform optimizations impacting content efficiency.

To achieve this I performed the following optimizations / changes:

Loaded JavaScript files asynchonously, used a media query for print.css, used a smaller/optimized version of pizzeria.jpg, optimized image sizes, 
used uncss to remove any unnecessary CSS selectors, checked if any CSS selectors were unnecssary for above-the-fold content, added a src/ folder to contain pre-minified files.

Additionally, I started using Grunt to automate a number of the optimization tasks.

grunt-uncss - task for uncss, grunt-imageoptim - task for optimizing images, grunt-contrib-uglify - task to minify Javascript,
grunt-contrib-cssmin - task to minify css, grunt-inline - task to inline critical CSS and Javascript.

I also added a src/ folder to contain pre-minified files

I moved the development versions of the HTML/CSS/Javascript files into a src directory and src/css, src/js subdirectories. The grunt tasks automate the process of minifying CSS and Javascript (grunt-contrib-uglify & grunt-contrib-cssmin), inlining selected CSS and Javascript (grunt-inline) and moving the release files into their final locations.
Results:

1. Ultimately achieved a mobile PageSpeed Insights score of 96
2. Yay - 96 PageSpeed score -- Success!
3. An automated Grunt pipeline to easily make further optimizations.


Goal of Part 2:

Identify and perform optimizations ensuring a consistent frame rate at 60fps when scrolling in pizza.html
Time to resize pizzas is less than 5 ms in pizza.html shown in the browser console.
Identify and perform optimizations impacting content efficiency.


To achieve this I performed the following optimizations / changes:

Primary optimizations included changes to main.js to remove unnecessary work from 'for' loops, wrote a new function determineNewWidth(size) to do a much simpler width calculation when resizing pizzas,
used a smaller/optimized version of pizzeria.jpg, optimized image sizes, used uncss to remove any unnecessary CSS selectors.

Additionally, I used Grunt to more easily make optimizations.

grunt-imageoptim --> optimized images, grunt-uncss --> remove unnecessary CSS, grunt-contrib-uglify --> Minify Javascript, 
grunt-contrib-cssmin --> Minify CSS, Inlined a minified version of the critical CSS, grunt-inline --> automate inlining of CSS

I also added a src/ folder to contain pre-minified files

I moved the development versions of the HTML/CSS/Javascript files into a view/src directory and view/src/css, view/src/js subdirectories. The grunt tasks automate the process of minifying CSS and Javascript (grunt-contrib-uglify & grunt-contrib-cssmin), inlining the CSS (grunt-inline), inlining the HTML (grunt-contrib-htmlmin) and moving the release files into their final locations.

Results:

1. A consistent frame rate at or above 60fps when scrolling in pizza.html
2. An automated Grunt pipeline to easily make further optimizations.
 
