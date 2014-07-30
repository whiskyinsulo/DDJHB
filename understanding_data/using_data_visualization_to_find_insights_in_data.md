# Using Data Visualization to Find Insights in Data

*visualization is critical to data analysis. It provides a front line of attack, revealing intricate structure in data that cannot be absorbed in any other way. We discover unimagined effects, and we challenge imagined ones.*

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;— *William S. Cleveland: visualizing Data*

Data by itself, consisting of bits and bytes stored in a file on a computer hard drive, is invisible. In order to be able to see and make any sense of data, we need to visualize it. In this chapter I’m going to use a broader understanding of the term visualizing, that includes even pure textual representations of data. For instance, just loading a dataset into a spreadsheet software can be considered as data visualization. The invisible data suddenly turns into a visible ‘picture’ on our screen. Thus, the questions should not be whether journalists need to visualize data or not, but which kind of visualization may be the most useful in which situation.

In other words: when does it makes sense to go beyond the table visualization? The short answer is: almost always. Tables alone are definitely not sufficient to give us an overview of a dataset. And tables alone don’t allow us to immediately identify patterns within the data. The most common example here are geographical patterns which can only be observed after visualizing data on a map. But there are also other kinds of patterns which we will see later in this chapter.

###Using visualization to Discover Insights

It is unrealistic to expect that data visualization tools and techniques will unleash a barrage of ready-made stories from datasets. There are no rules, no ‘protocol’ that will guarantee us a story. Instead, I think it makes more sense to look for ‘insights’, which can be artfully woven into stories in the hands of a good journalist.

Every new visualization is likely to give us some insights into our data. Some of those insights might be already known (but perhaps not yet proven) while other insights might be completely new or even surprising to us. Some new insights might mean the beginning of a story, while others could just be the result of errors in the data, which are most likely to be found by visualizing the data.

In order to make the finding of insights in data more effective, I find the following process very helpful:

![figs/incoming/05-BB.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-BB.png "Figure 71. Data insights: a visualization (Gregor Aisch)")

<center><small>Figure 71. Data insights: a visualization (Gregor Aisch)</small></center>

Each of these steps will be discussed further in this section.

###How To Visualize Data

Visualization provides a unique perspective on the dataset. You can visualize data in lots of different ways.

Tables are very powerful when you are dealing with a relatively small number of data points. They show labels and amounts in the most structured and organized fashion and reveal their full potential when combined with the ability to sort and filter the data. Additionally, Edward Tufte suggested including small chart pieces within table columns, for instance one bar per row or a small line chart (since then also known as a sparkline). But still, as mentioned in the introduction, tables clearly have their limitations. They are great to show you one-dimensional outliers like the top 10, but they are poor when it comes to comparing multiple dimensions at the same time (for instance population per country over time).

![figs/incoming/05-BC-graphical-table.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-BC-graphical-table.png "Figure 72. Tips from Tufte: sparklines (Gregor Aisch)")

<center><small>Figure 72. Tips from Tufte: sparklines (Gregor Aisch)</small></center>

Charts, in general, allow you to map dimensions in your data to visual properties of geometric shapes. There’s much written about the effectiveness of individual visual properties, and the short version is: color is difficult, position is everything. In a scatterplot, for instance, two dimensions are mapped to the to the x- and y-position. You can even display a third dimension to the color or size of the displayed symbols. Line charts are especially suited for showing temporal evolutions while bar charts are perfect for comparing categorical data. You can stack chart elements on top of each other. If you want to compare a small number of groups in your data, displaying multiple instances of the same chart is a very powerful way (also referred to as small multiples). In all charts you can use different kinds of scales to explore different aspects in your data (e.g., linear or log scale).

In fact, most of the data we’re dealing with is somehow related to actual people. The power of maps is to re-connect the data to our very physical world. Imagine a dataset of geo-located crime incidents. Crucially, you want to see where the crimes happen. Also maps can reveal geographic relations within the data, e.g. a trend from North to South or from urban to rural areas.

![figs/incoming/05-BD-choropleth.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-BD-choropleth.png "Figure 73. Cloropeth (Gregor Aisch)")

<center><small>Figure 73. Cloropeth (Gregor Aisch)</small></center>

Speaking of relations, the fourth most important type of visualization is a graph. Graphs are all about showing the inter-connections (edges) in your data points (nodes). The position of the nodes is then calculated by more or less complex graph layout algorithms which allow us to immediately see the structure within the network. The trick about graph visualization in general is to find a proper way to model the network itself. Not all datasets already include relations and even if they do, it might not be the most interesting aspect to look at. Sometimes it’s up to the journalist to define edges between nodes. A perfect example of this is the [U.S. Senate Social Graph](http://www.slate.com/articles/news_and_politics/politics/2009/04/the_senate_social_network.html), whose edges connect senators that voted the same in more than 65% of the votes.

![figs/incoming/05-BE-graph.jpg
](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-BE-graph.jpg "Figure 74. The Senate Social Network (slate.com)")

<center><small>Figure 74. The Senate Social Network (slate.com)</small></center>

###Analyze and Interpret What You See

Once you have visualized your data, the next step is to learn something from the picture you created. You could ask yourself:

* What can I see in this image? Is it what I expected?
* Are there any interesting patterns?
* What does this mean in the context of the data?

Sometimes you might end up with visualization that, in spite of its beauty, might seem to tell you nothing of interest about your data. But there is almost always something that you can learn from any visualization, however trivial.

###Document Your Insights and Steps

If you think of this process as a journey through the dataset, the documentation is your travel diary. It will tell you where you have traveled to, what you have seen there and how you made your decisions for your next steps. You can even start your documentation before taking your first look at the data.

In most cases when we start to work with a previously unseen dataset we are already full of expectations and assumptions about the data. Usually there is a reason why we are interested that dataset that we are looking at. It’s a good idea to start the documentation by writing down these initial thoughts. This helps us to identify our bias and reduces the risk of mis-interpretation of the data by just finding what we originally wanted to find.

I really think that the documentation is the most important step of the process; and it is also the one we’re most likely to tend to skip. As you will see in the example below, the described process involves a lot of plotting and data wrangling. Looking at a set of 15 charts you created might be very confusing, especially after some time has passed. In fact, those charts are only valuable (to you or any other person you want to communicate your findings) if presented in the context in which they have been created. Hence you should take the time to make some notes on things like:

* Why have I created this chart?
* What have I done to the data to create it?
* What does this chart tell me?

###Transform Data

Naturally, with the insights that you have gathered from the last visualization you might have an idea of what you want to see next. You might have found some interesting pattern in the dataset which you now want to inspect in more detail.

Possible transformations are:

####Zooming
> To have look at a certain detail in the visualization Aggregation To combine many data points into a single group

####Filtering
> To (temporarily) remove data points that are not in our major focus

####Outlier removal
> To get rid of single points that are not representative for 99% of the dataset.

Let’s consider that you have visualized a graph and what came out of this was nothing but a mess of nodes connected through hundreds of edges (a very common result when visualizing so-called densely connected networks), one common transformation step would be to filter some of the edges. If, for instance, the edges represent money flows from donor countries to recipient countries we could remove all flows below a certain amount.

###Which Tools to Use

The question of tools is not any easy one. Every data visualization tool available is good at something. Visualization and data wrangling should be easy and cheap. If changing parameters of the visualizations takes you hours, you won’t experiment that much. That doesn’t necessarily mean that you don’t need to learn how to use the tool. But once you learned it, it should be really efficient.

It often makes a lot of sense to choose a tool that covers both the data wrangling and the data visualization issues. Separating the tasks in different tools means that you have to import and export your data very often. Here’s a short list of some data visualization and wrangling tools:

* Spreadsheets like LibreOffice, Excel or Google Docs.
* Statistical programming frameworks like R (r-project.org) or Pandas (pandas.pydata.org)
* Geographic Information Systems (GIS) like Quantum GIS, ArcGIS, GRASS
* visualization Libraries like d3.js (mbostock.github.com/d3), Prefuse (prefuse.org), Flare (flare.prefuse.org)
* Data Wrangling Tools: Google Refine, Datawrangler
* Non-Programming Visualization Software: like ManyEyes, Tableau Public (tableausoftware.com/products/public)

The sample visualizations in the next section were created using R, which is kind of a swiss army knife of (scientific) data visualization.

###An Example: Making Sense of US Election Contribution Data

Let us have look at the US Presidential Campaign Finance database which contains about 450,000 contributions to US Presidential candidates. The CSV file is 60 megabytes and way too big to handle easily in a programme like Excel.

In the first step I will explicitly write down my initial assumptions on the FEC contributions dataset:

* Obama gets the most contributions (since he is the president and has the greatest popularity)
* The number of donations increases as the time moves closer to election date.
* Obama gets more small donations than Republican candidates.

To answer the first question we need to transform the data. Instead of each single contributions we need to sum the total amounts contributed to each candidate. After visualizing the results in a sorted table we can confirm our assumption that Obama would raise the most money:

Candidate | Amount ($)
--------- | ----------:
Obama, Barack | 72,453,620.39
Romney, Mitt  | 50,372,334.87
Perry, Rick   | 18,529,490.47
Paul, Ron     | 11,844,361.96
Cain, Herman  | 7,010,445.99
Gingrich, Newt| 6,311,193.03
Pawlenty, Timothy | 4,202,769.03
Huntsman, Jon |2,955,726.98
Bachmann, Michelle | 2,607,916.06
Santorum, Rick| 1,413,552.45
Johnson, Gary Earl | 413,276.89
Roemer, Charles E. Buddy III | 291,218.80
McCotter, Thaddeus G | 37,030.00

Even though this table shows the minimum and maximum amounts and the order, it does not tell very much about the underlying patterns in candidate ranking. Figure 75 is another view on the data, a chart type that is called ‘dot chart’ in which we can see everything that is shown in the table plus the patterns within the field. For instance, the dot chart allows us to immediately compare the distance between Obama and Romney and Romney and Perry without needing to subtract values. (Note: The dot chart was created using R. You can find links to the source codes at the end of this chapter).

![figs/incoming/05-CC.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-CC.png "Figure 75. visualizations to spot underlying patterns (Gregor Aisch)")

<center><small>Figure 75. visualizations to spot underlying patterns (Gregor Aisch)</small></center>

Now, let us proceed with a bigger picture of the dataset. As a first step I visualized all contributed amounts over time in a simple plot. We can see that almost all donations are very very small compared to three really big outliers. Further investigation returns that these huge contribution are coming from the “Obama Victory Fund 2012” (also known as Super PAC) and were made on June 29th ($450k), September 29th ($1.5mio) and December 30th ($1.9mio).

![figs/incoming/05-DD.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-DD.png "Figure 76. Three clear outliers (Gregor Aisch)")

<center><small>Figure 76. Three clear outliers (Gregor Aisch)</small></center>

While the contributions by Super PACs alone is undoubtedly the biggest story in the data, it might be also interesting to look beyond it. The point now is that these big contributions disturb our view on the smaller contributions coming from individuals, so we’re going to remove them from the data. This transform is commonly known as outlier removal. After visualizing again, we can see that most of the donations are within the range of $10k and -$5k.

![figs/incoming/05-EE.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-EE.png "Figure 77. Removing the outliers (Gregor Aisch)")

<center><small>Figure 77. Removing the outliers (Gregor Aisch)</small></center>

According to the contribution limits placed by the FECA individuals are not allowed to donate more than $2500 to each candidate. As we see in the plot, there are numerous donations made above that limit. In particular two big contributions in May attract our attention. It seems that they are mirrored in negative amounts (refunds) June and July. Further investigation in the data reveals the following transactions:

* On May 10 *Stephen James Davis*, San Francisco, employed at Banneker Partners (attorney), has donated **$25,800** to Obama.
* On May 25 *Cynthia Murphy*, Little Rock, employed at the Murphy Group (public relations), has donated **$33,300** to Obama.
* On June 15 the amount of **$30,800** was refunded to *Cynthia Murphy*, which reduced the donated amount to **$2500**.
* On July 8 the amount **$25,800** was refunded to *Stephen James Davis*, which reduced the donated amount to $0.

What’s interesting about these numbers? The $30,800 refunded to Cynthia Murphy equals the maximum amount individuals may give to national party committees per year. Maybe she just wanted to combine both donations in one transaction which was rejected. The $25,800 refunded to Stephen James Davis possibly equals the $30,800 minus $5000 (the contribution limit to any other political committee).

Another interesting finding in the last plot is a horizontal line pattern for contributions to Republican candidates at $5000 and -$2500. To see them in more detail, I visualized just the Republican donations. The resulting graphic is kind of the perfect example for patterns in data that would be invisible without data visualization.

![figs/incoming/05-FF.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-FF.png "Figure 78. Removing outliers 2 (Gregor Aisch)")

<center><small>Figure 78. Removing outliers 2 (Gregor Aisch)</small></center>

What we can see is that there are many $5000 donations to Republican candidates. In fact, a look up in the data returns that these are 1243 donations, which is only 0.3% of the total number of donations, but since those donations are evenly spread across time, the line appears. The interesting thing about the line is that donations by individuals were limited to $2500. Consequently, every dollar above that limited was refunded to the donors, which results in the second line pattern at -$2500. In contrast, the contributions to Barack Obama don’t show a similar pattern.

![figs/incoming/05-GG.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-GG.png "Figure 79. Removing outliers 3 (Gregor Aisch)")

<center><small>Figure 79. Removing outliers 3 (Gregor Aisch)</small></center>

So, it might be interesting to find out why thousands of Republican donors did not notice the donation limit for individuals. To further analyze this topic, we can have a look at the total number of $5k donations per candidate.

![figs/incoming/05-HH.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-HH.png "Figure 80. Donations per candidate (Gregor Aisch)")

<center><small>Figure 80. Donations per candidate (Gregor Aisch)</small></center>

Of course, this is a rather distorted view since it does not consider the total amounts of donations received by each candidate. The next plot shows the percentage of $5k donations per candidate.

![figs/incoming/05-II.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-II.png "Figure 81. Where does the senator’s money come from?: donations per candidate (Gregor Aisch)")

<center><small>Figure 81. Where does the senator’s money come from?: donations per candidate (Gregor Aisch)</small></center>

###What To Learn From This

Often, such a visual analysis of a new dataset feels like an exciting journey to an unknown country. You start as a foreigner with just the data and your assumptions, but with every step you make, with every chart you render, you get new insights about the topic. Based on those insights you make decisions for your next steps and what issues are worth further investigation. As you might have seen in this chapter, this process of visualizing, analyzing and transformation of data could be repeated nearly infinitely.

###Get the Source Code

All of the charts shown in this chapter were created using the wonderful and powerful software R. Created mainly as a scientific visualization tool, it is hard to find any visualization or data wrangling technique that is not already built into R. For those who are interested in how to visualize and wrangle data using R, here’s the source code of the charts generated in this chapter. Also, there is a wide range of books and tutorials available.

* [dotchart: contributions per candidate](https://gist.github.com/1769733)
* [plot: all contributions over time](https://gist.github.com/1816161)
* [plot: contributions by authorised committees](https://gist.github.com/1816169)

— *Gregor Aisch, Open Knowledge Foundation*
