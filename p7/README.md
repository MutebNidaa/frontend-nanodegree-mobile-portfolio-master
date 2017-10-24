frontend-nanodegree-mobile-portfolio-master
===============================

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.


### Getting started

#### Part 1: Optimize PageSpeed Insights score for index.html


Some useful tips to help you get started:

1. Check out the repository
1. To inspect the site on your phone, you can run a local server
  $> cd /path/to/your-project-folder

  $> python -m SimpleHTTPServer 8080

  ```
1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to the top-level of your project directory to make your local server accessible remotely.


  $> cd /path/to/your-project-folder
  $> ./ngrok http 8080

  ```
1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! Optional: [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

Profile, optimize, measure... and then lather, rinse, and repeat. Good luck!

#### Part 2: Optimize Frames per Second in pizza.html
@durant-udacity
Update README to describe part 2: pizzas

To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. You will find instructive comments in main.js. 

You might find the FPS Counter/HUD Display useful in Chrome developer tools described here: [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).

### What I did for index.html
1. OPtimize images
2. Minify CSS files and add in index.html
3. Minify Javascript files
4. Add async in <script src="http://www.google-analytics.com/analytics.js"></script>
5. Add async in  <script async src="js/perfmatters.js"></script>

### What I did for main.js
1. change document from (querySelector) to (getElementById) the function changeSliderLabel
2.  function changePizzaSizes creact naw array and variables outside the loop and creact two loop 
frist loop Iterates through pizza elements on the page and secand loop can be changes their widths
3. created pizzasDiv variable outside the loop 
4. function updatePositions created scrollTop and phase variable outside the loop

See live demo [here](https://rkrktktk15.000webhostapp.com/p7/p7/index.html)