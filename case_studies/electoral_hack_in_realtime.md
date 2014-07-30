# Electoral Hack in Realtime

![figs/incoming/03-FF.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-FF.png "Figure 39. Elections 2011 (Hacks/Hackers Buenos Aires)")

<center><small>Figure 39. Elections 2011 (Hacks/Hackers Buenos Aires)</small></center>

[Electoral Hack](http://elecciones.hhba.info/) is political analysis project that visualizes data from the provisional ballot results of the 23 October 2011 elections in Argentina. The system also features information from previous elections and socio-demographic statistics from across the country. The project was updated in real time with information from the provisional ballot count of the national elections of 2011 in Argentina and gave summaries of election results. It was an initiative of Hacks/Hackers Buenos Aires with the political analyst Andy Tow, and was a collaborative effort of journalists, developers, designers, analysts, political scientists, and others from the local chapter of Hacks/Hackers.

###What data did we use?

All data came from official sources: the National Electoral Bureau provided access to data of the provisional count by Indra; the Department of the Interior provided information about elected posts and candidates from different political parties; a [university project](http://yoquierosaber.org/) provided biographical information and the policy platforms of each presidential ticket; while socio-demographic information came from the 2001 National Census of Population and Housing (INDEC), the 2010 Census (INDEC), and from the Ministry of Health.

###How was it developed?

The application was generated during the 2011 Election Hackathon by Hacks/Hackers Buenos Aires the day before the election on October 23, 2011. The hackathon saw the participation of 30 volunteers with a variety of different backgrounds. Electoral Hack was developed as an open platform that could be improved over time. For the technology, we used Google Fusion Tables, Google Maps, and vector graphics libraries.

We worked on the construction of polygons for displaying geographic mapping and electoral demographics. Combining polygons in GIS software and geometries from public tables in Google Fusion Tables we generated tables with keys corresponding to the electoral database of the Ministry of Interior, Indra and sociodemographic data from INDEC. From this, we created visualizations in Google Maps.

Using the Google Maps API we published several thematic maps representing the spatial distribution of voting with different tones of color, where the intensity of colour represented the percentage of votes for the various presidential tickets in different administrative departments and polling stations, with particular emphasis on major urban centers: the City of Buenos Aires, the 24 districts of Greater Buenos Aires, the City of Cordoba, and Rosario.

We used the same technique to generate thematic maps of previous elections, namely the presidential primaries of 2011 and the election of 2007, as well as of the distribution of sociodemographic data, such as for poverty, child mortality, and living conditions, allowing for analysis and comparison. The project also showed the spatial distribution of the differences in percentage of votes obtained by each ticket in the general election of October compared to the August primary election.

Later, using partial data from the provisional ballot counts, we created an animated map depicting the anatomy of the count, in which the progress of the vote count is shown from the closing of the local polls until the following morning.

###Pros
* We set out to find and represent data and we were able to do that. At hand we had the [UNICEF’s database of child sociodemographics](http://infoargentina.unicef.org.ar/), as well as the database of candidates created by the yoquierosaber.org group of Torcuato Di Tella University. During the hackathon we gathered a large volume of additional data that we did not end up including.
* It was clear that the journalistic and programming work was enriched by scholarship. Without the contribution of Andy Tow and Hilario Moreno Campos, the project would have been impossible to achieve.

###Cons
* The sociodemographic data we could use was not up to date (most was from the 2001 census), and it was not very granular. For example, it did not include detail about local average GDP, main economic activity, education level, number of schools, doctors per capita, lots of other things that it would have been great to have.
* Originally the system was intended as a tool that could be used to combine and display any arbitrary data, so that journalists could easily display data that interested them on the web. But we had to leave this for another time.
* As the project was built by volunteers in a short time frame, it was impossible to do everything that we wanted to do. Nevertheless we made a lot of progress in the right direction.
* For the same reason, all the collaborative work of 30 people ended up condensed into a single programmer when the data offered by the government began to appear, and we ran into some problems importing data in real time. These were solved within hours.

###Implications

The Electoral Hack platform had a big impact in the media, with television, radio, print and online coverage. Maps from the project were used by several media platforms during the elections and in subsequent days. As the days went by, the maps and visualizations were updated, increasing traffic even more. On Election Day, the site created that very day received about 20 thousand unique visitors and its maps were reproduced on the cover page of the newspaper Página/12 for two consecutive days, as well as in articles in La Nación. Some maps appeared in the print edition of the newspaper Clarín. It was the first time that an interactive display of real-time maps had been used in the history of Argentine journalism. In the central maps one could clearly see the overwhelming victory of Cristina Fernandez de Kirchner by 54 percent of the vote, broken up by color saturation. It also served to help users understand specific cases where local candidates had landslide victories in the provinces.

— *This section was written by Mariano Blejman, Mariana Berruezo, Sergio Sorín, Andy Tow and Martín Sarsale from Hacks/Hackers Buenos Aires*
