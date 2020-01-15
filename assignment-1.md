Assignment #1: The Data (Due Date: Jan 24th, 11:59 PM)
=======================

In this assignment, you will:

1.  Write a survey of the data and the context in which it was created (report).

2.  Describe and justify the data ingestion process in part 3 (report).

3.  Develop code for ingesting and storing the data for later use
    (code).
    
The report portion of the assignment should be written in markdown,
saved as a pdf, and uploaded to Gradescope.

The data ingestion code should be submitted to Gradescope as a
programming assignment.

* * * * *

### Part 1

Introduce the problem being investigated and describe the data being 
used to approach the problem. That is, describe the problem of 
Quantifying Abstraction in Art, referring to the 
[Mondrian post](https://www.artnome.com/news/2018/4/11/quantifying-modrian-journey-to-abstraction)
for specifics and to assigned articles for context.

The data you will use in the replication consist of:
1. Images of Mondrian paintings from the Artnome website, Mondrian catalogue
   raisonné website, or other online sources that *you* will collect.
2. Metadata for collected images including title, date, dimensions.

Address the appropriateness of the data design and collection:

-   Why is the data is appropriate to address the problem? 

-   What are the potential shortcomings of the data for addressing the problem? 

-   What data have been used to address this problem in the past? Or, how has this
   problem been approached in a non-quantitative manner? (Historical context)

Summarize relevant details of the data generating process, describing
the population that the data represents, whether that population is
relevant to the question at hand, while addressing possible questions
of data reliability.

The material in this section should be informed by the listed
background readings and the introduction/data explanation sections of
the Mondrian blog post. Manovich, Carey, and Wang's 
[http://lab.softwarestudies.com/2011/06/mondrian-vs-rothko-footprints-and.html](Mondrian vs. Rothko) 
paper is a valuable second key reference, though the image features are
slightly more simplistic.

### Part 2

Describe the data ingestion process. This description should:

-   Specify from where the data originates, addressing legal issues
    pertaining to access.

-   Lay out the schema and justify the decisions (what's the unit
    corresponding to an observation? What are the storage
    considerations?)

-   Address the applicability of the pipeline to similar data sources
    you might anticipate using (what might those be?).

### Part 3

In a private GitHub repository for your project, structured according
to the methodology portion of the course, create a data ingestion
pipeline for the result-replication project. The pipeline should:

-   Write code that creates a list of Mondrian paintings that will
    provide the basis for our time series of art style.
    
-   Given a painting on one of the online collections 
    ([Artnome](https://knownwork.knack.com/artnome#artworks-piet-mondrian/), 
    [Catalogue Raisonné](http://pietmondrian.rkdmonographs.nl/) or other),
    download a full resolution image and accompanying 
    bibliographic/authorship information. 
    
-   Given a directory containing images and metadata, organize it
    on disk (justify your processing in part 2). The data source 
    should be specified as configuration.

-   Store the data according to your designed schema, taking care to
    appropriately type the data and implement the best storage design.

-   The stored data should be in a form most appropriate for
    assessment and cleaning (EDA).
