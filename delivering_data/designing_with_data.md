# Designing With Data

Similar in a way to graphing connections, flow diagrams also encode information into the connecting lines, usually by thickness and/or colour. For example, with the Eurozone in crisis and several members incapable of meeting their debts, The New York Times [sought to untangle the web of borrowing](http://www.nytimes.com/interactive/2011/10/23/sunday-review/an-overview-of-the-euro-crisis.html) that tied EU members together with their trading partners across the Atlantic and in Asia. In one “state” of the visualization, the width of the line reflects the amount of credit passing from one country to another, where a yellow to orange colour ramp indicates how “worrisome” it is – i.e., unlikely to be paid back!

On a happier topic, National Geographic magazine produced a [deceptively simple chart showing the connections of three US cities](http://www.sankey-diagrams.com/carbon-footprint-sankey-of-wine-transport/) – New York, Chicago and Los Angeles – to major wine producing regions, and how the transportation methods bringing product from each of the sources could result in drastically different carbon footprints, making Bordeaux a greener buy for New Yorkers than California wine, for example.

“SourceMap”, a project started at MIT’s business school, uses flow diagrams to take a rigorous look at global procurement for manufactured products, their components and raw materials. Thanks to a lot of heavy research, a user can now search for products ranging from [Ecco brand shoes](http://sourcemap.com/view/1760) to [orange juice](http://sourcemap.com/view/1011) and find out from what corners of the globe it was sourced from, and what would be its corresponding carbon footprint.

###To Show Hierarchy

![figs/incoming/06-GG-06.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-GG-06.png "Figure 92. OpenSpending.org (Open Knowledge Foundation)")
<center><small>Figure 92. OpenSpending.org (Open Knowledge Foundation)</small></center>

In 1991, the researcher Ben Shneiderman invented a new visualization form called the “[treemap](http://www.cs.umd.edu/hcil/treemap-history/)” consisting of multiple boxes concentrically nested inside of each other. The area of a given box represents the quantity it represents, both in itself and as an aggregate of its contents. Whether [visualizing a national budget by agency and sub agency](http://openspending.org/), visualizing the stock market by sector and company, or a programming language by classes and sub-classes, the treemap is a compact and intuitive interface for mapping an entity and its constituent parts. Another effective format is the dendrogram, which looks like a more typical organization chart, where sub-categories continue to branch off a single originating trunk.

###To Browse Large Databases

![figs/incoming/06-GG-07.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-GG-07.png "Figure 93. Every death on the road in Great Britain 1999-2000 (BBC)")
<center><small>Figure 93. Every death on the road in Great Britain 1999-2000 (BBC)</small></center>

While sometimes data vis is very effective at taking familiar information and showing it in a whole new light, what happens when you have brand-new information that people want to navigate? The age of data brings with it startling new discoveries almost every day, from Eric Fischer’s brilliant [geographic analyzes of Flickr snapshots](http://www.flickr.com/photos/walkingsf/sets/72157624209158632) to New York City’s release of thousands of previously [confidential teacher evaluations](http://projects.wsj.com/nyc-teachers/).

These data sets are at their most powerful when users can dig in and drill down to the information that is most relevant to them.

In early 2010, The New York Times was given access to Netflix’s normally private records of what areas rent which movies the most often. While Netflix declined to disclose raw numbers, The Times created an [engaging interactive database](http://www.nytimes.com/interactive/2010/01/10/nyregion/20100110-netflix-map.html) that let users browse the top 100-ranked rentals in 12 US metro areas, broken down to the postal code level. A colour-graded “heatmap” overlaid on each community enabled users to quickly scan and see where a particular title was most popular.

Toward the end of that same year, the Times [published the results of the United States decennial census](http://projects.nytimes.com/census/2010/explorer) — just hours after it was released. The interface, built in Adobe Flash, offered a number of visualization options and allowed users to browse down to every single census block in the nation (out of 8.2 million) to see the distribution of residents by race, income and education. Such was the resolution of the data, when looking through the data set in the first hours after publication, you wondered if you might be the first person in the world to explore that corner of the database.

Similar laudable uses of visualization as a database front-end include the BBC’s [investigation of traffic deaths](http://www.bbc.co.uk/news/uk-15975720), and many of the attempts to quickly index large scale data dumps as Wikileaks' release of the Iraq and Afghanistan war logs.

###To Envision Alternate Outcomes

![figs/incoming/06-GG-08.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-GG-08.png "Figure 94. Budget Forecasts, Compared with Reality (New York Times)")

<center><small>Figure 94. Budget Forecasts, Compared with Reality (New York Times)</small></center>

In the New York Times, Amanda Cox’s “porcupine chart” of [tragically optimistic US deficit projections](http://www.nytimes.com/interactive/2010/02/02/us/politics/20100201-budget-porcupine-graphic.html) over the years shows how sometimes what happened is less interesting than what didn’t happen. Cox’s fever line showing the surging budget deficit after a decade of war and tax breaks shows how unrealistic expectations of the future can turn out to be.

Bret Victor, a longtime Apple interface designer (and originator of the "kill math" theory of visualization to communicate quantitative information), has prototyped a kind of *[reactive document](http://worrydream.com/#!/TenBrighterIdeas)*. In his example, energy conservation ideas include editable premises, whereby a simple step like shutting off lights in empty rooms could save Americans the output of from two to 40 coal plants. Changing the percentage referenced in the middle of a paragraph of text causes the text in the rest of the page to update accordingly!

For more examples and suggestions, here is a [list of different uses for visualizations, maps and interactive graphics](http://www.ericson.net/content/2011/04/international-journalism-festival-links/) compiled by Matthew Ericson of The New York Times.

###When Not To Use Data visualization

In the end, effective data visualization depends on good, clean, accurate and meaningful information. Just as much as good quotes, facts and descriptions power good narrative journalism, data vis is only as good as the data that fuels it.

###When Your Story Can Be Better Told Through Text or Multimedia

Sometimes the data alone does not tell the story in the most compelling way. While a simple chart illustrating a trend line or summary statistic can be useful, a narrative relating the real-world consequences of an issue can be more immediate and impactful to a reader.

###When You Have Very Few Data Points

It has been said, “a number in isolation doesn’t mean anything”. A common refrain from news editors in response to a cited statistic is, “compared to what?” Is the trend going up or down? What is normal?

###When You Have Very Little Variability in Your Data, No Clear Trend or Conclusion

Sometimes you plot your data in Excel or a similar charting app and discover that the information is noisy – a lot of fluctuation, or a relatively flat trend. Do you raise the baseline from zero to just below the lowest value, in order to give the line some more shape? No! Sounds like you have ambiguous data and need to do more digging and analysis.

###When a Map is Not a Map

When the spatial element is not meaningful or compelling, or distracts attention from more pertinent numeric trends, like change over time or showing similarities between non-adjacent areas.

###Don’t Forget About Tables

If you have relatively few data points but have information that might be of use to some of your readers, consider just laying out the data in tabular form. It’s clean, easy to read and doesn’t create unrealistic expectations of "story." In fact, tables can be a very efficient and elegant layout for basic information.

— *Brian Suda, (optional.is)*
