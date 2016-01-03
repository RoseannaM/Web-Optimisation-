## Getting started

1. Clone the repo

1. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok http 8080
  ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! Optional: [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

**The optimized page is also hosted with firebase at this url:** [Page Hosted With Firebase](https://web-optimisation.firebaseapp.com/"Web-Optimisation")

##Optimizations Preformed

####Part 1: Optimize PageSpeed Insights score for index.html

Inlined the css.

Optimized the images for web. Resized them and compressed them.

Used the Web Font Loader script to avoid the font blocking the page.

####Part 2: Optimize Frames per Second in pizza.html

Changed the number of pizza images being rendered from 200 to 34.This had a significant impact on the fps.

Resized and optimised the pizzeria image as it was unnecessarily large.

Implemented _Use Strict_

Changed all instances of document.querySelector to getElementById.

Changed all instances of document.querySelectorAll to getElementByClassName.

####Part 3: Optimize Frames per Second for the Pizza resize time in pizza.html.

Put the array length in a variable at the start of the for loop so it would not calculate during each iteration.

Created a container var so it would no longer fetch HTML from the DOM during each iteration.


