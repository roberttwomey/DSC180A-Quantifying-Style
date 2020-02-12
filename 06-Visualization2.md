# Week 6: Visualization cont.: Dimensional Reduction, Clustering - Domain Specific Techniques II

## Topics

* Introduce dimensional reduction techniques; discuss clustering; talk about issues of visualizing visual cultural analysis.

### In-Class Activities

* Look at high res image plots (Manovich) on media commons.
* What additional measures did Manovich or Bailey (artnome) employ?
* Look at the dimensional reduction notebook ([dimensional_reduction.ipynb](notebooks/dimensional_reduction.ipynb))
* Discuss clustering.

## Assigned Readings

The basic metrics we will implement were discussed in these readings:
* [Quantifying Abstraction In Art: Mondrian](https://www.artnome.com/news/2018/4/11/quantifying-modrian-journey-to-abstraction), Jason Bailey, Artnome, 2018,  
* [Mondrian vs Rothko: footprints and evolution in style space](http://lab.softwarestudies.com/2011/06/mondrian-vs-rothko-footprints-and.html), Lev Manovich et. al, Software Studies Lab, 2011
* [Reply to Mondrian vs Rothko: footprints and evolution in style space](https://web.archive.org/web/20120717071426/http://iwasnteventhere.tumblr.com/post/7882377942/reply-to-mondrian-vs-rothko-footprints-and-evolution), Ryan Anderson, Tumblr via wayback machine, 2012.

Dimensional Reduction Techniques: 
- t-Distributed Stochastic Neighbor Embedding (t-SNE) https://lvdmaaten.github.io/tsne/
  - particularly [Visualizing Data using t-SNE](https://lvdmaaten.github.io/publications/papers/JMLR_2008.pdf)
- Uniform Manifold Approximation and Projection (UMAP) for Dimension Reduction [https://arxiv.org/abs/1802.03426](https://arxiv.org/abs/1802.03426)

### Homework

Using the clustering/visualization and advanced visual features code examples [dimensional_reduction.ipynb](notebooks/dimensional_reduction.ipynb), complete the discussion activity from next week:

* Replicate some Manovich Rothko v. Mondrian plots that incorporate Bokeh tooltips to preview images when you hover: 
  * Create a mean brightness vs. mean saturation plot
  * Plot brightness vs. saturation, labelled with creation date (size or color)
  * Plot the images in time with date (x) vs. saturation space (y)

* Extending Manovich: 
  * Plot a > 2 dimensional feature space (e.g. more than two features at once) on a 2d plane using PCA, UMAP, t-SNE or some other dimensional reduction technique. 
  * What are other visual features you could use?

Upload these results as link/pdf to the 2/12 google form:https://forms.gle/ro7dLqYHjixHtC9BA.

Next week Wed 2/19 we will discuss your Assignment 2 in class, including the results of the replication of artnome and Manovich, and possible ways to extend this work.

