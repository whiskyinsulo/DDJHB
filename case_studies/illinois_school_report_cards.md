# Illinois School Report Cards

![figs/incoming/03-EE.png](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-EE.png "Figure 43. 2011 Illinois School Report Cards (Chicago Tribune)")

<center><small>Figure 43. 2011 Illinois School Report Cards (Chicago Tribune)</small></center>

Each year, the Illinois State Board of Education releases school "report cards", data on the demographics and performance of all the public schools Illinois. It’s a massive dataset, this year’s drop was *~9,500 columns* wide. The problem with that much data is choosing what to present. (As with any software project, the hard part is not *building* the software, but building the *right* software.)

We worked with the reporters and editor from the education team to choose the interesting data. (There’s a lot of data out there that seems interesting but which a reporter will tell you is actually flawed or misleading.)

We also surveyed and interviewed folks with school-age kids in our newsroom. We did this because of an empathy gap — nobody on the news apps team has school-age kids. Along the way, we learned much about our users and much about the usability (or lack thereof!) of the previous version of our schools site.

We aimed to design for a couple specific users and use cases: (1) parents with a child in school who want to know how their school measures up, and (2) parents who’re trying to sort out where to live, since school quality often has a major impact on that decision.

The first time around, the schools site was about a six week, two developer project. Our 2011 update was a four week, two developer project. (There were actually three people actively working on the recent project, but none were full-time, so it adds up to about two.)

A key piece of this project was information design. Although we present far less data than is available, it’s still a lot of data, and making it digestible was a challenge. Luckily, we got to borrow someone from our graphics desk — a designer who specialises in presenting complicated information. He taught us much about chart design and, in general, guided us to a presentation that is readable, but does not underestimate the reader’s ability or desire to understand the numbers.

The site was built in Python and Django. The data is housed in MongoDB — the schools data is heterogeneous and hierarchical, making it a poor fit for a relational database. (Otherwise we probably would have used PostgreSQL.)

We experimented for the first time with Twitter’s Bootstrap user interface framework on this project, and were happy with the results. The charts are drawn with Flot.

The app is also home to the many stories about school performance that we’ve written. It acts as sort of a portal in that way — when there’s a new school performance story, we put it at the top of the app, alongside lists of schools relevant to the story. (And when a new story hits, readers of chicagotribune.com are directed to the app, not the story.)

Early reports are that readers love the schools app. The feedback we’ve received has been largely positive (or at least constructive!), and page views are through the roof. As a bonus, this data will remain interesting for a full year, so although we expect the hits to tail off as the schools stories fade from the homepage, our past experience is that readers have sought out this application year-round.

A few key ideas we took away from this project are:

* The graphics desk is your friend. They’re good at making complex information digestible.
* Ask the newsroom for help. This is the second project for which we’ve conducted a newsroom-wide survey and interviews, and it’s a great way to get the opinion of thoughtful people who, like our audience, are diverse in background and generally uncomfortable with computers.
* Show your work! Much of our feedback has been requests for the data that the application. We’ve made a lot of the data publicly available via an API, and we will shortly release the stuff that we didn’t think to include initially.

— *Brian Boyer, Chicago Tribune*
