---
title: "JavaScript Interactives"
date: 2022-04-19T12:14:19-04:00
draft: false
---

## Air Quality Explorer

In 2019, I was learning about our air quality research team, and what they learn from the NYC Community Air Survey. 

I learned that they sample air quality each season from nearly 100 locations around the city, and combine those readings with data on things like building density and emissions, traffic, industrial activity, and more. This lets them create a complex model that can *predict* air quality in unmonitored areas, based on what they know about all the other underlying factors. Cool! 

My colleague Grant Pezeshki and I put our head together and started designing a simple interactive page that would let somebody input their neighborhood and get the modelled air quality values for key pollutants, as well as their values for the underlying factors.

### A few key design decisions
- We didn't just want to deliver data - we wanted to explain the connections. 
- We wanted it to be easy for somebody to find their neighborhood, even if they didn't know what neighborhood scheme we were using. Nobody knows their NTA code.
- Everybody loves maps, but sometimes, bar charts are more useful: they can show both value distribution and rank, and easily let you compare a single value to the whole. So, we wanted to keep a map, but show the air quality in bar charts. 

### The technology we used
Grant wrote most of the initial JavaScript, and from this project, I learned enough to create future interactives. Here's how it works:
- A scrap of D3 code ingests a data file that contains a list of neighborhoods and each one's value for the two pollutants, and the tertile for the four factors.
- We use GOV.UK's Accessible Autocomplete to let the user identify their neighborhood - this is saved as a variable.
- We use that variable to sort the data file, deliver the tertile value to the maps, add a neighborhood highlight to the map and to the bar charts.
- The map and charts use Vega and Vega-Lite.

{{< addimage src="/air-quality-explorer.png" caption="Screenshot: Air Quality Explorer.">}}

---

## Interactive Heat Vulnerability Index
My colleagues who are climate researchers developed a Heat Vulnerability Index that scores NYC neighborhoods based on 5 factors that lead to the highest risk of heat-related mortality. 

Similar to the Air Quality Explorer, we could create an interactive that let a user find data for their neighborhood and see how it compares to the overall. 

I used Grant's JavaScript from the Air Quality Explorer and edited it to do essentially the same thing with Heat Vulnerability Index data to create an interactive Heat Vulnerability Index. 

{{< imagemodalbtn src="/heat-vuln-index.png" link="Heat Vulnerability Index" caption="The interactive Heat Vulnerability Index" id="modalHVI">}}

---

## COVID-19 Data by ZIP Code
After building the Heat Vulnerability Index, I looked for opportunities to continue writing one-page JavaScript data communication apps in my COVID-19 response work.

It was important to our team that we make the data easy to understand, but we felt that a lot of the data on the pages was oriented toward a policymaking audience - helping them answer the question "What areas need our attention?" But, most New Yorkers weren't trying to identify which neighorhoods had highest case rates. Most New Yorkers probably wanted to know what was happening in their neighborhood. 

So, we built a page that would access top-level ZIP Code data about COVID, and deliver it. It used the same tech as the other JavaScript interactives that we built. And, we focused on the following design and data comms approaches:
- Relevance: leveraging a location-first primary pathway to ensure that we're delivering immediately relevant information
- Providing numbers in different formats: like, reframing rates as "one out of every 7 people" to communicate to people without our data literacy
- Using comparisons to explain: comparing a neighborhood's value to that of its borough and the city as a whole
- In-line explanations of metrics and terms, for just-in-time context

Since launching this page, it's seen huge amounts of web traffic. The highest-traffic page is Latest Data, and for much of the vaccination era, the Vaccines page had highest traffic, but more recently, Data by ZIP has eclipsed Vaccines.

{{< imagemodalbtn src="/data-by-zip.png" link="Data by ZIP" caption="The ZIP Code Explorer" id="modalzip">}}

