---
layout: post
title: EPSS Data Google Spreadsheet
categories: [EPSS,CVE,GSheet]
excerpt: The Exploit Prediction Scoring System (EPSS) is a data-driven effort for estimating the likelihood (probability) that a software vulnerability will be exploited in the wild.This is Google Spreadsheet directly sourced from the EPSS Database, updated automatically every 24 hours. It's a data source with minimal elaboration to allow direct analysis.
author: alucab
image: /images/epss.png
---

![][EPSS_IMG]

## Understanding Exploit Prediction Scoring System (EPSS) 

The Exploit Prediction Scoring System (EPSS) is a data-driven effort for estimating the likelihood (probability) that a software vulnerability will be exploited in the wild. Our goal is to assist network defenders to better prioritize vulnerability remediation efforts. While other industry standards have been useful for capturing innate characteristics of a vulnerability and provide measures of severity, they are limited in their ability to assess threat. EPSS fills that gap because it uses current threat information from CVE and real-world exploit data. The EPSS model produces a probability score between 0 and 1 (0 and 100%). The higher the score, the greater the probability that a vulnerability will be exploited.
If you don't know anything about it go to my [EPSS Database Introduction](/epss-introduction)

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

[EPSS_IMG]: /images/epss.png
[EPSS_GSHEET]: https://docs.google.com/spreadsheets/d/15Y8v39ViK5tm7XN56Vmi0gx9G1PVagLEf8MA6tRslck/edit?usp=sharing
