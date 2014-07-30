# The Opportunity Gap

![figs/incoming/03-YY.png
](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-YY.png "Figure 27. The Opportunity Gap project (ProPublica)")

<center><small>Figure 27. The Opportunity Gap project (ProPublica)</small></center>

[The Opportunity Gap](http://projects.propublica.org/schools) used never-before-released U.S. Department of Education civil rights data and showed that some states, like Florida, have levelled the field and offer rich and poor students roughly equal access to high-level courses, while other states, like Kansas, Maryland and Oklahoma offer less opportunity in districts with poorer families.

The data included every public school in a district with 3,000 students or more. More than three-quarters of all public-school children were represented. A reporter in our newsroom obtained the data and our Computer Assisted Reporting Director cleaned it very extensively.

It was roughly a three-month project. Altogether, six people worked on the story and news application: two editors, a reporter, a CAR person, and two developers. Most of us weren’t all working on it exclusively throughout that period.

The project really required our combined skills — deep domain knowledge, an understanding of data best practices, design and coding skills, and so on. More importantly it required an ability to find the story in the data. It also took editing, not only for the story that went with it, but for the news app itself.

For the data cleaning and analysis we used mostly Excel and cleaning scripts, as well as MS Access. The news app was written in Ruby on Rails and uses JavaScript pretty extensively.

In addition to an overview story, our coverage included an interactive news application, which let readers understand and find examples within this large national data set that related to them. Using our news app, a reader could find their local school — say, for example, [Central High School in Newark, N.J.](http://goo.gl/HJVCf) — and immediately see how well the school does in a wide variety of areas. Then they could hit a button that says ‘[Compare to High and Low Poverty Schools](http://goo.gl/WrAIi)’, and immediately see other high schools, their relative poverty, and the extent to which they offer higher math, Advanced Placement, and other important courses. In our example, Central High is bookended by Millburn Sr. High. The Opportunity Gap shows how only 1% of Milburn students get Free or Reduced Price lunch but 72% of them are taking at least one AP course. In the other extreme, International High has 85% of its students getting Free/Reduced Price lunch and only 1% taking AP courses.

Through this example a reader can use something they know — a local high school — to understand something they don’t know — the distribution of educational access, and the extent to which poverty is a predictor of that access.

We also integrated the app with Facebook, so readers could log in to Facebook and our app would automatically let them know about schools that might interest them.

Traffic to all of our news apps are excellent, and we’re particularly proud of the way this app tells a complex story — and more to the point, helps readers tell their own particular story for themselves.

As with many projects that start with government data, the data needed a lot of cleaning. For instance, while there are only around 30 possible Advanced Placement courses, some schools reported having hundreds of them. This took lots of manual checking and phone calls to schools for confirmation and corrections.

We also worked really hard at making sure the app told a “far” story and a “near” story. That is, the app needed to present the reader with a broad, abstract national picture — specifically, a way to compare how states did relative to each other on educational access. But given that abstraction sometimes leaves readers confused as to what the data means to them, we also wanted readers to be able to find their own local school and compare it to high and low-poverty schools in their area.

If I were to advise aspiring data journalists interested in taking on this kind of project, I’d say you have to know the material and be inquisitive! All of the rules that apply to other kinds of journalism apply here. You have to get the facts right, make sure you tell the story well, and crucially, make sure your news app doesn’t disagree with a story you’re writing — because if it does, one of the two might be wrong.

Also, if you want to learn to code, the most important thing is to start. You might like learning through classes or through books or videos — and all are available and quite good — but make sure you have a really good idea for a project and a deadline by which you’ve got to complete it. If there’s a story in your head that can only come out as a news app, then not knowing how to program won’t stop you!

— *Scott Klein, ProPublica*
