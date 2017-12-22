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

<div id="map" class="map"></div>
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


<script src="http://www.openlayers.org/api/OpenLayers.js"></script>
<script>
  var map = new OpenLayers.Map('map');
  var mapnik = new OpenLayers.Layer.OSM();
  var markers = new OpenLayers.Layer.Markers('Markers');

  map.addLayer(mapnik);
  map.addLayer(markers);

  var lonLat = new OpenLayers.LonLat(8.82937, 53.06180).transform(
    new OpenLayers.Projection("EPSG:4326"), map.getProjectionObject()
  );

  markers.addMarker(new OpenLayers.Marker(lonLat));
  map.setCenter(lonLat, 17);
</script>
