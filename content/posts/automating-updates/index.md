---
title: "Automating Updates"
date: 2022-06-20T10:14:19-04:00
draft: false
---

## Heat syndrome
My climate colleagues approached me to talk about a page that would provide near realtime data on temperature and heat-related illnesses. 

I built a simple page that showed charts with the data. My colleagues automated an R script to output the files and a bash script to push the files to the Github repository. The charts were built to read the data in the Github repo. So, without intervention, this page updates every day. 

{{< imagemodal src="/syndromic.png" link="Heat Syndrome Data" caption="Near realtime heat syndrome data" id="modalsyndromic">}}

---

## Realtime Air Quality
My colleagues who work on air quality have a network of realtime air quality monitors, so we collaborated to get those data to the web, too. We used a similar approach: local code building updated files and pushing them to a Github repo.

The page is a little bit more involved, with buttons letting users highlight data from specific monitors and zoom in on recent days of data. Much of this, especially the integration with a Leaflet map, was done by my colleague Chris Gettings. 

{{< imagemodal src="/realtime.png" link="Realtime AQ data" caption="Near realtime air quality data" id="AQmodal">}}