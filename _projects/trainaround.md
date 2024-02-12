---
layout: project
name: TrainAround
short_description: Monitoring Athletes Workout Using a BLE Star Topology Network with Android. 
image: /assets/images/trainaround/wearOS-square.png
technologies: Java, Android, WearOS, Bluetooth Low Energy
authors: "Giacomo Pacini, Enrico Nello, Matteo Pierucci, Tommaso Giorgi"
date: 2022-05-29
prior: 14
github: https://github.com/Ruggero1912/TrainAround
---

TrainAround introduces a service that lets a trainer control the training status of a group of athletes in real-time.

### Current solutions

The most common approach nowadays for workout tracking
consists in Wearable apps that run directly on the wearable device
and let you access the device's services all on the device itself.

Fitness apps are designed specifically to assist with exercise, other
types of physical training, or related fitness topics. The purpose of
those fitness app is to provide the user with instructions and
examples of one or more types of exercise, physical activity, record
statistics on workouts or collect data on walks, or some other fitness
topic.

Anyway, all these applications suffer from the impossibility
for a trainer to monitor in real time the workout
sessions of many athletes, instead of just one.

Most of the time, in real life sport-scenarios, it would be interesting
to change the perspective from 1:1 (Athlete self-checking his/her
own statistics) to One-to-Many (Trainer supervising his/her
Athletes’ statistics). 

Also, for those apps that lets users to connect
to a personal trainer to share statistics about fitness routine, the
delivery of the latter is **asynchronous**. 
Thus, they miss an on-thefly monitoring feature that could let the trainer to track more
effectively the session.

In addition to that, existing workout tracking apps running on
smartphones cannot accurately sense user activities when the phone
is placed away from the user, or just become unhandy if they
require the phone to be attached to the body.

### Characteristics of TrainAround

We instead developed an application that collects data from
multiple Wear OS smartwatches and shows the collected
information from all the smartwatches on one central Android
device, which is supposed to be the coach / trainer device.

The aim is to find a **lightweight solution** that **does not need the
presence of the smartwatches' paired phones**, so that the monitored
users do not have to bring their phones with them. 

The other requirement is to **avoid the use of internet**, so that the
application could work even in remote areas or where there is no
Wi-Fi hotspot for the smartwatches.

So, from a technical point of view our work consists in creating a
local area network between one android device (acting as a server /
central node) and multiple Android Wear OS devices acting as
clients / sensors.

TrainAround was thought to be addressed for the track and field
world, where the presence of small groups of athletes and their
coaches would actually take advantages from using it.
