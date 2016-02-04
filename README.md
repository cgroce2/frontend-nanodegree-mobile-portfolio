## Website Performance Optimization portfolio project

My project for the Udacity Website Performance Optimization course.

I completed this project using techniques to optimize HTML, CSS and JavaScript in order to improve website page speed and user experience for both mobile and desktop.

Goal of Part 1:

1. Identify and perform optimizations to achieve an improved PageSpeed score using PageSpeed Insights.
2. Identify and perform optimizations impacting content efficiency.

To increase the PageSpeed score here are some of the optmizations I made:
Loaded JavaScript files asynchonously
Used a media query for print.css
Optimized image sizes
Used Grunt to help remove unnecessary css, minification of files and inlining of css.



Goal of Part 2:

1. Identify and perform optimizations ensuring a consistent frame rate at 60fps when scrolling in pizza.html
2. Identify and perform optimizations impacting content efficiency.

To hit 60 fps I primrily made optimizations to main.js to remove unnecessary work from 'for' loops and wrote a new function. determineNewWidth(size), to do a much simpler width calculation when resizing pizzas.  I also optimized image sizes and used Grunt to help remove unnecessary css, minification of files and inlining of css. 
