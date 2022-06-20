---
title: "Re-designing Neighborhood Reports"
date: 2022-04-01T10:14:19-04:00
draft: false
---

The EH Data Portal's Neighborhood Reports were designed to show data for a neighborhood on a a specific environmental health topic. There are neighborhood reports for Asthma, Outdoor air, Housing, Climate, and Active design. They looked like this, below: a list of indicators, neighborhood-boro-city comparisons, a trend, and a big colorful indicator about whether or not the chosen neighborhood is better, in the middle, or worse than most other neighborhoods. 

{{< addimage src="/old-data-portal-old-NR-output.png" caption="The old EH Data Portal Neighborhood Reports.">}}

But, there were a few problems:
- They were PDFs
- Our site had more information about each of these indicators, but you couldn't click to explore them
- It wasn't easy to go back and get a different report, or a report for a different neighborhood.

Basically, classic PDF problems: the content doesn't really share the same environment as the rest of the site. 

## Formative research
With the plan to re-design the neighborhood reports, we conducted formative research. First, we did a usability assessment, and identified some priority areas to fix: the new reports should be mobile compatible, be easy to use, and enable further exploration into indicators or other reports. 

Second, we did user research, inspired and guided by [Civic Service Design](www.civicservicedesign). For this user research, we:
- Assembled a user group by reaching out to contacts we knew used the portal regularly
- Distributing an open-ended survey asking for thoughts and ideas
- Recruited 6 people for in-depth interviews in which we asked how they use data. Crucially, we weren't really asking them for their opinions on the site - rather, we were asking about their data-seeking habits so that we could brainstorm ways that the site could meet their needs and help solve their problems.
- Recruited 6 people for a co-design session in which we collaboratively sketched out a re-designed set of Neighborhood Reports.

This collaborative design session didn't get us there, however. But by synthesizing everything we heard, we identified a set of key problems and concerns:
- Yes, people want things to be easy to use - even expert data users
- People - even health professionals - want us to provide context and explanation. The Why of an issue.
- Users wanted to understand why a neighborhood performed the way it did, and wanted to be able to explore similar neighborhoods.
- They didn't want to stop there - they wanted to think about what could be done about an issue, given the often problem-identifying lense of disparity data. 

## Design
Our team met weekly to help synthesize our findings, crystalize them into key questions, and rapidly iterate on designs that would address them. 

Our intial-final design featured:
- Mobile functionality, which we sketched out using Bootstrap
- Multi-step interactivity, allowing a user to get an overview first and details on demans
- Connections to other reports, other neighborhoods, and additional indicator details

There were some cool details, but some of them had to be changed or abandoned due to implementation constraints.

## Implementation
We worked with a contractor to implement, and the design went through some further iteration. Once they were launched, they meet a lot of the original project goals: they're mobile compatible, they let us provide more information with the information we have, they allow a greater level of integration and exploration. And, we think they meet our user's needs, too. 

{{< addimage src="/new-NR-1.png" caption="The new EH Data Portal Neighborhood Reports.">}}

After seeing the summary output, a user can click into specific indicators to get more detailed information: neighborhood-boro-city comparisons, and other data displays: a bar chart, a trend chart, and a map. The modal quickly and easy pops up or goes away, making exploration really light and simple.

{{< addimage src="/new-NR-2.png" caption="Indicator details at the new EH Data Portal Neighborhood Reports.">}}
