---
title: Network Visualisation with visNetwork
date: '2023-01-12'
slug: []
categories: []
tags: [R, visNetwork, igraph]
type: ''
subtitle: ''
image: ''
---

<script src="{{< blogdown/postref >}}index_files/htmlwidgets/htmlwidgets.js"></script>
<script src="{{< blogdown/postref >}}index_files/pymjs/pym.v1.js"></script>
<script src="{{< blogdown/postref >}}index_files/widgetframe-binding/widgetframe.js"></script>

![](featured.png)

## Project context & Data

This visualisation was built as part of a project on network analysis in 2018 in collaboration with [SwissContact](https://www.swisscontact.org/en/about-us) and University of Sydney. The network data is sourced and owned by SwissContact. The data represents men and women cocoa farmers from Indonesia and the existing social network between them, how long they knew each other and how they come to meet each other along with Swiss Contact experts. The network visualisation was therefore build to capture this relationship between them and explore the network properties.

## Visual

I used `visNetwork` and `igraph` to work with the network data in R. `visNetwork` is a R package for network visualisation based on [vis.js](https://visjs.org/) javascript library. `igraph` is a collection of network analysis tools available across R, Python, C/C++ and Mathematica. Some nework properties such as degree, centrality were computed using `igraph` which were than translated into visual features.

The visual below also has an in-built spring algorithm which enables the icons to recoil and vibrate back and forth like a spring - try pulling one of the icons! You can also selectively highlight parts of the network by clicking on the icon (or node) of interest and all connected edges and nodes will get highlighted. You can also zoom in, zoom out and drag it around to change focus.

<div id="htmlwidget-1" style="width:100%;height:600px;" class="widgetframe html-widget"></div>
<script type="application/json" data-for="htmlwidget-1">{"x":{"url":"index_files/figure-html//widgets/widget_interactiveVis.html","options":{"xdomain":"*","allowfullscreen":false,"lazyload":false}},"evals":[],"jsHooks":[]}</script>
