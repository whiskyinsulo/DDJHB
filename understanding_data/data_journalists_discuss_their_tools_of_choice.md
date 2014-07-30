# Data Journalists Discuss Their Tools of Choice

Psssss. That is the sound of your data decompressing from its airtight wrapper. Now what? What do you look for? And what tools do you use to get stuck in? We asked data journalists to tell us a bit about how they work with data. Here is what they said.

###Lisa Evans, The Guardian

At the Guardian Datablog we really like to interact with our readers and allowing them to replicate our data journalism quickly means they can build on the work we do and sometimes spot things we haven’t. So the more intuitive the data tools the better. We try to pick tools that anyone could get the hang of without learning a programming language or having special training and without a hefty fee attached.

We’re currently using Google products quite heavily for this reason. All the datasets we tidy and release are available as a Google Spreadsheet which means people with a Google account can download the data, import it into their own account and make their own charts, sort the data and create pivot tables or they can import the data into a tool of their choice.

To map data we use Google Fusion tables. When we create heat maps in Fusion we share our KML shape files so that readers can download and build their own heat maps maybe adding extra layers of data onto the Datablog’s original map. The other nice feature of these Google tools is that they work on the many platforms our readers use to access the blog, such as their desktop, their mobile and tablets.

In addition to Google Spreadsheets and Fusion we use two other tools in our daily work. The first is tableau is visualise multi-dimensional data sets, the second is ManyEyes for quick analysis of data. None of these tools are perfect so we continue to look for better visualization tools that our readers will enjoy.

###Cynthia O’Murchu, Financial Times

Am I ever going to be a coder? Very unlikely! I certainly don’t think that all reporters need to know how to code. But I do think it is very valuable for them to have a more general awareness of what is possible and know how to talk to coders.

If you’re starting out, walk don’t run. You need to persuade your colleagues and editors that working with data can get you stories that you wouldn’t otherwise get and that it’s worthwhile doing. Once they see the value of this approach, you can expand into doing more complex stories and projects.

My advice is to learn Excel and do some simple stories first. Start out small and work your way up to database analysis and mapping. You can do so much in Excel - it’s an extremely powerful tool and most people don’t even use a fraction of its functionality. If you can, go on a course on Excel for journalists such as the one offered by the Centre for Investigative Journalism.

With respect to interpreting data: don’t take this lightly. You have to be conscientious. Pay attention to detail and question your results. Keep notes on how you’re processing the data and keep a copy of the original data. It is easy to make a mistake. I always do my analysis two or three times practically from scratch. Even better would be to get your editor or someone else to analyze the data separately and compare the results.

### Scott Klein, ProPublica

The ability to write and deploy complex software as quickly as a reporter can write a story is a pretty new thing. It used to take a lot longer. Things changed thanks to the development of two free/open source rapid development frameworks: Django and Ruby on Rails, both of which were first released in the mid-2000s.

Django, which is built on top of the Python programming language, was developed by Adrian Holovaty and a team working in a newsroom - the Lawrence Journal-World in Lawrence, Kansas. Ruby on Rails was developed in Chicago by by David Heinemeier Hansson and 37Signals, a web application company.

Though the two frameworks take different approaches to the “MVC pattern” they’re both excellent and make it possible to build even very complex web applications very quickly. They take away some of the rudimentary work of building an app. Things like creating and fetching items from the database, and matching URLs to specific code in an app are built into the frameworks, so developers don’t need to write code to do basic things like that.

While there hasn’t been a formal survey of news app teams in the U.S., it is generally understood that most teams use one of these two frameworks for database-backed news apps. At ProPublica we use Ruby on Rails.

The development of rapid web server “slice” provisioning services like Amazon Web Services also took away some of what used to make deploying a web app a slow process.

Apart from that, we pretty standard tools to work with data: Google Refine and Microsoft Excel to clean data; SPSS and R to do statistics; ArcGIS and QGIS to do GIS; Git for source code management; TextMate, Vim and Sublime Text for writing code; and a mix of MySQL, PostgreSQL and SQL Server for databases. We built our own JavaScript framework called “Glass” that helps us build front-end heavy apps in JavaScript very quickly.

###Cheryl Phillips, Seattle Times

Sometimes the best tool can be the simplest tool - the power of a spreadsheet is easy to underestimate. But using a spreadsheet back when everything was in DOS enabled me to understand a complex formula for the partnership agreement for the owners of The Texas Rangers - back when George W. Bush was one of the key owners. A spreadsheet can help me flag outliers or mistakes in calculations. I can write clean-up scripts and more. It is a basic in the toolbox for a data journalist. That said, my favourite tools have even more power - SPSS for statistical analysis and mapping programs that enable me to see patterns geographically.

###Gregor Aisch, Open Knowledge Foundation

I’m a big fan of Python. Python is a wonderful open source programming language which is easy to read and write (e.g. you don’t have to type a semi-colon after each line). More importantly, Python has a tremendous user base and therefore has plugins (called packages) for literally everything you need.

I would consider Django as something rarely needed by data journalists. It is a Python web application framework, aka a tool to create big, database driven web applications. It is definitely too heavyweight for small interactive infographics.

I also used QGis, which is an open source toolkit providing a wide range of GIS functionality needed by data journalists who deal with geo data every now and then. If you need to convert geospatial data from one format into another, then QGis is what you need. It can handle nearly every geodata format out there (Shapefiles, KML, GeoJSON, …). If you need to cut out a few regions, QGis can do this as well. Plus there is a huge community around QGis so you find tons of resources like [tutorials](http://wiki.awf.forst.uni-goettingen.de/wiki/index.php/QGIS_tutorial_2012) out in the web.

R was created mainly as a scientific visualization tool. It is hard to find any visualization method or data wrangling technique that is not already built into R. R is a universe in its own, the mecca of visual data analysis. One drawback is that you need to learn (yet another) programming language as R has it’s own language. But once you have taken the initial climb on the learning curve, there’s no tool more powerful than R. Trained data journalists can use R to analyze huge dataset which extends the limits of Excel (for instance, if you have a table with a million rows).

What’s really nice about R is that you’re able to keep an exact ‘protocol’ of what you’re doing with the data along the entire process from reading a CSV file to generating charts. If the data changes, you can regenerate the chart using one click. If someone is curious about the integrity of your chart, you can show the exact source which allows everyone to recreate the exact chart on their own (or maybe find the mistakes you made).

NumPy + MatPlotLib is kind of a way of doing the same thing in Python. It’s an option if you’re already well trained in Python. In fact, NumPy and MatPlotLib are two examples of Python packages. They can be used for data analysis and data visualization and are both limited to static visualizations. They cannot be used to create interactive charts with tooltips and more advanced stuff.

I’m not using MapBox, but I’ve heard it is a great tool if you want to provide more sophisticated maps based on OpenStreetMap. It allows you, for instance, to customise the map styles (colours, labels, etc). There’s also a companion of MapBox, called Leaflet. Leaflet is basically a higher level JavaScript library for mapping that allows you to easily switch between map providers (OSM, MapBox, Google Maps, Bing, …).

RaphaelJS is a rather low-level visualization library which allows you to work with basic primitives (like circles, lines, texts), and to animate them, add interactions etc. There’s no thing like a ready to use bar chart in it, so you have to draw a set of rectangles yourself.

However, the good thing about Raphael is that everything you create will also work in Internet Explorer. That’s not the case with many other (amazing) visualization libraries like d3. Sadly, so many users are still using IE and no newsroom can afford to ignore 30% of their users.

Besides of RaphaelJS, there’s also the option of creating a Flash fallback for IE. That is basically what the New York Times is doing. This means that you have to develop each application twice.

I’m still not convinced about the “best” process of shipping visualization for IE and modern browsers. Often I find that RaphaelJS applications can run horribly slow on IE, like ten times slower than they run in Flash using modern browsers. So Flash fallbacks might be a better option if you want to provide high quality animated visualizations for all users.

###Steve Doig, Walter Cronkite School of Journalism of Arizona State University

My go-to tool is Excel, which can handle the majority of CAR problems and has the advantages of being easy to learn and available to most reporters. When I need to merge tables, I typically use Access, but then export the merged table back into Excel for further work. I use ESRI’s ArcMap for geographic analyzes; it’s powerful and is used by the agencies that gather geocoded data. TextWrangler is great for examining text data with quirky layouts and delimiters, and can do sophisticated search-and-replace with regular expressions. When statistical techniques like linear regression are needed, I use SPSS; it has a friendly point-and-click menu. For really heavy lifting, like working with datasets that have millions of records that may need serious filtering and programmed variable transformations, I use SAS software.

###Brian Boyer, Chicago Tribune

Our tools of choice include Python and Django. For hacking, scraping and playing with data, and PostGIS, QGIS and the MapBox toolkit for building crazy web maps. R and NumPy + MatPlotLib are currently battling for supremacy as our kit of choice for exploratory data analysis, though our favorite data tool of late is homegrown: CSVKit. More or less everything we do is deployed in the cloud.

###Angélica Peralta Ramos, La Nacion (Argentina)

At La Nacion we use:

* Excel for cleaning, organising and analyzing data;
* Google Spreadsheets for publishing and connecting with services such as Google Fusion Tables and the Junar Open Data Platform;
* Junar for sharing our data and embedding it in our articles and blog posts;
* Tableau Public for our interactive data visualizations;
* Qlikview, a very fast business intelligence tool that we use to analyze and filter large datasets;
* NitroPDF for converting PDFs to text and excel files;
* Google Fusion Tables for map visualizations.

###Pedro Markun, Transparência Hacker

As a grassroots community without any technical bias we at Transparency Hackers use a lot of different tools and programming languages. Every member has it’s own set of preferences and this great variety is both our strength and our weakness. Some of us are actually building a ‘Transparency Hacker Linux Distribution’ which we could live-boot anywhere and start hacking data. This toolkit has some interesting tools and libraries for handling data like Refine, RStudio and OpenOffice Calc (usually an overlooked tool by savvy people, but really useful for quick/small stuff). Also we’ve been using Scraperwiki quite a lot to quickly prototype and save data results online.

For data visualization and graphs there are a lot of tools we like. Python and NumPy are pretty powerful. A few people in the community have been playing with R but at the end of the day I still think Javascript plotting graph libs like d3, Flot and RaphaelJS ends up being used in the majority of the projects. Finally, we’ve been experimenting a lot with mapping and Tilemill has been a really interesting tool to work with.
