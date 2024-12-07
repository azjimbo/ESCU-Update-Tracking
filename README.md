Splunk Threat Research team (STRT) does a good job at keeping up with new analytics.  However, for smaller deployments it can be difficult to sort through what is applicable and/or what has changed when these new versions are available.  They have a solution for a larger organization to be able to track and test changes when they become available, but in smaller orgs, the ability to manage and maintain another tool is cumbersome.  I use this dashboard, which can go in any app, to track the changes when we get around to deploying an updated version.  There are two editions of this dashboard available.  The first is for folks who are not using Enterprise Security, and this one does not track notable actions.  The second one does.

These work off an embedded csv generating query (under 'Overview' in the Guidance panel).  To make this dashboard work, run this twice.  Once before and once after pushing the update.  Then select as the first source csv the earlier of those two, then the post update as the 'csv to compare'.  Hit submit and wha-la! There's your deltas between the two versions.

These also can serve as a backup of your saved searches/correlation searches.

Updated the non-w/notable one to include drilldown for updated search in new tab.
