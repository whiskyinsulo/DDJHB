# Covering the Public Purse with OpenSpending.org

![figs/incoming/03-PP-02.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-PP-02.png "Figure 34. Where Does My Money Go? (Open Knowledge Foundation)")

<center><small>Figure 34. Where Does My Money Go? (Open Knowledge Foundation)</small></center>

In 2007, Jonathan came to the Open Knowledge Foundation with a one page proposal for a project called [Where Does My Money Go?](http://www.wheredoesmymoneygo.org/), which aimed to make it easier for UK citizens to understand how public funds are spent. This was intended to be a proof-of-concept for a bigger project to visually represent public information, based on the pioneering work of Otto and Marie Neurath’s Isotype Institute in the 1940s.

The *Where Does My Money Go?* project enabled users to explore public data from a wide variety of sources using intuitive open source tools. We won an award to help to develop a prototype of the project, and later received from Channel 4’s 4IP to turn this into a fully fledged web application. Information design guru David McCandless (from [Information is Beautiful](http://www.informationisbeautiful.net/)) created several different views of the data which helped people relate to the big numbers — including the ‘Country and Regional Analysis’, which shows how money is disbursed in different parts of the country, and [‘Daily Bread’](http://wheredoesmymoneygo.org/dailybread.html), which shows citizens a breakdown of their tax contributions per day in pounds and pence.

![figs/incoming/03-PP-01.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-PP-01.png "Figure 35. The Where Does My Money Go? Daily Bread Tax Calculator (Open Knowledge Foundation)")

<center><small>Figure 35. The Where Does My Money Go? Daily Bread Tax Calculator (Open Knowledge Foundation)</small></center>

Around that time, the holy grail for the project was the cunningly acronymed [Combined Online Information System](http://data.gov.uk/dataset/coins) (or COINS) data, which was the most comprehensive and detailed database of UK government finance available. Working with Lisa Evans (before she joined the Guardian Datablog team), Julian Todd and Francis Irving (now of Scraperwiki fame), Martin Rosenbaum (BBC) and others, we filed numerous requests for the data — many of them unsuccessful.

When the data was finally released in mid 2010, it was widely considered a coup for transparency advocates. We were given advance access to the data to load it into our web application, and we received a significant attention from the press when this fact was made public. On the day of the release we had dozens of journalists showing up on our IRC channel to discuss and ask about the release, as well as to enquire about how to open and explore it (the files were tens of gigabytes in size). While some pundits claimed the massive release was so complicated it was effectively [obscurity through transparency](http://web.archive.org/web/20100614164226/http://www.silicon.com/management/public-sector/2010/06/10/tax-spend-revelations-buried-deep-in-whitehall-data-graveyard-39745912/), lots of brave journalists got stuck into the data to give their readers an unprecedented picture of how public funds are spent. The Guardian [live-blogged](http://www.guardian.co.uk/global/datablog/2010/jun/04/coins-treasury-data-live-blog) about the release and numerous other media outlets covered it, and gave analyzes of findings from the data.

It wasn’t long before we started to get requests and enquiries about running similar projects in other countries around the world. Shortly after launching [OffenerHaushalt](http://offenerhaushalt.de/) — a version of the project for the German state budget created by Friedrich Lindenberg — we launched [OpenSpending](http://openspending.org/), an international version of the project, which aimed to help users map public spending from around the world a bit like OpenStreetMap helped them to map geographical features. We implemented new designs with help from the talented Gregor Aisch, partially based on David McCandless’s original designs.

![figs/incoming/03-PP-03.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-PP-03.png "Figure 36. OffenerHaushalt, the German version of Where Does My Money Go? (Open Knowledge Foundation)")

<center><small>Figure 36. OffenerHaushalt, the German version of Where Does My Money Go? (Open Knowledge Foundation)</small></center>

With the OpenSpending project, we have worked extensively with journalists to acquire, represent, interpret and present spending data to the public. OpenSpending is first and foremost an enormous, searchable database of public spending — both high level budget information and transaction-level actual expenditure. On top of this are built a series of out of the box visualizations such as treemaps and bubbletrees. Anyone can load in their local council data and produce visualizations from it.

While initially we thought there would be a greater demand for some of our more sophisticated visualizations, after speaking to news organizations we realised that there were more basic needs that needed to be satisfied first, such as the the ability to embed dynamic tables of data in their blogposts. Keen to encourage news organizations to give the public access to the data alongside their stories — we built a widget for this too.

Our first big release was around the time of the first International Journalism Festival in Perugia. A group of developers, journalists and civil servants collaborated to load Italian data into the OpenSpending platform, which gave a rich view of how spending was broken down amongst central, regional and local administrations. It was covered in [Il Fatto Quotidiano](http://www.ilfattoquotidiano.it/2011/04/18/dati-aperti-e-trasparenza-in-convegno-a-roma/105192/), [Il Post](http://www.ilpost.it/2011/04/19/grafico-spesa-pubblica-italia/), [La Stampa](http://www3.lastampa.it/economia/sezioni/articolo/lstp/398705/), [Repubblica](http://www.repubblica.it/tecnologia/2011/04/19/news/spesa_pubblica_e_bilanci_comunali_la_via_italiana_agli_open_data-15152320/), and [Wired Italia](http://daily.wired.it/news/economia/2011/04/19/open-spending.html), as well as in the [Guardian](http://www.guardian.co.uk/news/datablog/2011/apr/19/italy-public-spending).

![figs/incoming/03-PP-04.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-PP-04.png "Figure 37. The Italian version of Where Does My Money Go? (La Stampa)")

<center><small>Figure 37. The Italian version of Where Does My Money Go? (La Stampa)</small></center>

In 2011 we worked with [Publish What You Fund](http://www.publishwhatyoufund.org/) and the [Overseas Development Institute](http://www.odi.org.uk/) to map aid funding to Uganda from 2003-2006. This was new because for the fist time you could see aid funding flows alongside the national budget — enabling you to see to what extent the priorities of donors aligned with the priorities of governments. There were some interesting conclusions, for example both counter HIV programmes and family planning emerged as almost entirely funded by external donors. This was covered in the [Guardian](http://www.guardian.co.uk/global-development/poverty-matters/2011/nov/25/uganda-aid-confusion-analyze-spending?newsfeed=true).

We’ve also been working with NGOs and advocacy groups to cross-reference spending data with other sources of information. For example, Privacy International approached us with a big list of surveillance technology companies and a list of agencies attending a well known international surveillance trade show, known colloquially as the ‘wiretappers ball’. By systematically cross-referencing company names with spending datasets, it was possible to identify which companies had government contracts — which could then be followed up with FOI requests. This was covered by the [Guardian](http://www.guardian.co.uk/news/datablog/2012/feb/07/surveillance-shows-attendees-iss-world) and the [Wall Street Journal](http://blogs.wsj.com/digits/2012/02/06/high-tech-surveillance-comes-to-small-towns/?KEYWORDS=privacy).

We’re currently working to increase fiscal literacy among journalists and the public as part of a [project called Spending Stories](http://jwyg.okfn.org/2011/06/22/faq-for-spending-stories/), which lets users link public spending data to public spending related stories to see the numbers behind the news, and the news around the numbers.

Through our work in this area, we’ve learned that:

* Journalists are often not used to working with raw data, and many don’t consider it a necessary foundation for their reporting. Sourcing stories from raw information is still a relatively new idea.
* analyzing and understanding data is a time-intensive process, even with the necessary skills. Fitting this into a short-lived news cycle is hard, so data journalism is often used in longer-term, investigative projects.
* Data released by governments is often incomplete or outdated. Very often, public databases cannot be used for investigative purposes without the addition of more specific pieces of information requested through FOI.
* Advocacy groups, scholars and researchers often have more time and resources to conduct more extensive data-driven research than journalists. It can be very fruitful to team up with them, and to work in teams.

— *Lucy Chambers and Jonathan Gray, Open Knowledge Foundation*
