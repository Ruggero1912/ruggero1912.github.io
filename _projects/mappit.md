---
layout: project
name: MappIt
short_description: discover new places to visit and share adventures and experiences
image: /assets/images/mappit/application-architecture-mappit.png
technologies: Java, MongoDB, Neo4j, Spring, GeoJSON, OSM
authors: "Giacomo Pacini, Enrico Nello, Matteo Pierucci"
date: 2022-01-30
priority: 15
github: https://github.com/Ruggero1912/MappIt
---

MappIt is the *social network for explorers*, in which you can post your journeys to points of interests of many kinds, like castles, ruines, ancient buildings and historical places in general.

The user can post new visits, find new places to visit, interact with posts of other users and search among them according to various filters, like distance or popularity.

### Service implementation

The implementation of this project focused mainly on two aspects:
- **the backend of the service:** APIs of the service, the databases structure and the business logic
- **data population:** scripts that exploited external API and services to add places and posts in the databases of the service


The development of this service included many different aspects of software engineering and service design like for example:
- **Java application packages organization**
- **Java application databases connection handling**
- **Service endpoints**
- **Application use cases**
- **Functional requirements**
- **Non-Functional requirements**
- **databases queries analysis** by means of the *Operation Frequency Table*
- **Indexes** on certain collections and documents attributes to improve performances of certain frequent queries
- **Redundant fields** in documents to improve queries performances in terms of *executionStats*
- **Database sharding**: we proposed a database sharding based on the country code of places and users in order to grant higher service availability
- **Cross-database consistency management**
- **Definition of analysis queries**
- **Data population service**: [here an article about it]({{'/2022/02/10/how-to-create-a-database-of-thousands-of-users-in-a-couple-of-hours.html' | relative_url}}).



*Want to know more details? [Ask me](mailto:giacomo@paciosoft.com)*

### MappIt is Open Source

The code is freely available in this GitHub repo: <a href="{{ page.github }}" target="_blank">here</a>.

You will also find there a more technical readme file and the complete technical documentation of the project.