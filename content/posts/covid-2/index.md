---
title: "COVID-19 data strategy"
date: 2022-06-10T12:14:19-04:00
draft: false
---

I spent 27 months activated with the Health Department's COVID-19 response, working on our data webpages. In this time, I:
- Led COVID-19 data visualization and data communication strategy
- Managed and developed front-end web code
- Trained and mentored analysts to do similar work
- Authored and co-authored papers, spoke at conferences and workshops

This project had wide-reaching effects. 
- We built the Health Department's most high-profile digital product ever. 
- We brought our knowledge to the world, allowing it to influence research, policy, and pandemic response
- We raised the profile of the importance of smart, strategic data communication in the department
- We advised people in other jurisdictions' health agencies on how to do similar work

Here's what we tried to do with our data communication project:

**Build trust**: In March 2020, people were scared. I know I was. People were looking for data, but they weren't finding answers to the questions they were asking. For the Health Department - and the city as a whole - to mount an effective response, we needed to be open and trustworthy. That meant answering people's questions when they ask them, and it meant showing that we knew what was going on. 

A clear, transparent data communication strategy was vital to building trust. We were guided by the principles of crisis communication: be first, be right, be credible.

**Support a population-wide response**: Data aren't just for data professionals. Data are knowledge, and we wanted to share that widely. This is, after all, a pandemic, and responsing to a pandemic requires that everybody pitch in. That means that we needed everybody on the same page - whether it was getting people to mask up when they left their house, or offering data to people who were doing new analyses, data helped get everybody to flatten the curve. 

Here's how we tried to do this.

## Be transparent
Early on, we'd know that the data would change. Early in the pandemic, people noticed that data for prior days would adjust upward: we were pubilshing data by date of diagnosis, meaning that if yesterday, we learned about a new case a week ago, then the count for the date a week ago would go up. This was new to much of our audience, and we fielded a lot of questions about why "old data" were changing.

Additionally, analytics and informatics methods were being developed on the fly. These surely would change, and that would change data values, too. We knew that this could freak people out or look like manipulation or suppression, so we wanted to be fully transparent about it.

Publishing data in a Github repository meant:
- People could see the historical record, via previous versions stored by git
- We could include a lot of documentation, data definitions, and more
- People could ask questions by filing issues - and we'd answer them

{{< addimage src="/covid-github.png" caption="The COVID data Github repo.">}}

## Publish data as data
Government agencies are often notoriously bad at publishing data, often formatting it as web content, or burying it in PDFs. We wanted to make it easy for researchers, journalists, and others to use the data - so we committed to publishing them in machine-readable CSV format. 

## Make the data friendly and approachable
To make the data accessible for many kinds of people, regardless of data literacy. To do this, we:
- Built data pages as standard webpages, rather than as technical-feeling "dashboards"
- Created communication-oriented visualizations, frequently departing from design and visualizations standards common to research, academic or biomedical data analysis. We built clear, focused, message-oriented visuals.
- Explained metrics, interspersing visuals with explanations of the metrics they were showing, what they mean and why they are important.

## Use lightweight, easy technology
When we started, we wanted to build something that we could launch in *days*. That means choosing very lightweight technology. We started with a free Datawrapper account and a free Github account.

[Datawrapper interviewed me about our team's experience using their platform.](https://blog.datawrapper.de/nyc-health-covid-reporting/)

## Set up a maintainable workflow
We'd be updating the data every day, and we didn't know how long it would last - maybe months! We needed a workflow that was simple, and easy for new staff coming in to emergency response work to pick up. Feeding the charts from a Github repository meant that an analyst would only have to run the code that updated our local CSVs and then upload them to Github - that would update all of our data pages. 

## Listen to users
To ensure that we were meeting our targets, we listened to our users. We monitored the Issues in the Github repository, kept tabs on data conversations on Twitter, conducted informal usability research and sitewide surveys. We'd synthesize what we learned and fold in our findings into new development plans. 

## Adapt
The pandemic changes, so our data reporting had to, too. We aimed to stay flexible and adaptible, with a "continuous improvement" approach whereby we might prototype and launch something but aim to refine and improve it as it was live, rather than being late trying to get it perfect the first time. 

And, we planned to modify the data and what we were displaying as needs dictated, rather than assuming that the needs wouldn't change as the pandemic did. 