Assignment #2: Cleaning and EDA (Due Feb 16, 11:59 PM)
===============================

In this assignment you will:

1.  Statistically assess the quality of the data, justify the
    data-cleaning logic, and explain/analyze the
    features/statistics/target needed for the replication (report).
    
2.  Develop and justify data cleaning (code).

* * * * *

### Part 1

* (Cleaning) Perform an initial EDA to statistically assess the quality of the data
and its appropriateness for addressing the problem at hand, **justifying
data cleaning logic**. This will likely address issues with image quality, resolution, 
color depth (rgb vs. grayscale), as well as distinguishing between the different
classes of images found in the catalogue raisonneé (paintings and drawings) so that
you only use the images most relevant to an quantitative analysis of visual style.
Tie these issues to their possible impact on eventual results. Some possible 
questions to address include: 

	- The catalogue raisonneé contains images of paintings and drawings, stored as
	color and grayscale images. Can you quantitatively, automatically distinguish
	between these two classes of images? If so, on the basis of what features?
	- Images are stored at a variety of resolutions. What is a threshold/cutoff of
	minimum resolution necessary to participate in this analysis? At what point 
	does imagery become too indistinct/low-information content to be of use in 
	assessing visual style?
	- Given these decisions, what portion of Mondrian's published catalogue 
	raisonné should reasonably be included in your analysis of his stylistic
	development.

Describe your decisions about data inclusion and justify your choices.

* (Descriptive Stats) Statistically summarize the relevant, cleaned attributes and 
derived features (e.g. in univariate and bivariate analyses) for Mondrian's 
paintings. This includes metadata about paintings (date made, size, medium),
average hue, brightness, saturation, and edge scores, and others. You can include
interactive visualizations (bokeh) as part of these descriptive analyses of the 
features of the images and the population as a whole.      

* (Working with Manovich Style-Space Plots) Calculate and plot the distribution of
Mondrian paintings in a variety of style spaces following Manovich's methods. 
The analysis should describe the tradeoffs with respect to choice of visual features. 
For instance:
    - Plot single measures vs. time. Can you generalize about a trajectory of visual 
    evolution in Mondrian's work?
    - Plot simple bivariate relationships (brightness vs. hue, brightness vs. saturation,
    edge score vs. saturation, etc.) and describe what relationships we can see in these
    plots. 
    - Consider multiple features at once (n>2) as high-dimensional descriptors of
    Mondrian's paintings. Use PCA or UMAP or t-SNE to plot these high dimensional features
    on 2d graphs.
        - Can you identify distinct clusterers of work in this high dimensional feature
       space? (Use k-means, affinitey clustering, or another technique to cluster)
       - If so, what is the signifcance of these clusters?
    - Which combinations of features, approaches, techniques are most appropriate for
    analyzing an evolution of abstraction.

* (Abstraction Score) Perform the artnome (Jason Bailey's) abstraction analysis
  (based on complexity score) on your downloaded and cleaned data of Mondrian's
  paintings. Include an introduction to the technique and interpret the results.
  (In Assignment #3 you will carefully address the shortcoming of this result.)
  	- Compare your work to the publish results on artnome via visual comparison.
	- Analyzed where your workflow may have departed from Jason Bailey's.

### Part 2

Develop code to clean data (as defined and justified in Part 1),
create the features for the replication, and compute the statistics
for the report. Such code should conform to the methodology portion
of the course (e.g. using the project template).

In particular, your project should have a `run.py` with the following
targets:
1. `data` creates the data needed for analysis.
2. `process` cleans and prepares the data for analysis (e.g. cleaning
   and feature creation).
3. `data-test` ingests a small amount of *test data* (that `process`
   can then process).

