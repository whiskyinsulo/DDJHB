# The Tell-All Telephone

![figs/incoming/03-BB.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-BB.png "Figure 46. The Tell-All Telephone (Zeit Online)")

<center><small>Figure 46. The Tell-All Telephone (Zeit Online)</small></center>

Most people’s understanding of what can actually be done with the data provided by our mobile phones is theoretical; there were few real-world examples. That is why Malte Spitz from the German Green party decided to publish his own data. To access the information, he had to file a suit against telecommunications giant Deutsche Telekom. The data is the basis for ZEIT Online’s accompanying interactive map, were contained in a massive Excel document. Each of the 35,831 rows of the spreadsheet represent an instance when Spitz’s mobile phone transferred information over a half-year period.

Seen individually, the pieces of data are mostly harmless. But taken together they provide what investigators call a profile; a clear picture of a person’s habits and preferences, and indeed, of his or her life. This profile reveals when Spitz walked down the street, when he took a train, when he was in a plane. It shows that he mainly works in Berlin and which cities he visited. It shows when he was awake and when he slept.

To illustrate just how much detail from someone’s life can be mined from this stored data, ZEIT ONLINE has "augmented" Spitz’s information with records that anyone can access: the politician’s tweets and blog entries were added to the information on his movements. It is the kind of process that any good investigator would likely use to profile a person under observation. ZEIT ONLINE decided to keep one part of Spitz’s data record private, namely, whom he called and who called him. That kind of information would not only infringe on the privacy of many other people in his life, it would also, even if the numbers were encrypted, reveal much too much about Spitz (but government agents in the real world would have access to this information).

We were very happy to work with Lorenz Matzat and Michael Kreil from Open Data City to find a solution how to understand and extract the geolocation from the dataset. Every connection of Spitz’s mobile phone has to be triangulated to the positions of the antenna pole. Every pole has three antennas, each covering 120º. The two programmers found out, that the saved position indicated the direction from the mast Spitz’s mobile phone was connecting from.

Matching this with the positions of the poles-map of the [state-controlled agency](http://emf2.bundesnetzagentur.de/karte.html) gave us the possibility to get his position for each of the 260,640 minutes during the 181 days and put it via API on a Google Map. Together with the in-house graphics and design team we created a great interface to navigate: By pushing the play button, you will set off on a trip through Malte Spitz’s life.

After a very successful launch of the Project in Germany, we noticed that we were having very high traffic from outside Germany and decided to create an English version of the app. After earning the German Grimme Online Award, the project was honored with an ONA Award in September 2011, the first time for a German news website.

* [See the data](https://docs.google.com/spreadsheet/ccc?authkey=COCjw-kG&key=0An0YnoiCbFHGdGp3WnJkbE4xWTdDTVV0ZDlQeWZmSXc&hl=en_GB&authkey=COCjw-kG#gid=0)
* [Read the story](http://www.zeit.de/datenschutz/malte-spitz-data-retention)

— *Sascha Venohr, Zeit Online*
