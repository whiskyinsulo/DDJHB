# Data visualization DIY: Our Top Tools

![figs/incoming/06-LL-01.jpg
](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-01.jpg "Figure 102. The Wikileaks war logs (The Guardian)")

<small>Figure 102. The Wikileaks war logs (The Guardian)</small>

What data visualization tools are out there on the web that are easy to use - and free? Here on the [Datablog and Datastore](http://www.guardian.co.uk/data) we try to do as much as possible using the internet’s powerful free options.

That may sound a little disingenuous, in that we obviously have access to the Guardian’s amazing graphics and interactive teams for those pieces where we have a little more time - such as [this map of public spending](http://www.guardian.co.uk/news/datablog/2011/oct/26/government-spending-department-2010-11) (created using Adobe Illustrator) or this [Twitter riots interactive](http://www.guardian.co.uk/uk/interactive/2011/dec/07/london-riots-twitter).

But for our day-to-day work, we often use tools that anyone can - and create graphics that anyone else can too.

So, what do we use?

###[Google Fusion Tables](http://www.google.com/fusiontables/Home/)

This online database and mapping tool has become our default for producing quick and detailed maps, especially those where you need to zoom in. You get all the high resolution of google maps but it can open a lot of data - 100mb of CSV, for instance. The first time you try it, Fusion tables may seem a little tricky - but stick with it. We used it to produce maps like the Iraq one above and also border maps like this one of homelessness too.

![figs/incoming/06-LL-02.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-02.jpg "Figure 103. Homelessness interactive map (The Guardian)")

<small>Figure 103. Homelessness interactive map (The Guardian)</small>

The main advantage is the flexibility - you can can upload a kml file of regional borders, say - and then merge that with a data table. It’s also getting a new user interface, which should make it easier to use.

You don’t have to be a coder to make one - and [this Fusion layers tool](http://gmaps-samples.googlecode.com/svn/trunk/fusiontables/fusiontableslayer_builder.html) allows you to bring different maps together or to create search and filter options, which you can then embed on a blog or a site.

[This excellent tutorial by Google’s Kathryn Hurley](http://sites.google.com/site/fusiontablestalks/talks/fusion-tables-where-2-0-workshop) is a great place to start.

**Top tip** : use shpescape to convert official shp files into Fusion tables for you to use. Also, watch out for over-complicated maps - Fusion can’t cope with more than a million points in one cell

###[Tableau Public](http://www.tableausoftware.com/public)

If you don’t need the unlimited space of the professional edition, this is free - and means you can make pretty complex visualizations simply and easily with up to 100,000 rows. We use it when we need to bring different types of charts together - as in [this map of top tax rates around the world](http://www.guardian.co.uk/news/datablog/interactive/2012/mar/20/top-tax-rates-world), which also has a bar chart too.

Or you can even use it as a data explorer - which is what we did below with the [US federal elections spending data](http://www.guardian.co.uk/news/datablog/2012/feb/02/us-presidential-election-fundraising) (although we ran out of space in the free public version - something to watch out for). Tableau also needs the data formatted in quite specific ways for you to get the most out of it. But get through that and you have something intuitive which works well. [La Nación in Argentina has built its entire data journalism operation around Tableau](http://blogs.lanacion.com.ar/data/), for instance.

![figs/incoming/06-LL-03.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-03.png "Figure 104. 2012 Presidential Campaign Finance (The Guardian)")

<small>Figure 104. 2012 Presidential Campaign Finance (The Guardian)</small>

Tableau has some good [online tutorials](http://www.tableausoftware.com/learn/training) here for you to start with.

**Top tip** : Tableau is designed for PCs, although a Mac version is in the works. Use a mirror such as parallels to make it work

###[Google spreadsheet charts](http://www.google.com/google-d-s/spreadsheets/)

![figs/incoming/06-LL-04.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-04.jpg "Figure 105. UK government spending and taxation (The Guardian)")

<small>Figure 105. UK government spending and taxation (The Guardian)</small>

After something simple - like a bar or line chart, or a pie chart? You’ll find that Google spreadsheets (which you create from the documents bit of your Google account) can create some pretty nice charts - including the animated bubbles used by Hans Rosling’s [Gapminder](http://www.gapminder.org/). Unlike the [charts API](http://code.google.com/apis/chart/) you don’t need to worry about code - it’s pretty similar to making a chart in Excel, in that you highlight the data and click the chart widget. The customisation options are worth exploring too - you can change colours, headings and scales. They are pretty design-neutral, which is useful in small charts. The line charts have some nice options too, including annotation options.

**Top tip** : spend some time with the chart customisation options - you can create your own colour palette

![figs/incoming/06-LL-05.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-05.jpg "Figure 106. Death Row Prisoners and Executions (Datamarket)")

<small>Figure 106. Death Row Prisoners and Executions ([Datamarket](http://datamarket.com/))</small>

###[Explore this data](http://datamarket.com/data/set/1n0t/#ds=1n0t!1o3i&display=line&m=tg,th,tj) US executions

Better-known as a data supplier, Datamarket is actually a pretty nifty tool for visualizing numbers too. You can upload your own or use some of the many datasets they have to offer - but the options do get better if you get the Pro account.

**Top tip** : works best with time series data, but check out their extensive data range

###[Many Eyes](http://www-958.ibm.com/software/data/cognos/manyeyes/)

If ever a site needed a bit of TLC, it’s IBM’s Many Eyes. When it launched, created by [Fernanda B. Viégas](http://fernandaviegas.com/) and [Martin Wattenberg](http://www.bewitched.com/) it was a unique exercise in allowing people to simply upload datasets and visualise them. Now, with its creators working for Google, the site feels a little unloved with its muted colour palettes - and hasn’t seen much new in the way of visualizations for some time.

![figs/incoming/06-LL-06.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-06.jpg "Figure 107. Doctor Who Villains (The Guardian)")

<small>Figure 107. Doctor Who Villains (The Guardian)</small>

###[Doctor Who Villains](http://www.guardian.co.uk/news/datablog/2010/jul/16/doctor-who-villains-list)

If ever a site needed a bit of TLC, it’s IBM’s Many Eyes. When it launched, created by Fernanda B. Viégas and Martin Wattenberg it was a unique exercise in allowing people to simply upload datasets and visualise them. Now, with its creators working for Google, the site feels a little unloved with its muted colour palettes - and hasn’t seen much new in the way of visualizations for some time.

![figs/incoming/06-LL-07.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-07.jpg)

**Top tip** : you can’t edit the data once you’ve uploaded it, so make sure you get it right before you create it.

###[Color Brewer](http://colorbrewer2.org/)

![figs/incoming/06-LL-08.jpg
](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-08.jpg "Figure 108. Color brewer")

<small>Figure 108. Color brewer</small>

Not, strictly speaking, a visualization tool, Color Brewer - originally designed with federal funding and developed at Penn State - is really for choosing map colors, and is worth spending some time with if plan to make many more. You can choose your base colour and get the codes for the entire palette.

And some more
![figs/incoming/06-LL-09.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/06-LL-09.jpg "Figure 109. More from Color Brewer")

<small>Figure 109. More from Color Brewer</small>

If none of these are for you, it’s also worth checking out this [DailyTekk piece](http://dailytekk.com/2012/02/27/over-100-incredible-infographic-tools-and-resources/) which has even more options. The ones above aren’t the only tools, just those we use most frequently. There are lots of others out there too, including:

* [Chartsbin](http://chartsbin.com/) A tool for creating clickable world maps
* [iCharts](http://www.icharts.net/) Specialises in small chart widgets
* [Geocommons](http://geocommons.com/) Shares data and boundary data to create global and local maps

Oh and there’s also [piktochart.com[(http://piktochart.com/), which provides templates for those text/numbers visualizations there are a lot of around at the moment.

— *Simon Rogers, The Guardian*

.
