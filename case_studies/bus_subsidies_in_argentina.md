# Bus Subsidies in Argentina

Since 2002 subsidies for the public bus transportation system in Argentina have been growing exponentially, breaking a new record every year. But in 2011, after winning the elections, Argentina´s new government announced cuts in subsidies for public services starting December of the same year. At the same time the national government decided to transfer to the City of Buenos Aires government the administration of the local bus lines and metro lines. As the transfer of subsidies to this local government hasn’t been clarified and due to lack of sufficient local funds to guarantee the safety of the transportation system, the government of the City of Buenos Aires rejected this decision.

As this was happening my colleagues at La Nación and I were meeting for the first time to discuss how to start our own data journalism operation. Our Financial Section Editor suggested that the subsidies data published by the [Secretaría de Transporte](http://www.transporte.gov.ar/) (the Department of Transportation) would be a good challenge to start with as it was very difficult to make sense of due to the format and the terminology.

The poor conditions of the public transportation system impact the life of more than 5.800.000 passengers everyday. Delays, strikes, vehicle breakdowns or even accidents are often happening. We thus decided to look into where the subsidies for the public transportation system in Argentina go and make this data easily accessible to all Argentinian citizens by means of a “Transport Subsidies Explorer”, which is currently in the making.

![figs/incoming/03-LL-01.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-LL-01.jpg "Figure 48. The Transport Subsidies Explorer (La Nación)")

<center><small>Figure 48. The Transport Subsidies Explorer (La Nación)</small></center>

We started with calculating how much bus companies receive every month from the government. To do this we look at the data published on the [website of the Department of Transportation](http://www.transporte.gov.ar/content/subsidios-sistau/0 where more than 400 PDFs containing monthly cash payments towards more than 1300 companies since 2006 were published.

![figs/incoming/03-LL-02.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-LL-02.jpg "Figure 49. Ranking subsidised transport companies (La Nación)")

<center><small>Figure 49. Ranking subsidised transport companies (La Nación)</small></center>

We teamed up with a senior programmer to develop a scraper in order to automate the regular download and conversion of these PDFs into Excel and Database files. We are using the resulting dataset with more than 285.000 records for our investigations and visualizations, in both print and online. Additionally, we are making this data available in machine readable format for every Argentinian to reuse and share.

The next step was to identify how much the monthly maintenance of a public transport vehicle costed the government on average. To find this out we went to another government website, that of the [Comisión Nacional de Regulación del Transporte](http://www.cnrt.gov.ar/index2.htm) (The National Commission for the Regulation of Transport), CNRT, responsible for regulating transportation in Argentina. On this website we found a list of bus companies which altogether owned 9000 vehicles. We developed a normalizer to allow us to reconcile bus company names and cross-reference the two datasets.

To proceed we needed the registration number of each vehicle. We found on the CNRT website a list of vehicles per bus line per company with their license plates. Vehicle registration numbers in Argentina are composed of letters and numbers that corresponds to the vehicle’s “age”. For example my car has the IDF234 and the “I” corresponds to March-April 2011. We reverse engineered the license plates for buses belonging to all listed companies to find out the average age of buses per company and thus be able to show how much money goes to each company and compare the amounts based on the average age of their vehicles.

![figs/incoming/03-LL-03.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-LL-03.jpg "Figure 50. Comparing age of fleets to the amount of money they receive from government (La Nación)")

<center><small>Figure 50. Comparing age of fleets to the amount of money they receive from goernment (La Nación)</small></center>

In the middle of this process the content of the government released PDFs containing the data we needed mysteriously changed although the URLs and names of the files remained the same. One of the things that has changed was that some PDFs were now missing the vertical "totals", making it impossible to cross-check totals across all the entire investigated time period, 2002-2011.

We took this case to a hackathon organised by Hacks/Hackers in Boston where developer Matt Perry generously created what we call the “PDF Spy.” This application won the "Most Intriguing” category in that event. The [PDF Spy](http://gristlabs.com/2011/09/24/pdfspy/) points at a Web page full of PDFs and checks if the content within the PDFs has changed. “Never be fooled by ‘government transparency' again,” writes Matt Perry.

###Who worked on the project?

A team of seven journalists, programmers and an interactive designer have been working on this investigation for 13 months.

The skills we needed for this project were:

* Journalists with knowledge of how the subsidies for the public transportation system work and what the risks were; knowledge of the bus companies market.
* A programmer skilled in Web scraping, parsing and normalising data, extracting data from PDFs into Excel spreadsheets.
* A statistician for conducting the data analysis and the different calculations
* A designer for producing the interactive data visualizations.

###What tools did we use?

We used VBasic for applications, Excel Macros, Tableau Public and Junar Open Data Platform as well as Ruby on Rails, the Google charts API and Mysql for the Subsidies Explorer.

The project had a great impact. We’ve had tens of thousands of views and the investigation was featured on the front page of La Nación’s print edition.

The success of this first data journalism project helped us internally to make the case for establishing a data operation that would cover investigative reporting and providing service to the public. This resulted in Data.lanacion.com.ar, a platform where we publish data on various topics of public interest in machine readable format.

— *Angélica Peralta Ramos, La Nación, Argentina*
