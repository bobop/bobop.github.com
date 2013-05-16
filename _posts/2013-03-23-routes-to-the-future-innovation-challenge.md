---
layout: post
title: Routes to the Future - Innovation Challenge
---

I'm writing this in the last hour of the [Innovation Challenge](http://futureeverything.org/summit/conference/workshops-fringe-events/innovation-challenge/) staged by Future Everything and TFGM. I've been here at 4 Piccadilly Place for 31 hours and managed to get a few hours kip at around 3am!

I didn't come to enter any of the competitions, I came to build an API from the newly released GTFS Transport schedule data released by [TFGM](http://www.tfgm.com/Pages/default.aspx) this week. I built [GMBusTimes](http://gmbustimes.com/) at the Lovely Data Hackathon a couple of years ago and it used a SPARQL endpoint for it's bus schedule data provided by Swirrl. However, they removed the data and the endpoint a few months ago and GMBusTimes has been broken since. I also wanted to have some control over the API so I could fix any issues and ensure it was available over the long term.

So I built [http://gtfsapi.herokuapp.com](http://gtfsapi.herokuapp.com/) to provide a RESTful API providing json formatted results for the GMBusTimes app, and for any other apps I and others want to build.

I haven't managed to complete the integration of the new API with GMBusTimes, and I started the "Bus Fair" idea to use the API too:&nbsp;[http://busfair.herokuapp.com](http://busfair.herokuapp.com/)

It's been alot of fun and very tiring and I'm looking forward to the presentations from the other teams a bit later.
