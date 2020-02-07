# Week 5: Visualization, Clustering, Dimensional Reduction - Domain Specific Techniques II

## Topics

* Discuss basic image features; introduce higher-order image features; introduce clustering, dimensional reduction, visualization techniques; talk about issues of visualizing visual cultural analysis.

### In-Class Activities

* Look at results of preliminary data analysis (brightness, hue, variance, edge score)
  * Which images should we include in our analysis of style?
  * What are the consequences of eliminating data from our replication?
* Look at high res image plots (Manovich) on media commons.
* What additional measures did Manovich or Bailey (artnome) employ?
* Look at the [bokeh notebook](notebooks/bokeh.ipynb)
* Look at dimensional reduction, clustering, and visualization notebook (TK)

## Assigned Readings

The basic metrics we will implement were discussed in these readings:
* [Quantifying Abstraction In Art: Mondrian](https://www.artnome.com/news/2018/4/11/quantifying-modrian-journey-to-abstraction), Jason Bailey, Artnome, 2018,  
* [Mondrian vs Rothko: footprints and evolution in style space](http://lab.softwarestudies.com/2011/06/mondrian-vs-rothko-footprints-and.html), Lev Manovich et. al, Software Studies Lab, 2011
* [Reply to Mondrian vs Rothko: footprints and evolution in style space](https://web.archive.org/web/20120717071426/http://iwasnteventhere.tumblr.com/post/7882377942/reply-to-mondrian-vs-rothko-footprints-and-evolution), Ryan Anderson, Tumblr via wayback machine, 2012.

Additional readings TK.

### Homework

Please look through the following clustering/visualization and advanced visual features code examples, and then create your own notebook to attempt the following:

* Replicate some Manovich Rothko v. Mondrian plots that incorporate Bokeh tooltips to preview images when you hover: 
  * Create a mean brightness vs. mean saturation plot
  * Plot brightness vs. saturation, labelled with creation date (size or color)
  * Plot the images in time with date (x) vs. saturation space (y)
  * Plot a > 2 dimensional feature space on a 2d plane using PCA, UMAP, t-SNE or some other dimensional reduction technique.
* Replicate the above as static high-res image outputs where we plot each point as an image rendered to the canvas, rather than a point on a scatter plot.

Bring your jupyter notebooks and rendered results to class for Wed 2/12 Discussion.
