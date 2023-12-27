---
layout: post
title: Exploring Cybersecurity Insights with Google Looker Studio's KEV & EPSS Playground
categories: [KEV,EPSS,Looker,CVE]
author: alucab
excerpt: Explore an interactive Google Looker Studio dashboard merging cybersecurity insights from CISA KEV (Cybersecurity and Infrastructure Security Agency's Known Exploited Vulnerabilities) and EPSS (Exploit Prediction Scoring System) scores.
image: /images/2023-12-27-KEV-EPSS-looker-playground.PNG
---

## Overview

This interactive dashboard consolidates essential cybersecurity insights from two key sources:
- CISA KEV Catalog
- EPSS Scores Database

### How to Use It

Using the dashboard is straightforward. Simply interact with the various filters and views to analyze vulnerabilities. Understand the correlation between KEV and EPSS scores, gaining insights into your vulnerability landscape.

## The Value in Insights

This dashboard offers a powerful lens into your cybersecurity posture. By amalgamating data from CISA KEV and EPSS scores, it provides actionable insights, enabling informed decision-making regarding vulnerability management and risk mitigation strategies.

### Use Cases:

#### Prioritizing Remediation Efforts

Integrating CISA KEV's known exploited vulnerabilities and EPSS's predictive scores, the dashboard assists security teams in prioritizing which vulnerabilities to address first. High EPSS scores coupled with CISA KEV data signify critical vulnerabilities that have a high probability of being exploited or are actively being exploited. This prioritization helps in allocating resources efficiently, focusing on the most pressing security concerns.

Consider for example this view of the main Microsoft related CVEs that are actively related to a campaign and with an EPSS score over 50%

![][MAIN_IMG]

#### Trend Analysis and Forecasting

The dashboard could enable trend analysis by tracking changes in EPSS scores over time for specific vulnerabilities. Understanding how these scores evolve provides insights into the shifting threat landscape. It allows security professionals to anticipate potential future threats and take preemptive measures to safeguard systems before vulnerabilities are actively exploited.

#### Comparative Analysis and Benchmarking

Comparing vulnerabilities based on their CISA KEV status and EPSS scores allows for benchmarking against industry standards. Identifying discrepancies between severity and exploit likelihood reveals areas where traditional severity ratings might not align with real-world exploit probabilities. This analysis helps refine risk assessment methodologies and improve decision-making for vulnerability remediation strategies.



## Powered by Google Looker Studio

This dashboard utilizes internal data sources from Google spreadsheets, ensuring up-to-date information without manual CSV file imports. The continuous updates to EPSS scores add ongoing value. Data sources are refreshed every 24 hours to maintain relevance.



<div style="text-align: center"> 
<iframe src="https://lookerstudio.google.com/embed/reporting/cb1300d3-b1fd-4e6d-8e38-cae516aff15d/page/sPPB"  width="100%" height="500px" frameborder="0" style="border:0" allowfullscreen></iframe>
</div>

## Feedback
For questions or ideas send me a message in [Github](https://github.com/alucab/vulnerabilitysheets) or find me on [LinkedIn](https://www.linkedin.com/in/alucab)

[MAIN_IMG]: /images/2023-12-27-KEV-EPSS-looker-playground.PNG