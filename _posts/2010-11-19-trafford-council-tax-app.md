---
layout: post
title: Trafford Council Tax App
---

I've been developing a few websites based on the Open Data from Trafford Council including the [Trafford Open Data Maps](http://traffordopendata.heroku.com/) site and the [Trafford Supplier Spend](http://traffordspending.heroku.com/) site.

They then released the data of the [Council Tax bands](http://www.trafford.gov.uk/opendata/) each of the 90,000+ properties in Trafford and I had to map that, it's such juicy data!

[Trafford Council Tax](http://traffordcounciltax.heroku.com/)

![](http://s3.amazonaws.com/bobob_prod/medium/5/tct.jpg?1320612664 "traffordcounciltax")

When I heard that this data was released, my immediate thought was that I's want to check the tax bands of the houses on my street if I lived in Trafford. So I created a way to search for your street and then to see the colour coded markers for the houses on your street, which would produce something like this: [http://j.mp/9pEZBo](http://j.mp/9pEZBo)

Trafford Council also released the historical data on the tax band charges since 1993 so I used the [Google Visualisation](http://code.google.com/apis/visualization/interactive_charts.html) tool to create an interactive barchart showing how the charges have risen over the year. [See the interactive bar chart here](http://traffordcounciltax.heroku.com/taxbands).

As with my other Open Data apps, I deployed the app to Heroku which offers free and easy hosting for small Ruby On Rails apps.

I have been surprised that the [Tree Map](http://traffordopendata.heroku.com/trees) has got the most attention even though this Council Tax app is more controversial. Maybe it's because people don't know I've done this yet. Well, at least you do now!