---
title: "Data Portal Redesign Part 2: The Work"
date: 2022-06-19T12:14:19-04:00
draft: true
---

## The groundwork
The site re-design started as a pilot in 2020, when we began re-building the Neighborhood Reports. First, we conducted a 6-month user research and user-centered design process, during which we conducted a survey, key informant interviews, and co-design sessions.

Then, we engaged a contractor to re-build the Neighborhood Reports. We wound up launching these on our extant site. This build would form the backbone of our full portal re-build. 

{{< addimage src="/old-data-portal-new-NRs.png" caption="The old portal's new Neighborhood Reports.">}}

## Choosing  technology
In general, we wanted stable, reliable, conventional technology that would be easy for both staff to develop and maintain, or for new contractors to interface with. This would support a modular approach to site maintenance and develop. 

- Static site: building the new prototype as a static site  would let us build a secure, fast, flexible site that would let us pursue both internal develop and modular contracting, since it relies on fairly common, conventional technologies. We chose [Hugo](https://gohugo.io/).
- [NYC Core Framework](https://www1.nyc.gov/assets/doitt/html/nyc-core-framework/index.html): we built our site's templates using this framework, which was developed for City agencies using [Bootstrap](https://getbootstrap.com/). It had good accessibility and translation functionality built in.

A simple site built using core HTML, CSS, and JavaScript would allow easy integration of some other technologies, like:
- [Vega Lite](https://vega.github.io/vega-lite/) for automated visualizations, and [Arquero](https://uwdata.github.io/arquero/) for client-side data manipulation. Data were stored as JSON in a Github repository, ingested and manipulated using Arquero and vanilla JavaScript, and delivered to a Vega-Lite specification.
- [Lunr.js](https://lunrjs.com/) for sitewide search, and subsearches powered by [GOV.UK's Accessible Autocomplete](https://github.com/alphagov/accessible-autocomplete)
- Development deployment to a Github repository using Github Actions to index the site for search, build, and deploy the site. 

## Beginning in earnest
After taking receipt of the re-designed Neighborhood Reports, we began building the rest of the portal in earnest. 
- We learned Hugo, wrote templates and functions
- Our ported over content, building out our new site prototype, and refactoring old code for efficiency.
- We developed a new categorization scheme that would let us communicate how topics are interrelated
- We conducted a major content audit, reviewing all topic areas, and web copy in cooperation with our internal partners
- We conducted a major data audit, reviewing our datasets and their display needs so that we could write requirements and contract for the full development of our Data Explorer module 
- We re-developed our database to deliver data structured and optimized for display in this system

{{< addimage src="/new-portal-home.png" caption="The new portal's home page.">}}


## The new prototype
Here's what it features:
- A consistent style with the same navbar on every page to help show users where they are.
- A "related content" functionality that connects content based on core areas that we choose
- A "tags" functionality that connects content based on a looser set of keywords
- A new "Key Topic" area that connects resources across the other content types: Data Explorer, Neighborhood Reports, Data Stories, and Data Features.
- A strong sitewide search
- Major rennovations to the Data Explorer function:
    - Collapsing our 'topic' and 'indicator/visualization' pages to get users to visualizations in fewer clicks
    - Ability to toggle between indicators, so that users could explore faster and more easily
    - Improved UX on display options, letting them switch measures or years more easily
    - Improved visualizations and tooltips.

## Timeline and launch
The full prototype development took about a year:
- Summer 2021: begin Hugo development
- Fall 2021: content migration
- Winter 2022: begin contracting for remaining components
- Spring 2022: content and data audit
- July 2022: complete full site prototype
- August 2022: launch site
- September 2022 onward: ongoing iteration, development, and maintenance. The site is never *done*. We chose to re-design the site not as a milestone to reach, but a path to put us on: one that would allow us to do ongoing user research and user-centered design, frequent optimzation and experimentation, all with a platform that could give us full control over our product. 