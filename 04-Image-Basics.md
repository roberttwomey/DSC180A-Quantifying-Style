# Week 4: Image Basics - Domain Specific Technique

## Topics

* Concluding Cultural Analytics Discussion
* Basics of image processing


### In-Class Activities

* Discuss responses to Manovich / Cultural Analytics Articles
* Look at image processing notebook.

## Assigned Readings

The basic metrics we will implement were discussed in these readings:
* [Quantifying Abstraction In Art: Mondrian](https://www.artnome.com/news/2018/4/11/quantifying-modrian-journey-to-abstraction), Jason Bailey, Artnome, 2018,  
* [Mondrian vs Rothko: footprints and evolution in style space](http://lab.softwarestudies.com/2011/06/mondrian-vs-rothko-footprints-and.html), Lev Manovich et. al, Software Studies Lab, 2011
* [Reply to Mondrian vs Rothko: footprints and evolution in style space](https://web.archive.org/web/20120717071426/http://iwasnteventhere.tumblr.com/post/7882377942/reply-to-mondrian-vs-rothko-footprints-and-evolution), Ryan Anderson, Tumblr via wayback machine, 2012.

### Homework

Please look through the following image processing code examples: [basic-image-stats.ipynb](notebooks/basic-image-stats.ipynb) and then create your own notebook to attempt the following: 

* Load a single Mondrian image
  * Compute resolution (pixel count), mean saturation, mean brightness.
  * Compute the grayscale variance (Value in the HSV image) for your painting. 
    * Compute the per-row grayscale variance, and average per-row.
  * Approximate an "edge score"
  * Implement all of the above as functions, you can use these later.
* EDA to assess the full set of images:
  * Plot histograms of the above stats (resolution, mean brightness, mean saturation, average per-row grayscale variance, and edge score) across your set of scraped images. 
  
Bring your jupyter notebook to class for Wed 2/5 Discussion.
