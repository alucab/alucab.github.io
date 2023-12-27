---
layout: post
title: CISA KEV Google Spreadsheet
categories: [KEV,CVE,GSheet]
excerpt: A Google Spreadsheet directly sourced from the CISA KEV Catalog, updated automatically every 24 hours. It's a data source with minimal elaboration to allow direct analysis. 
author: alucab
image: /images/cisa.webp
---

![][CISA_IMG]

## Understanding CISA KEV Catalog

The CISA Known Exploited Vulnerabilities (KEV) Catalog stands as a critical resource curated by the Cybersecurity and Infrastructure Security Agency (CISA) to aid in identifying vulnerabilities actively exploited by cybercriminals. 
If you don't know anything about it go to my [CISA KEV Introduction](/cisa-kev-introduction)

## CISA KEV Google Spreadsheet

I've developed a [CISA KEV Spreadsheet][CISA_GSHEET] directly sourced from the CISA KEV Catalog, updated automatically every 24 hours. It's a basic data source without any elaborations to allow direct analysis.

Here a sample

<div style="text-align: center"> 
<iframe frameborder="0" width="100%" height="500px" scrolling="no" allowfullscreen src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQ2rjzP8U9wgDcgP-HEsag9E1Gz3QG2ED8OGioPMnVuCjvwm8pGhsdapgsfadO0JO3xYdcUa6kEa61t/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
</div>

This easily accessible resource provides several benefits:

- **Real-Time Information:** Having data refreshed regularly ensures access to the latest information on actively exploited vulnerabilities, aiding in swift decision-making for vulnerability remediation.

- **Convenience and Ease of Use:** With the spreadsheet readily available and updated automatically, organizations and individuals can conveniently access and utilize the data without the need for manual updates or checks. It's easy to grap it and create visualization or analyses without manual CSV imports or JSON parsing

- **Easiness of Integration:** Google Spreadsheet is a format extremely powerful and diffused. It is also easily integrated in Google Looker Studio without need for CSV imports to be refreshed, scripts, or external connectors

- **Enhanced Security Posture:** Immediate access to refreshed vulnerability information empowers swift action, allowing for quicker vulnerability resolution, thereby strengthening the overall cybersecurity posture.


Utilizing and maintaining access to a continuously updated spreadsheet derived from the CISA KEV Catalog ensures that organizations and individuals have a reliable, easily accessible resource to bolster their cybersecurity defenses against known and actively exploited vulnerabilities.

## Resource Links

- [Official CISA Known Exploited Vulnerabilities Catalog](https://www.cisa.gov/resources-tools/resources/kev-catalog)
- [CISA KEV Spreadsheet (Updated Daily)][CISA_GSHEET]



[CISA_IMG]: https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhmRFG6Xp2cUYbmQgYLPwJuEEH2i8lUIEEtMoycnyzKS4e_KBv14tfmALTtvYtvJnFKo9OUzj7LFyd1u8FTd3Nd2lgFa4dp2s3eO2lpolSYcLaiX0aUXs6DKPYgW5akbJlbKA6aC043prrHMAlJ0zZMxRu-r-eCdfJQTrJ90bjDOBQuCpMrAhn_n5-s/s728-rw-ft-e30/cisa.png
[CISA_GSHEET]: https://docs.google.com/spreadsheets/d/1Wk--S5xrii8-7QJsapKlqMfWYk7xPOzfnLDQc1msR4o/edit?usp=sharing
[Securin]: https://www.securin.io/articles/cisa-launches-known-exploited-vulnerabilities-catalog