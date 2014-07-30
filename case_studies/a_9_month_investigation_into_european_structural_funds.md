# A 9 Month Investigation into European Structural Funds

![figs/incoming/03-OO-01.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-OO-01.png "Figure 28. EU Structural Funds Investigation (Bureau of Investigative Journalism)")

<center><small>Figure 28. EU Structural Funds Investigation (Bureau of Investigative Journalism)</small></center>

In 2010, the [Financial Times](http://www.ft.com/intl/eu-funds) and the [Bureau of Investigative Journalism (BIJ)](http://www.thebureauinvestigates.com/category/projects/europes-hidden-billions/) joined forces to investigate European Structural Funds. The intention was to review who the beneficiaries of European Structural Funds are and check whether the money was put to good use. At €347bn over seven years Structural Funds is the second largest subsidy programme in the EU. The programme has existed for decades, but apart from broad, generalised overviews, there was little transparency about who the beneficiaries are. As part of a rule change in the current funding round, authorities are obliged to make public a list of beneficiaries, including project description and amount of EU and national funding received.

The project team was made up of up to 12 journalists and one full-time coder collaborating for nine months. Data gathering alone took several months.

The project resulted in five days of coverage in the Financial Times and the BIJ, a BBC radio documentary, and several TV documentaries.

Before you tackle a project of this level of effort, you have to be certain that the findings are original, and that you will end up with good stories nobody else has.

The process was broken up into a number of distinct steps:

1. **Identify who keeps the data and how it is kept**

 The European Commission’s Directorate General for the Regions have a portal to the websites of regional authorities that publish the data. We believed that the Commission would have an overarching database of project data that we could either access directly, or which we could obtain through a Freedom of Information request. No such database exists to the level of detail we required. We quickly realised that many of the links the Commission provided were faulty and that most of the authorities published the data in PDF format, rather than analysis-friendly formats such as CSV or XML.

 A team of up to 12 people worked on identifying the latest data and collating the links into one large spreadsheet we used for collaboration. Since the data fields were not uniform (for example headers were in different languages, some data sets used different currencies, some included breakdowns of EU and National Funding) we needed to be as precise as possible in translating and describing the data fields available in each data set.<br><br>

2. **Download and prepare the data**

 The next step consisted of downloading all the spreadsheets, PDFs and, in some cases, web scraping the original data.

 Each data set had to then be standardized. Our biggest task was extracting data out of PDFs, some hundreds of pages long. Much of this was done using UnPDF and ABBYY FineReader, which allow data to be extracted to formats such as CSV or Excel.

 It also involved checking and double checking that the PDF extraction tools had captured the data correctly. This was done using filtering, sorting and summing up totals (to ensure it corresponded with what was printed on the PDFs).<br><br>

3. **Create a database**

 The team’s coder set up a SQL database. Each of the files prepared were then used as a building block for the overall SQL database. A once a day process would upload all the individual data files into one large SQL database, which could be queried on the fly through its front end by using queries.<br><br>

4. **Double-checking and analysis**

 The team analyzed the data in two main ways:

 #####Via the database front end

  This entailed typing particular keywords of interest (e.g. "tobacco", "hotel", "company A" in to the search engine. With help of Google Translate, which was plugged into the search functionality of our database, those keywords would be translated into 21 languages and would return appropriate results. These could be downloaded and reporters could do further research on the individual projects of interest.

 #####By macro-analysis using the whole database

 Occasionally, we would download a full data set, which could then be analyzed for example using keywords, or aggregating data by country, region, type of expenditure, number of projects by beneficiary etc.

Our story lines were informed by both these analyzes, but also through on the ground and desk research.

Double-checking the integrity of the data (by aggregating and checking against what authorities said had been allocated) took a substantial amount of time. One of the main problems was that authorities would for the most part only divulge the amount of "EU and national funding". Under EU rules, each program is allowed to fund a certain percentage of the total cost using EU funding. The level of EU funding is determined, at program level, by the so-called co-financing rate. Each program (e.g. regional competitiveness) is made up of numerous projects. At the project levels, technically one project could receive 100 per cent EU funding, and another none at all, as long as grouped together, the amount of EU funding at the program level is not more than the approved co-financing rate.

This meant that we needed to check each EU amount of funding we cited in our stories with the beneficiary company in question.

— *Cynthia O’Murchu, Financial Times*
