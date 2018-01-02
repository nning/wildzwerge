---
layout: page
title: Impressum
permalink: /impressum/
order: 2
---

## Adresse des Vereins & Kindergartens

Naturkindergarten Wildzwerge e.V.  
Weg zum Krähenberg 33A  
28201 Bremen

<span data-schema="mailto" data-address="mail@wildzwerge.de"></span>

Registergericht | Amtsgericht Bremen  
Registernummer  | VR8049

### Anreise

<div id="map" class="map">
  <div id="marker"></div>
</div>

[Link auf OpenStreetMap](http://www.openstreetmap.org/?mlat=53.06180&mlon=8.82937#map=19/53.06180/8.82937)

## Vertretungsberechtigter Vorstand

Karen Schumann (1. Vorsitzende)  
Marie Tödtemann (2. Vorsitzende)

## Gemeinnützigkeit

Gemäß Freistellungsbescheid ist der Verein als gemeinnützig aufgrund der
Förderung der Erziehung anerkannt und zur Ausstellung von
Zuwendungsbestätigungen für Spenden und Mitgliedsbeiträge berechtigt.

## Urheberrecht

"Greenbeans" font is made by [Tup
Wanders](http://www.fontspace.com/profile/Tuppus) and shared under the terms of
[CC BY 3.0](https://creativecommons.org/licenses/by/3.0/).


<script src="https://cdnjs.cloudflare.com/ajax/libs/openlayers/4.6.4/ol.js">
</script>

<script>
  var head = document.getElementsByTagName('head')[0];
  var link = document.createElement('link');
  link.rel = 'stylesheet';
  link.href = 'https://cdnjs.cloudflare.com/ajax/libs/openlayers/4.6.4/ol.css';
  head.appendChild(link);

  var pos = ol.proj.fromLonLat([8.82937, 53.06180]);

  var map = new ol.Map({
    layers: [
      new ol.layer.Tile({
        source: new ol.source.OSM()
      })
    ],
    target: 'map',
    controls: ol.control.defaults(),
    view: new ol.View({
      center: pos,
      zoom: 17
    })
  });

  var markerElement = document.getElementById('marker');
  var marker = new ol.Overlay({
    position: pos,
    element: markerElement
  });

  map.addOverlay(marker);
  markerElement.style.display = 'block';
</script>
