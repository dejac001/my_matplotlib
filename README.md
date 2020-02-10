# my_matplotlib
Tips and tricks with matplotlib that I found useful during my PhD

matplotlibrc
============
I recommend making one for each journal submission,
allowing you to toggle options specific for each journal.


plots with error bars
=====================
*example to be added later*
I don't like matplotlib defaults for error bars.
I like to have the symbols on top of the error bars,
and I only want to see error bars that are outside of the symbol.
To do this, I make layered plots using *zorder*.
On the bottom layer I plot the error bar using the *errorbar* method.
Above that layer, I plot white symbols of the same symbol type
to hide the error bars behind.
Above that layer I plot the actual symbols, and I add the legend key
on this layer too.