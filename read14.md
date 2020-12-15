
# pyplot

* pyplot provides a convenient interface to the matplotlib object-oriented plotting library

![](https://matplotlib.org/_static/logo2_compressed.svg)

|Method|	Usage|
|---------|----------|
|plt.annotate|	Annotate some points|
|plt.gca().spines|	Moving spines|
|plt.legend|	Adding a legend|
|plt.plot(X, C, color='', linewidth= , linestyle='') |Changing colors and line widths|
|plt.xlim() , plt.ylim()	|Setting limits|
|plt.xticks() , plt.yticks()	|Setting ticks and tick labels|
|np.linspace	|Get the data for the sine and cosine functions|
|plt.figure(figsize=( , ), dpi=)|figure|

**Simple plot**
In this section, we want to draw the cosine and sine functions on the same plot. Starting from the default settings, we'll enrich the figure step by step to make it nicer.

**Instantiating defaults**
* we've instantiated (and commented) all the figure settings that influence the appearance of the plot. The settings have been explicitly set to their default values, but now you can interactively play with the values to explore their affect

**Subplots**
* With subplot you can arrange plots in a regular grid. You need to specify the number of rows and columns and the number of the plot. Note that the gridspec command is a more powerful alternative.

**Axes**
* Axes are very similar to subplots but allow placement of plots at any location in the figure. So if we want to put a smaller plot inside a bigger one we do so with axes.

**Ticks**
* Well formatted ticks are an important part of publishing-ready figures. Matplotlib provides a totally configurable system for ticks.

