---
layout: post
title: Trafford Open Data Maps
---

![](http://www.trafford.gov.uk/common/images/header/council-logo.png "trafford-council-logo")

In the last couple of weeks I've created a couple of apps based on Open Data from [Trafford Counci](http://www.trafford.gov.uk/opendata/)l. Trafford and [Salford Councils](http://www.salford.gov.uk/opendata.htm)&nbsp;are the only 2 Councils in Greater Manchester to have any Open Data and Salford doesn't have that much.

Trafford however released the locations of all sorts of things, from Libraries to Trees, Allotments to Recycling Centres, and I've mapped them!

[Trafford Open Data Maps](http://traffordopendata.heroku.com)

Here's the geeky/techy explanation about how I made this app:

![](http://s3.amazonaws.com/bobob_prod/medium/3/tod.jpg?1320611853 "traffordod")

The data Trafford Council provides is in XML format but I needed to get it into a databse so I could quickly query the data. This was particularly important for the Trees because there are 15,000 of them and the XML file was over 4MB which would have taken a long time to load and read and plot on a map. Having the tree data in a database makes it much quicker to access the tree data.

Since I'm a [Ruby On Rails](http://rubyonrails.org)&nbsp;developer, I chose to create a simple Rails application to import the data from the XML files into a MySQL database, and then to query the database to plot the location of the items on a Google Map. This was pretty straight forward for most of the data sets, but the Bus Stops and Trees were a different ball game.

There are nearly 1,600 Bus Stops and over 15,000 Trees, so to plot them all on a map of Trafford would take a while and clutter the map with the marker icons to the point of it not being useful. So I created some nifty code so that only 300 trees are on the map at any time. This helps the visualisation of the markers on the map by plotting just enough trees to make the map still understandable. Then when you zoom into the map more trees are loaded so that when you are zoomed in far enough, all the trees in the area you are looking at are plotted. This is the same process with the Bus Stops.

I also used the URN numbers of the Schools to create links to their [OFSTED](http://www.ofsted.gov.uk) page and their [EDUBASE](http://www.edubase.gov.uk)&nbsp;page so that the Schools map is more useful.

The Parks And Open Spaces, Recycling Centres, Schools and Trees pages also have Info boxes below the maps displaying some stats for those data sets. The place names and tree names link to Wikipedia articles to provide more context and images.

![](http://timharvey.net/wp-content/heroku_logo.png "2008-02-09-1")

To get the app off my computer and onto the web for all to see, I deployed it to [Heroku](http://heroku.com)&nbsp;which offers free hosting for Ruby On Rails applications. It was the first time I used Heroku and I found it really easy and quick and free Rails hosting is hard to argue with! Their limit for free hosting is that your database can't be over 5MB, and this is the reason I haven't included the 27,000 Streetlights!

If you have any ideas for new features or ways to interact with these maps, or want to contribute your time and skills, please let me know by leaving a comment below or emailing me at [ben@bobop.co.uk](mailto:ben@bobop.co.uk).