---
layout: page
title: iOS portfolio
---

# iOS portfolio

*Note that most recent projects I have worked on are protected by NDA and I can not list them here.*

## [Total Mama](https://innovation.ox.ac.uk/incubator-ventures/total-mama/)

This project was a startup that spin-off from Oxford university, trying to
improve the health of pregnant mothers and their babies by monitoring their progress
and offering advice based on input from experts at Oxford.

Sadly, it was never finished due to lack of funding.

![Total Mama Charts](/assets/totalmamacharts.png)

### Uses:

* [Charts](https://github.com/danielgindi/Charts)
* *ResearchKit* to obtain data from the mothers and use in Oxford's research.
* Executed mathematical functions obtained from Oxford's research to plot the data in charts.
* *Model-View-Presenter* architecture
  * Plain old object acts as *Presenter*.
  * *UIViewController* arranges *View* and *Presenter* together.
  * *UIView* subclass acts as *View*.

## [Nuffield HealthScore](https://www.nuffieldhealth.com/healthscore)

A health tracking application that we inherited from another company. In the 2.1 release
we re-skinned the whole application with a new set of designs produced by yet another 3rd Party.

In 2.2 we integrated with *HealthKit* and *Microsoft Band* to obtain more data from the user
to better reflect their health in the app.

After being maintained by another agency, the product was discontinued.

![Nuffield HealthScore](/assets/nuffieldhealthscore.jpeg)

### Uses:

* Push notifications
* Offline functionality
* *HealthKit*
* *Microsoft Band*
* Bespoke circular chart written as a *UIView* subclass, including animations
* Device sensors to track activities like running.

## [Barcelona City App](https://itunes.apple.com/gb/app/barcelona-city-app/id660676262?mt=8)

![Barcelona City App](/assets/bcncity.png)

### Uses:

* Geofences
* *NodeJS* (*Express* + *MongoDB*) backend
* Push notifications

## [Food2U](http://appcircus.com/apps/food2u)

![Food2U](/assets/food2u.png)

The company was bought by Just-Eat and no longer exists.

### Uses:

* *Titanium Appcelerator* to build a cross-platform app (JS code).
* *LAMP* stack.
* *Twilio* to dispatch orders to restaurants.

## [MobileID](http://www.mobileid.cat/en/)

![MobileID](/assets/mobileid.png)

### Uses:

* Certificate generation
* Certificate signing
* [Nonces](https://en.wikipedia.org/wiki/Cryptographic_nonce), Salt & Pepper, and other measures to ensure security is up to the standards.
* Push notifications

## [By-Taxi](https://itunes.apple.com/gb/app/by-taxi/id524360817?mt=8)

![By-Taxi](/assets/bytaxi-ios.jpeg)

### Uses:

* *MapKit*
* *Geofences*
* *WebSockets*
* Push notifications
