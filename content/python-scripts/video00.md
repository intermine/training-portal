# video00

+++ title = "Tutorial 0" description = "" weight = 1 +++    


Welcome to InterMine python tutorial! In this tutorial, I will show you how to interact with the intermine registry, which lists the different InterMines available on the web, and contains information about their URLs, the datasets and organisms you can find in each InterMine, and a few other things.

First, don’t forget to run pip install intermine in your terminal, if you haven’t already.

Then, let’s look at cells.

In the first cell, we run from intermine import registry then registry.getMines from an organism. Then we can see the output. FawMine, Flymine, LocustMine and XenMine are all InterMines that contain information about fruit flies.

Now that we have the mines. We can use getInfo\(mine\) to get all information about a particular mine. Here we use flymine as an example. Let’s click it and we can see the output. The output gives information about it including its description and URL and API version and others.

Next, We can use getData function to get data of flymine.

Then we can see the output.

Good, this is the Intermine Python Tutorial Overview.

Thank you for watching!

