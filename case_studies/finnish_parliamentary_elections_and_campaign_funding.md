# Finnish Parliamentary Elections and Campaign Funding

![figs/incoming/03-DD.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-DD.png "Figure 38. Election Financing (Helsingin Sanomat)")

<center><small>Figure 38. Election Financing (Helsingin Sanomat)</small></center>

In recent months there have been ongoing trials related to the election campaign funding of the Finnish general elections of 2007.

After the elections in 2007, the press found out that the laws on publicizing campaign funding had no effect on politicians. Basically, campaign funding has been used to buy favors from politicians, who have then failed to declare their funding as mandated by Finnish law.

After these incidents, the laws became stricter. After the general election in March 2011, Helsingin Sanomat decided to carefully explore all the available data on campaign funding. The new law stipulates, that election funding must be declared and only donations below 1500 euros may be anonymous.

###1. Find Data and Developers.

 Helsingin Sanomat has organized HS Open hackathons since March 2011. We invite Finnish coders, journalists and graphic designers to the basement of our building. Participants are divided into groups of three, and they are encouraged to develop applications and visualizations. We have had about 60 participants in each of our three events so far. We decided that campaign funding data should be the focus of HS Open #2, May 2011.

 The National Audit Office of Finland is the authority that keeps records of campaign funding. That was the easy part. Chief information Officer, Jaakko Hamunen, built a website that provides real time access to their campaign funding database. The Audit Office made this in just two months after our request.

 The [Vaalirahoitus](http://www.vaalirahoitus.fi/).fi website will provide the press and public information on campaign funding on every elections from now on.

###2. Brainstorm for Ideas.

 The participants of HS Open 2 came up with twenty different prototypes about what to do with the data. You can find all the prototypes [on our website](http://blogit.hs.fi/hsnext/hs-open-2-tuotti-parikymmenta-prototyyppia) (text in Finnish).

 A bioinformatics researcher called Janne Peltola noted that campaign funding data looked like gene data they research in terms of containing many interdependencies. In bioinformatics there is an open source tool called [Cytoscape](http://www.cytoscape.org/) which is used to map these interdependencies. So we ran the data through Cytoscape, and had a very interesting prototype.

###3. Implement the Idea on Paper and on the Web.

 The law on campaign funding states that elected members of parliament must declare their funding two months after the elections. In practice this meant that we got the real data in mid-June. In HS Open, we had data only from MPs who had filed before the deadline.

 There was also a problem with the data format. The National Audit Office provided the data as two CSV files. One contained the total budget of campaigns, the other listed all the donors. We had to combine these two, creating a file that contained three columns: donor, receiver and amount. If the politicians had used their own money, in our data format it looked like Politician A donated X euros to Politician A. Counter-intuitive perhaps, but it worked for Cytoscape.

 When the data was cleaned and reformatted, we just ran it through Cytoscape. Then our graphics department made a full page page graphic out of it.

 Finally we created a beautiful visualization on our [website](http://www.vaaliraha.com/). This was not a network analysis graphic. We wanted to give people an easy way to explore how much campaign funding there is and who gives it. The first view shows the distribution of funding between MPs. When you click on one MP, you get the breakdown of his or her funding. You can also vote on whether this particular donor is good or not. The visualization was made by Juha Rouvinen and Jukka Kokko, from an ad agency called Satumaa.

 The web version of campaign funding visualization uses the same data as the network analysis.

###4. Publish the Data

 Of course, the National Audit Office already publishes the data, so there was no need to republish. But, as we had cleaned up the data and given it a better structure, we decided to publish it. We give out our data with a [Creative Commons Attribution licence](http://creativecommons.org/licenses/by/3.0/). Subsequently several independent developers have made visualizations of the data, some of which we have published.

 The tools we used for the project were: Excel and Google Refine for data cleaning and analysis, Cytoscape for network analysis, and Illustrator and Flash for the visualizations. The Flash should have been HTML5, but we ran out of time.

 What did we learn? Perhaps the most important lesson was that data structures can be very hard. If the original data is not in suitable format, recalculating and converting it will take a lot of time.
