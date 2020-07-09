+++
title = "Tutorial 14"
description = ""
weight = 15
+++
{{< lead >}}
<br/>


Welcome to the fourteenth tutorial in the InterMine python tutorial series! With the great need for data visualisation in the present world, we have introduced a few visual features to InterMine as well. This tutorial will have details of how we can visualise the data using the Python client.

This feature of the Python Client is supported only on Python versions >= 3.6 because of the dependencies. So please update your Python environment if needed.

First, let’s import bar_chart from InterMine. Like the tutorial 13, you need to access your account from humanmine in the method save_mine_and_token.

plot_go_vs_p(list name) can be used to print GO Terms vs p-value, as the name suggests. Also each bar in the bar-chart is labelled by the gene count corresponding to the particular GO Term.

Here we can see the bar chart.

Similarly, plot_go_vs_count(list name) can be used to print GO Terms vs gene count. Again, each bar in the bar-chart is labelled by the annotation corresponding to the particular GO Term.

Again, we can see the bar chart.

query_to_barchart_log is used to plot the query given as an argument in xml format.

It is important to note that the query should be in a format such that the first row contains the gene, the second row has content for x-axis and the third row consists of y-axis values.

When the second argument is 'true', the y axis values are converted to their corresponding log values. It is really useful if the values have a diverse range. If not needed, the second argument can be any string except an empty string(“\t”)

We can see the bar chart here.

We will soon be coming out with more plots. If you have any ideas feel free to open an issue in the Python Client repository.

In the next tutorial, it will help you utilise the module to get details about the data model of various mines.

Thank you for watching!
