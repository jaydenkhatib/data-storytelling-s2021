---
title:  Sample Story
date:   2021-03-01 00:09:00 -0500
categories: [ "maps" ]
authors: Rahul Bhargava
---

This is a sample story.

## Here are Some Markdown Samples

This has some content in _italics_ and *bold*.  You can include [links](https://google.com).

> “A blockquote is something you do too"

There are some samples below:
* embedding a Tableau Public viz
* embedding a Vega-Lite Chart
* embedding a Leaflet map

### You can Embed a Tableau Public Viz

<div class='tableauPlaceholder' id='viz1615571471442' style='position: relative'>
<noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;th&#47;theme-overlap-playground&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript>
<object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='theme-overlap-playground&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;th&#47;theme-overlap-playground&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en' /><param name='filter' value='publish=yes' /></object>
</div>
<script>
  var divElement = document.getElementById('viz1615571471442');
  var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

### Here's a Vega-Lite Chart

<div id="my-chart"></div>
<script>
// This is the specification for the chart, including the data
var myVegaLiteSpec = {
  "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
  "description": "A simple bar chart with embedded data.",
  "data": {
    "values": [
      {"a": "A", "b": 28}, {"a": "B", "b": 55}, {"a": "C", "b": 43},
      {"a": "D", "b": 91}, {"a": "E", "b": 81}, {"a": "F", "b": 53},
      {"a": "G", "b": 19}, {"a": "H", "b": 87}, {"a": "I", "b": 52}
    ]
  },
  "mark": "bar",
  "encoding": {
    "x": {"field": "a", "type": "nominal", "axis": {"labelAngle": 0}},
    "y": {"field": "b", "type": "quantitative"}
  }
};
// when the page loads, render the chart into the "my-chart" div element
$(function(){ vegaEmbed( '#my-chart', myVegaLiteSpec) });
</script>

### Here's a Leaflet Map

<style>
#my-map { height: 180px; }
</style>
<div id="my-map"></div>
<script>
$(function(){
  // when the page loads, set up the map with all the code
  let map = L.map('my-map').setView([42.3370, -71.0892], 15);
  let osmTileLayer = L.tileLayer( 'http://a.tile.stamen.com/toner/{z}/{x}/{y}.png', {
      attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>'
  }).addTo( map );  
});
</script>
