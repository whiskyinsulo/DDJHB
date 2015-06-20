# Basic Steps in Working with Data

There are at least three key concepts you need to understand when starting a data project:

* Data requests should begin with a list of questions you want to answer.
* Data often is messy and needs to be cleaned.
* Data may have undocumented features

![figs/incoming/05-MM.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/05-MM.png "Figure 69. Messy Data")

<small>Figure 69. Messy Data</small>

###Know the Questions You Want to Answer

In many ways, working with data is like interviewing a live source. You ask questions of the data and get it to reveal the answers. But just as a source can only give answers about which he or she has information, a data set can only answer questions for which it has the right records and the proper variables. This means that you should consider carefully what questions you need to answer even before you acquire your data. Basically, you work backwards. First, list the data-evidenced statements you want to make in your story. Then decide which variables and records you would have to acquire and analyze in order to make those statements.

Consider an example involving local crime reports. Let’s say you want to do a story looking at crime patterns in your city, and the statements you want to make involve the times of day and the days of a week in which different kinds of crimes are most likely to happen, as well as what parts of town are hot spots for various crime categories.

You would realize that your data request has to include the date and the time each crime was reported, the kind of crime (murder, theft, burglary, etc.) as well as the address of where the crime occurred. So Date, Time, Crime Category and Address are the minimum variables you need to answer those questions.

But be aware that there are a number of potentially interesting questions that this four-variable data set CAN’T answer, like the race and gender of victims, or the total value of stolen property, or which officers are most productive in making arrests. Also, you may only be able to get records for a certain time period, like the past three years, which would mean you couldn’t say anything about whether crime patterns have changed over a longer period of time. Those questions may be outside of the planned purview of your story, and that’s fine. But you don’t want to get into your data analysis and suddenly decide you need to know what percentage of crimes in different parts of town are solved by arrest.

One lesson here is that it’s often a good idea to request ALL the variables and records in the database, rather than the subset that could answer the questions for the immediate story. (In fact, getting all the data can be cheaper than getting a subset, if you have to pay the agency for the programming necessary to write out the subset.) You can always subset the data on your own, and having access to the full data set will let you answer new questions that may come up in your reporting and even produce new ideas for follow-up stories. It may be that confidentiality laws or other policies mean that some variables, such as the identities of victims or the names of confidential informants, can’t be released. But even a partial database is much better than none, as long as you understand which questions the redacted database can and can’t answer.

###Cleaning Messy Data

One of the biggest problems in database work is that often you will be using for analysis reasons data that has been gathered for bureaucratic reasons. The problem is that the standard of accuracy for those two is quite different.

For example, a key function of a criminal justice system database is to make sure that defendant Jones is brought from the jail to be in front of Judge Smith at the time of his hearing. For that purpose, it really doesn’t matter a lot if Jones' birth date is incorrect, or that his street address is misspelled, or even if his middle initial is wrong. Generally, the system still can use this imperfect record to get Jones to Smith’s courtroom at the appointed time.

But such errors can skew a data journalist’s attempts to discover the patterns in the database. For that reason, the first big piece of work to undertake when you acquire a new data set is to examine how messy it is and then clean it up. A good quick way to look for messiness is to create frequency tables of the categorical variables, the ones that would be expected to have a relatively small number of different values. (When using Excel, for instance, you can do this by using Filter or Pivot Tables on each categorical variable.)

Take “Gender”, an easy example. You may discover that your Gender field includes any of a mix of values like these: Male, Female, M, F, 1, 0, MALE, FEMALE, etc., including misspellings like ‘Femal’. To do a proper gender analysis, you must standardise - decide on M and F, perhaps - and then change all the variations to match the standards. Another common database with these kinds of problems are American campaign finance records, where the Occupation field might list “Lawyer”, “Attorney”, “Atty”, “Counsel”, “Trial Lawyer” and any of a wealth of variations and misspellings; again, the trick is to standardise the occupation titles into a shorter list of possibilities.

Data cleanup gets even more problematic when working with names. Are “Joseph T. Smith”, “Joseph Smith”, “J.T. Smith”, “Jos. Smith” and “Joe Smith” all the same person? It may take looking at other variables like address or date of birth, or even deeper research in other records, to decide. But tools like Google Refine can make the cleanup and standardisation task faster and less tedious.

###Data May Have Undocumented Features

The Rosetta Stone of any database is the so-called data dictionary. Typically, this file (it may be text or PDF or even a spreadsheet) will tell you how the data file is formatted (delimited text, fixed width text, Excel, dBase, et al.), the order of the variables, the names of each variable and the datatype of each variable (text string, integer, decimal, et al.) You will use this information to help you properly import the data file into the analysis software you intend to use (Excel, Access, SPSS, Fusion Tables, any of various flavors of SQL, et al.)

The other key element of a data dictionary is an explanation of any codes being used by particular variables. For instance, Gender may be coded so that ‘1=Male’ and ‘0=Female’. Crimes may be coded by your jurisdiction’s statute numbers for each kind of crime. Hospital treatment records may use any of hundreds of 5-digit codes for the diagnoses of the conditions for which a patient is being treated. Without the data dictionary, these data sets could be difficult or even impossible to analyze properly.

But even with a data dictionary in hand, there can be problems. An example happened to reporters at the Miami Herald in Florida some years ago when they were doing an analysis of the varying rates of punishment that different judges were giving to people arrested for driving while intoxicated. The reporters acquired the conviction records from the court system and analyzed the numbers in the three different punishment variables in the data dictionary: amount of prison time given, amount of jail time given, and amount of fine given. These numbers varied quite a bit amongst the judges, giving the reporters' evidence for a story about how some judges were harsh and some were lenient.

But for every judge, about 1-2 percent of the cases showed no prison time, no jail time and no fine. So the chart showing the sentencing patterns for each judge included a tiny amount of cases as “No punishment,” almost as an afterthought. When the story and chart was printed, the judges howled in complaint, saying the Herald was accusing them of breaking a state law that required that anyone convicted of drunk driving be punished.

So the reporters went back to Clerk of the Court’s office that had produced the data file and asked what had caused this error. They were told that the cases in question involved indigent defendants with first-time arrests. Normally they would be given a fine, but they had no money. So the judges were sentencing them to community service, such as cleaning litter along the roads. As it turned out, the law requiring punishment had been passed after the database structure had been created. So all the court clerks knew that in the data, zeros in each of the prison-jail-fine variables meant community service. However, this WASN’T noted in the data dictionary, and therefore caused a Herald correction to be written.

The lesson in this case is to always ask the agency giving you data if there are any undocumented elements in the data, whether it is newly-created codes that haven’t been included in the data dictionary, changes in the file layout, or anything else. Also, always examine the results of your analysis and ask “Does this make sense?” The Herald reporters were building the chart on deadline and were so focused on the average punishment levels of each judge that they failed to pay attention to the scant few cases that seemed to show no punishment. They should have asked themselves if it made sense that all the judges seemed to be violating state law, even if only to a tiny degree.

— *Steve Doig, Walter Cronkite School of Journalism of Arizona State University*

.
