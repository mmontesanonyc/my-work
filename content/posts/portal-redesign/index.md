---
title: "Data Portal Redesign Part 1: Problems and Priorities"
date: 2022-06-18T12:14:19-04:00
draft: false
---

In 2021, our team began a re-design of the Environment and Health Data Portal. This site is one of the Health Department's marquee data communication platforms and a major way that our bureau and division communicate. 

{{< addimage src="/old-data-portal-home.png" caption="The old EH Data Portal.">}}


The site was designed to store and automatically visualize datasets ("indicators") that show how environments and heath are related. Over time, the site grew to include additional content types, like:
- {{< imagemodal src="/old-data-portal-data-story.png" link="Data stories" caption="This is a data story" id="modal1">}}
- {{< imagemodal src="/old-data-portal-old-NR-output.png" link="Neighborhood reports" caption="The old EH Data Portal Neighborhood Reports" id="modal2">}}
- The portal's original functionality, automatically visualizing a dataset, became called the Data Explorer. {{< imagemodal src="/old-data-portal-indicator-map.png" link="Here's an example." caption="Visualization of an indicator" id="modalindicator">}}


## Things we wanted to address
### Front-end issues
- Inconsistency: the site was designed as one product but grew to host other products, which led to a mish-mash of different designs on the site. For example, the one-off data interactive pages looked very different from the Data Explorer, Data Stories, and Neighborhood Reports. {{< imagemodal src="/old-data-portal-realtime.png" link="Here's an interactive data page" caption="Realtime air quality page" id="realtime">}}
- Usability issues: the site had a host of usability issues. Data searches and site searches weren't great. Browsability was problematic due to the information architecture (a very hierarchical tree) and the technology, which meant that we were manually managing links between some content types.
- Speed and performance issues: a lot of the site was built to load front-end content from our database, meaning that it was slow to load simple text content.
- Categorization issues: datasets were organized very hierarchically. This made it difficult to build in connections between related environmental and health issues, which are multifaceted and interrelated. {{< imagemodal src="/old-data-portal-aq-hub.png" link="On the portal, our stopgap approach was to create one-off Hub Pages to connect data cross areas." caption="Air Quality hub page" id="aqhub">}}
- Data visualization: for a data communication site, the visualization had room to improve. 

### Organizational issues
- Technical debt: due to staff turnover, the current staff didn't have a thorough understanding of how to maintain and develop the site under its existing framework.
- Data management: our fairly complex back-end database was designed to support the site; staff turnover made data loading and management a challenge given the current structure of the database.

## Re-design priorities
Because of those issues, a site redesign had to encompass technoloogy, content strategy, information architecture, usability work, and informatics strategy. 

The following were our priorities:
- Manageable technology: we wanted to pursue a smart technology strategy that would let us do in-house maintenance and development, as well as easily contract for pieces we didn't have the time or capacity to build. This would let develop with an  agile style and continuous improvement. 
- Consistency: we needed the site to be a clear, singular product, rather than a collection of components. It needed a consistent design, navigation, and search functions. 
- Contemporary, reliable design: the site needed to appear trustworthy. It needed to look good, use familiar design components, and work well on mobile devices. 
- Integration: the site needed to support ways to connect content types across content areas. We wanted to support users' ability to browse and discover related content, so we needed the site structure to be able to support communicating the connections and relationships between topics. 
- Usability: The site needed to be easy to use. No - it needed to be *nice* to use.

So, we set off to design the best government data communication website. 



