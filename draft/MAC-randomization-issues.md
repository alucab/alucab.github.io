---
layout: post
title: On the MAC address a device identification mean
categories: [Device Analysis,Start]
excerpt: Often the MAC address is considered a reliable identier of the device identity and a source of classification. MAC Randomization for privacy preservation definitely challenges this assumption and imposes a leap in device analytics
author: alucab
image: /images/epss.png
---

![][EPSS_IMG]

## What are MAC Addresses and why are they important for privacy ?

Every network interface has a MAC address, which is a traditionally considered a unique identifier and is used as a network address in communications. Your phone, tablet or computer's WiFi interface has a unique MAC address that it uses to identify itself to nearby network access points when it's looking for known WiFi networks to join, and to identify itself when joining a WiFi network. So do PLCs, OT and IoMT devices. In the era of mobility, location tracking is a major privacy concern for portable device users. Although a growing number of applications make use of location data, operating systems (OSs) provide the ability to turn off location services provided by the GPS or cellular/Wi-Fi connectivity. Wi-Fi access points, however, can monitor device locations without user consent by means of MAC addresses

Over the last few years many services have appeared, that use the WiFi signals emitted by smartphones to monitor the presence of people. The leading application of such services has been in the retail analytics sector, where they are widely used to monitor how many people pass in front of a store, how many enter it, how long they stay, how often they come back etc. But his technique is largely used by banks for security reasons and in many other environments.

Refraining from taking a position here (I am not a lawyer…), the point is that tracking WiFi is getting rather common. And it does raise legitimate privacy concerns.

You may wonder whether this is legal. The reality is that it’s in a kind of grey area. In legal terms people should wonder whether the MAC address of a WiFi interface is “personally identifiable information”, which is the kind of data that falls under personal data regulation and privacy directives. Most companies that do WiFi tracking for a living state it is not:

* FTC : “This persistent identifiers (MAC address) often can be linked to individuals by name. For example, when you sign into a commercial WiFi hotspot, your MAC address is tied to the information you use to sign up for the service. Additionally, automatic WiFi probes also broadcast the names of last networks a device has connected to, which potentially reveal additional information about the individual, such as the name of their home or work network”

* EC ( Article 29 Data Protection Working Party, Opinion 01/2017 ): “WiFi-tracking, depending on the circumstances and purposes of the data collection, such tracking under the GDPR is likely either to be subject to consent, or may only be performed if the personal data collected is anonymised.”

To address privacy issues Apple, starting from v.8 of its iOS operating system, added a WiFi MAC randomization feature. iPhones, when sending out hello messages, are using a randomized version of their real MAC address . Think of it as a fake identity. So you can still see the presence of a device, but such device may change its identity at any time (even multiple times during a same day), so that tracking becomes ineffective.

And Android? Well, also Android has added support for WiFi MAC randomization, starting from v.6 , but this feature is not used consistently by all phone manufacturers (see here for a detail description of what various vendors have done).

The question is then: provided that now many (we measured ~50%) of devices use WiFi MAC randomization, what is the statistical significance of the analytics provided by WiFi tracking?

## EPSS Database Google Spreadsheet

I've developed a [EPSS Database Spreadsheet][EPSS_GSHEET] directly sourced from the EPSS Database, updated automatically every 24 hours. It's a basic data source without any elaborations to allow direct analysis.

Here a sample

{% include embed.html url="https://docs.google.com/spreadsheets/d/15Y8v39ViK5tm7XN56Vmi0gx9G1PVagLEf8MA6tRslck/edit?usp=sharing" %}


This easily accessible resource provides several benefits:

- **Real-Time Information:** Having data refreshed regularly ensures access to the latest information on actively exploited vulnerabilities, aiding in swift decision-making for vulnerability remediation.

- **Convenience and Ease of Use:** With the spreadsheet readily available and updated automatically, organizations and individuals can conveniently access and utilize the data without the need for manual updates or checks. It's easy to grap it and create visualization or analyses without manual CSV imports or JSON parsing

- **Easiness of Integration:** Google Spreadsheet is a format extremely powerful and diffused. It is also easily integrated in Google Looker Studio without need for CSV imports to be refreshed, scripts, or external connectors

- **Enhanced Security Posture:** Immediate access to refreshed vulnerability information empowers swift action, allowing for quicker vulnerability resolution, thereby strengthening the overall cybersecurity posture.


Utilizing and maintaining access to a continuously updated spreadsheet derived from the EPSS Database ensures that organizations and individuals have a reliable, easily accessible resource to bolster their cybersecurity defenses against known and actively exploited vulnerabilities.

## Resource Links

- [Exploit Prediction Scoring System (EPSS) Home](https://www.first.org/epss/)
- [EPSS Daily Snapshot(CSV gzip)](https://epss.cyentia.com/epss_scores-current.csv.gz)
- [EPSS API](https://www.first.org/epss/api)
- [EPSS Database Spreadsheet (Updated Daily)][EPSS_GSHEET]


## Feedback
For questions or ideas send me a message in [Github](https://github.com/alucab/vulnerabilitysheets) or find me on [LinkedIn](https://www.linkedin.com/in/alucab)


