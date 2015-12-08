# Introduction:

For the purpose of this assignment I have used graph editor software named [yEd Graph Editor](https://www.yworks.com/products/yed). yEd Graph Editor is a free software for all major computer platforms which provides its users the possibility to generate and create high-quality diagrams, and if needed to manually edit and modify them. 

# Data Gathering and preprocessing

The data set analyzed here is a work compiled by M. Newman (2006) in May 2006 and it represents the data on coauthorship network of scientists who work and execute experiments in the field of network theory. The dataset itself comes in a form of a file with .gml extension.

yEd Graph Editor natively supports .gml extension, so there was no need for preprocessing and no troubles occurred, while opening up a graph in the software. 

# Visualisations

After the dataset was successfully loaded, all the information appeared on the screen. The first outcome was not very representative. Thus additional modifications were needed. 
![Figure 1]()

At first I tried to create a **hierarchical layout** with primary orientation going from top to bottom. However, soon it became clear, that this type of layout might not be very suitable for the type of data analyzed. 

![Figure 2]()

For this reason I have also tried to create a **directed tree** layout, which looked a bit different, but still did not provide enough visual feedback. 

![Figure 3]()

After experimenting with several other layouts, I have found **circular layout** to work best for the type of data which represents networks. Through this type of graph it was possible to observe a *big picture* clearly, and indicate distinct network groups. Those groups represented scientists and authors, who seem to work a lot with each other or simply cite each other. 

![Figure 4]()

For example, from the outset my attention was immediately caught by this very dense circle. This group was separated and featured a lot of tight interlinkages. 

![Figure 5]()

What was interesting, is that selecting a particular node in  yEd Graph Editor would show its own ego networks on the left sidebars under the window area called «neighborhood». 

![Figure 6]()

yEd Graph Editor provides the possibility not only to show graphs, but also analyze them. However, analysis featured might be limited compared to other software products, the primary focus of which is network analysis. One of the available analysis features is the calculation of graph’s centrality measures. It can be found under the section called *tool* in the top bar menu of the main window. I have decided to use «number of connected edges» as a parameter for a centrality measure. In addition to that, it was possible to colorize and change the size of nodes, according to the value of calculated measures.

![Figure 7]()

 I have used orange color and a bigger node size, in order to highlight those nodes who scored high on the measurement calculation process. 

![Figure 8]()

It appears that scientist with surname written as Barabasi has the biggest amount of outgoing and ingoing citations in total. Another remarkable node has lead to Newman, the actual author of the explored dataset.

![Figure 9]()
![Figure 10]()

Later on I have changed the parameter of centrality measure to the ingoing citation only. However, it did not make a lot of differences to the existing network leaders. On the other hand, remarkably the previously outlined distinct dense science group changed dramatically. It was clearly possible to observe, that only half of the researchers in the circles get a lot of incoming citations. The test of the outgoing citations has shown, that another half of this groups is the one who cites the first half. 

![Figure 11]()
![Figure 12]()

After that I have tried to use an experimental feature called «one-click-layout». This function tries to identify the best possible layout for the provided type of data and after that generates a suitable graph. 

![Figure 13]()

Different setting of algorithms used provided me different results. Even running the same algorithm over and over again will make slight changes to the graph. 

![Figure 14]()
![Figure 15]()

# Conclusion

Generaly, I found yEd Graph Editor to be a good tool for the start of network analysis. However, it might be not so robust and does not feature many analysis tools compared to other existing solutions, like [Gephi](http://gephi.org/). However, at the time of writing, Gephi software for mac platforms was still in beta development and did not work properly all the time, which made the product itself redundant. 




M. E. J. Newman, Phys. Rev. E 74, 036104 (2006).