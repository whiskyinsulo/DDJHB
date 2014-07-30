# Mapa76 Hackathon

![figs/incoming/03-MM.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-MM.png "Figure 41. Mapa76 (Hacks/Hackers Buenos Aires)")

<center><small>Figure 41. Mapa76 (Hacks/Hackers Buenos Aires)</small></center>

We opened the [Buenos Aires chapter of Hacks/Hackers](http://www.meetup.com/HacksHackersBA/) in April 2011. We hosted two initial meetups to publicize the idea of greater collaboration between journalists and software developers, with between 120 and 150 people at each event. For a third meeting we had a 30-hour hackathon with eight people at a digital journalism conference in the city of Rosario, 300 kilometers from Buenos Aires.

A recurring theme in these meetings was the desire to scrape large volumes of data from the web, and then to represent it visually. To help with this a project called Mapa76.info was born, which helps users to extract data, and then to display it using maps and timelines. Not an easy task.

Why Mapa76? On March 24, 1976 there was a coup in Argentina, which lasted until 1983. In that period there were an estimated 30,000 disappeared people, thousands of deaths, and 500 children born in captivity appropriated for the military dictatorship. Over 30 years later, the number of people in Argentina convicted of crimes against humanity committed during the dictatorship amounts to 262 people (September 2011). Currently there are 14 ongoing trials and 7 with definite starting dates. There are 802 people in various open court cases.

These prosecutions generate large volumes of data that are difficult for researchers, journalists, human rights organizations, judges, prosecutors, and others to process. Data is produced in a distributed manner and investigators often don’t take advantage of software tools to assist them with interpreting in. Ultimately this means that facts are often overlooked and hypotheses are often limited. Mapa76 is an investigative tool providing open access to this information for journalistic, legal, juridical, and historical purposes.

To prepare for the hackathon we created a platform which developers and journalists could use to collaborate on the day of the event. Martin Sarsale developed some basic algorithms to extract structured data from simple text documents. Some libraries were also used from DocumentCloud.org project, but not many. The platform would automatically analyze and extract names, dates and places from the texts — and would enable users to explore key facts about different cases (e.g. date of birth, place of arrest, alleged place of disappearance and so on).

Our goal was to provide a platform for the automatic extraction of data on the judgments of the military dictatorship in Argentina. We wanted to a way of automatically (or at least semi-automatically) displaying key data related to cases from 1976-1983 based on written evidence, arguments and judgments. The extracted data (names, places and dates) are collected, stored and can be analyzed and refined by the researcher, as well as being explored using maps, timelines and network analysis tools.

The project will allow journalists and investigators, prosecutors and witnesses to follow the story of a person’s life, including the course of their captivity and subsequent disappearance or release. Where information is absent, users can comb through a vast number of documents for information which could be of possible relevance to the case.

For the hackathon, we made a public announcement through [Hacks/Hackers Buenos Aires](http://www.meetup.com/HacksHackersBA/), which then had around 200 members (at the time of writing there are around 540). We also contacted many Human Rights associations. The meeting was attended by about forty people including journalists, advocacy organizations, developers and designers.

During the hackathon, we identified tasks that different types of participants could pursue independently to help things run smoothly. For example, we asked designers to work on an interface that combining maps and timelines, we asked developers to look into ways of extracting structured data and algorithms to disambiguate names, and we asked journalists to look into what happened with specific people, to compare different versions of stories, and to comb through documents to tell stories about particular cases.

Probably the main problem we had after the hackathon was that our project was very ambitious, our short-term objectives were demanding, and it is hard to coordinate a loose-knit network of volunteers. Nearly everyone involved with the project had a busy day job and many also participated in other events and projects. Hacks/Hackers Buenos Aires had 9 meetings in 2011.

The project is currently under active development. There is a core team of four people working with over a dozen collaborators. We have a [public mailing list](http://groups.google.com/group/mapa76-dev/) and [code repository](https://github.com/mapa76/) through which anyone can get involved with the project.

— *Mariano Blejman, Hacks/Hackers Buenos Aires*
