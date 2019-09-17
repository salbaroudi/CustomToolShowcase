## Purpose:

This project collects custom visualizations I have developed, to help me make sense of the data I encounter. I try to meet the following principles when I produce such examples:

1) Maximal Information Density (for datums in plot).

2) Avoidance of Scroll-Bar Hell (if possible).

3) Representing numerical relations and concepts with a diversity of visual marks (lines, areas, boxes...) and properties (color, shape, line intensity). Properties shown should have independent representations, that are clearly distinct.

4) Image generation method should be sufficiently generalized, to be used in a wide variety of contexts.



## BoxplotBlast() Example:

This code takes a DataFrame as an input, picks out all numerical columns, and then displays stacked 
boxplots for each numerical column. Because some numerical columns can have large tails of outliers,
BoxPlotBlast clips the visualizations, indicating outlier tails or max/min values (with coloured lines).

For the dataset below, we see a lot of variation in outlier tails and bounds. Data scaling might also be required, depending on the modelling applcation.

![bpblast][bpb]


## Timeline Visualization Example:

For large datasets with time-series data, an Analyst may wonder about gaps in the data itself. This visualization uses a heatmap to show the number of records in a given time window. It quickly shows if records or missing, or if the number of records per unit time is constant.

We can see clearly in the example below, that some data for a given day is completely missing. For other days, the number of records is heavy/light (not constant).

![timegaps][timeblocks]


[bpb]: /web/img/bpblast.png
[timeblocks]: /web/img/timegaps.png
