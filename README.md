## Installation

1. Change directory to the <strong>dist</strong> folder
2. Run the command in terminal to tart server
```
$> python -m SimpleHTTPServer 8080
```
3. Run the command in terminal to set up online server after installing ngrok
```
$> ./ngrok http 8080
```

## Steps Taken for Optimization
### Part 1
1. Split CSS files
2. media query on CSS file links
3. used async on the link for google analytics
4. downloaded the first three images to ensure that the files were in local folders
5. resized the last image to 100px using grunt-responsive-images node tool
6. placed css into HTML under the style tag
7. deleted the Google font
8. used lossless compression for profile and pizza pictures to significantly lower image sizes

### Part 2

1. Used percentages for resizing the pizzas rather than changing the layout then adding style using a for loop
2. Cached the style so that the layout is changed outside the for loop and then the style is applied in bulk as a loop (used idea from provided website.)
3. moved ```var pizzasDiv = document.getElementById("randomPizzas");``` out of the for loop
4. added translateZ(0) to CSS
5. added cols and rows to make less than 200 pizzas in the background
6. changed querySelectorAll to getElementsByClassName
7. changed query to getElementById
8. moved ```var movingPizzas = document.querySelector("#movingPizzas1");``` out of for loop so the DOM selection is done once.  changed querySelector to getElementById.
9. added div end tag to ```<div class="container">```

## License
No License.
