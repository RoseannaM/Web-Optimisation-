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
I inlined the css.

I added a script that adds the css for the google font after the page has loaded. 

####Part 2: Optimize Frames per Second in pizza.html

I changed the number of pizza images being rendered from 200 to 34.This had a significant impact on the fps.
The pizzeria image was unnecessarily large so I resized it and optimised it for the web.
