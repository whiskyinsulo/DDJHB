# Data in the News: Wikileaks

![figs/incoming/03-GG.jpg](http://datajournalismhandbook.org/1.0/en/figs/incoming/03-GG.jpg "Figure 40. The Wikileaks War Logs (The Guardian)")

<center><small>Figure 40. The Wikileaks War Logs (The Guardian)</small></center>

It began with one of the investigative reporting team asking: “You’re good with spreadsheets, aren’t you?” And this was one hell of a spreadsheet: 92,201 rows of data, each one containing a detailed breakdown of a military event in Afghanistan. This was the [WikiLeaks war logs](http://www.guardian.co.uk/news/datablog+world/the-war-logs). Part one, that is. There were to be two more episodes to follow: Iraq and the cables. The official term was SIGACTS: the US military significant actions database.

The Afghanistan war logs — shared with the New York Times and Der Spiegel — was data journalism in action. What we wanted to do was enable our team of specialist reporters to get great human stories from the information — and we wanted to analyze it to get the big picture, to show how the war really is going.

It was central to what we would do quite early on that we would not publish the full database. Wikileaks was already going to do that and we wanted to make sure that we didn’t reveal the names of informants or unnecessarily endanger Nato troops. At the same time, we needed to make the data easier to use for our team of investigative reporters led by David Leigh and Nick Davies (who had negotiated releasing the data with Julian Assange). We also wanted to make it simpler to access key information, out there in the real world — as clear and open as we could make it.

The data came to us as a huge excel file — over 92,201 rows of data, some with nothing in at all or poorly formatted. It didn’t help reporters trying to trawl through the data for stories and was too big to run meaningful reports on.

Our team built a simple internal database using SQL. Reporters could now search stories for key words or events. Suddenly the dataset became accessible and generating stories became easier.

The data was well structured: each event had the following key data: time, date, a description, casualty figures and — crucially — detailed latitude and longitude.

We also started filtering the data to help us tell one of the key stories of the war: the rise in IED (improvised explosive device) attacks — home-made roadside bombs which are unpredictable and difficult to fight. This dataset was still massive — but easier to manage. There were around 7,500 IED explosions or ambushes (an ambush is where the attack is combined with, for example, small arms fire or rocket grenades) between 2004 and 2009. There were another 8,000 IEDs which were found and cleared. We wanted to see how they changed over time — and how they compared. This data allowed us to see that the south, where British and Canadian troops were based then, was the worst-hit area — which backed-up what our reporters who had covered the war knew.

The Iraq war logs release in October 2010 dumped another 391,000 records of the Iraq war into the public arena.

This was in a different league to the Afghanistan leak — there’s a good case for saying this made the war the most documented in history. Every minor detail was now there for us to analyze and break down. But one factor stands out: the sheer volume of deaths, most of which are civilians.

As with Afghanistan, the Guardian decided not to republish the entire database, largely because we couldn’t be sure the summary field didn’t contain confidential details of informants and so on.

But we did allow our users to download a spreadsheet containing the records of every incident where somebody died, nearly 60,000 in all. We removed the summary field so it was just the basic data: the military heading, numbers of deaths and the geographic breakdown.

We also took all these incidents where someone had died and [put it on a map using Google Fusion tables](http://www.guardian.co.uk/world/datablog/interactive/2010/oct/23/wikileaks-iraq-deaths-map). It was not perfect, but a start in trying to map the patterns of destruction which had ravaged Iraq.

December 2010 saw the release of the cables. This was in another league altogether, a huge dataset of official documents: 251,287 dispatches, from more than 250 worldwide US embassies and consulates. It’s a unique picture of US diplomatic language — including over 50,000 documents covering the current Obama administration. But what did the data include?

The cables themselves came via the huge Secret Internet Protocol Router Network, or SIPRNet. SIPRNet is the worldwide US military internet system, kept separate from the ordinary civilian internet and run by the Department of Defense in Washington. Since the attacks of September 2001, there had been a move in the US to link up archives of government information, in the hope that key intelligence no longer gets trapped in information silos or “stovepipes”. An increasing number of US embassies have become linked to SIPRNet over the past decade, so that military and diplomatic information can be shared. By 2002, 125 embassies were on SIPRNet: by 2005, the number had risen to 180, and by now the vast majority of US missions worldwide are linked to the system — which is why the bulk of these cables are from 2008 and 2009. As David Leigh wrote:

An embassy dispatch marked SIPDIS is automatically downloaded on to its embassy classified website. From there, it can be accessed not only by anyone in the state department, but also by anyone in the US military who has a security clearance up to the ‘Secret’ level, a password, and a computer connected to SIPRNet

…which astonishingly covers over 3 million people. There are several layers of data in here; all the way up to SECRET NOFORN, which means that they are designed never be shown to non-US citizens. Instead, they are supposed to be read by officials in Washington up to the level of Secretary of State Hillary Clinton. The cables are normally drafted by the local ambassador or subordinates. The “Top Secret” and above foreign intelligence documents cannot be accessed from SIPRNet.

Unlike the previous releases, this was predominantly text, not quantified or with identical data. This is what was included:

####A source
The embassy or body which sent it

####A list of recipients
Normally cables were sent to a number of other embassies and bodies

####A subject field
Basically a summary of the cable

####Tags
Each cable was tagged with a number of keyword abbreviations.

####Body text
The cable itself. We opted not to publish these in full for obvious security reasons

One interesting nuance of this story is how the cables have almost created leaks on demand. They led the news for weeks on being published — but now, whenever a story comes up about some corrupt regime or international scandal, access to the cables gives us access to new stories.

Analysis of the cables is an enormous task which may never be entirely finished.

— *This is an edited version of a chapter first published in Facts are Sacred: the power of data by Simon Rogers, The Guardian*
