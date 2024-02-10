---
layout: project
name: dronesimulator
short_description: A web app that lets people learn drones normatives and best practices. 
image: /assets/images/dronesimulator/dronesimulator-logo.png
technologies: PHP, JavaScript, Python, Flask, SciKitLearn, SQL
authors: "Giacomo Pacini"
date: 2020-04-16
active_project: True
priority: 5
---


Drones are getting more and more popular and for this reason EASA (the European Union Aviation Safety Agency) and ENAC (Ente Nazionale Aviazione Civile) introduced some regulations and a mandatory knowledge test in order to fly certain drones.

<!-- In addition, every time a pilot wants to fly with its drone he has to check weather and fly regulations for that place. -->

### What is dronesimulator

dronesimulator is a web app that lets people simulate the test that they have to face to obtain the open category pilot certificate.

#### Functionalities

Beside the test simulation, the service implements various functionalities such as:
- **suggestion of new questions**: users of the platform can suggest new questions to be insterted in the simulation collection.
- **questions reporting**: users can report error, refuses or missing details in the questions that they find during the simulation.
- **moderation**: moderators can approve or reject suggested questions, modify and update the questions in the collection and review the eventual reports from users about questions with errors.
- **similar questions retrieval**: users can search for an arbitrary question and the service will retrieve the nearest questions in the service collection.
- **questions category prediction**: given a question the system classifies it among the categories used in the collection.
- **persistence of previous simulations**: users can save and review their past simulations, the answers they gave and the score they achieved.
- **dronesimulator meteo**: a service that is open also to unregistered users, it lets people search for any place or address in the world and returns the weather forecasts in terms of wind, solar storms, precipitations relative to that place. It returns also information about the number of visible satellites for GPS coverage and about eventual flight bans or limitations.

### Can I try it?

The website is available online and it has more than **21.000 registered users** from Italy.

You can try it by yourself at [dronesimulator.it](https://dronesimulator.it).