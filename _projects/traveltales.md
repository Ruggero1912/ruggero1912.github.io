---
layout: project
name: TravelTales
short_description: An in-car oriented service that plays audio news personalized on passengers' interests. 
image: /assets/images/traveltales/travel-tales.png
technologies: Python
authors: "Giacomo Pacini, Enrico Nello, Matteo Pierucci"
date: 2024-01-16
priority: 10
github: https://github.com/enricollen/TravelTales
---

Consider the situation in which you are traveling with other people that have different interests, and you do not know what to talk about.

You could play some radio news or listen to pop music, but maybe you and the others share some common interests to specific topics. It would be great to discover it and talk about them!

<!-- Listening to generalistic radio news

When traveling together with other people it is 

Current solutions
 -->



### What is TravelTales

TravelTales is a service whose aim is to stimulate conversations between people in a shared space.

The service was developed for in-car usage.

The main characteristic of TravelTales is to know people preferences and propose news that are the nearest to the interests of the passengers.

### How does it works


#### News crawling and indexing 

The service can fetch news from any website, then for each of them it generates a summary which will be indexed according to topics that are treated in that news.


For each news summary the system exploits the Coqui xTTS model v2 to produce a synthetized audio version of it.


#### News suggestion

Every time a TravelTales client instance tries to load the most interesting news for the group that is recognised as currently onboard, the retrieval system loads the interests of the passengers and computes the ranking of the most interesting news.

At that point news audio file is played by the client system.


#### Users interests adaptation

After news proposition, the system starts a feedback gathering phase in which people engagement level is estimated by exploiting audio and video features coming from each user.

