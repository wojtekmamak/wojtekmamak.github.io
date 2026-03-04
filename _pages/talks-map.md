---
layout: single
title: "Talks Map"
permalink: /talks-map/
author_profile: true
---

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<div class="talks-map">
  <h2>Where I've Presented</h2>
  <p>An interactive map showing locations of my conference talks, workshops, and invited seminars (2017-2025).</p>
  <div id="map"></div>
</div>

<script>
// Initialize map centered on Europe
var map = L.map('map').setView([50.0, 15.0], 4);

// Add OpenStreetMap tiles
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '© OpenStreetMap contributors',
    maxZoom: 18
}).addTo(map);

// Talk locations with details
var talks = [
    // Spain
    {lat: 43.3183, lng: -1.9812, title: "Re-visiting Historical Ontology Workshop", location: "San Sebastián, Spain", year: 2025},
    
    // USA
    {lat: 34.1377, lng: -118.1253, title: "10th Integrated History and Philosophy of Science", location: "Pasadena, CA, USA", year: 2025},
    
    // France  
    {lat: 48.7904, lng: 2.4555, title: "Practices Around Computation Symposium", location: "Paris, France", year: 2024},
    
    // Mongolia
    {lat: 47.9184, lng: 106.9177, title: "Study Visit Fellowship - NMU", location: "Ulaanbaatar, Mongolia", year: 2024},
    
    // Czech Republic
    {lat: 50.0755, lng: 14.4378, title: "Polish-Czech Academies Workshop", location: "Prague, Czechia", year: 2024},
    
    // Poland - Warsaw (multiple talks)
    {lat: 52.2297, lng: 21.0122, title: "Multiple talks at IFiS PAS", location: "Warsaw, Poland", year: "2017-2024", count: 8},
    
    // Poland - Kraków
    {lat: 50.0647, lng: 19.9450, title: "Philosophy in Informatics & Other conferences", location: "Kraków, Poland", year: "2017-2021", count: 3},
    
    // Poland - Other cities
    {lat: 49.2992, lng: 19.9496, title: "Cognitive Systems Modeling Conferences", location: "Małe Ciche & Kiry, Poland", year: "2017-2018", count: 2},
    {lat: 51.7592, lng: 19.4560, title: "Computer Games Culture Conference", location: "Łódź, Poland", year: 2017},
    
    // Bulgaria
    {lat: 42.6977, lng: 23.3219, title: "Bulgarian Academy of Sciences", location: "Sofia, Bulgaria", year: 2022},
    
    // Italy
    {lat: 45.4642, lng: 9.1900, title: "Measurement at the Crossroads", location: "Milan, Italy", year: 2022},
    
    // UK
    {lat: 51.5074, lng: -0.1278, title: "ESHS Biennial Conference", location: "London, UK", year: 2018}
];

// Custom icon for talk markers
var talkIcon = L.icon({
    iconUrl: 'https://raw.githubusercontent.com/pointhi/leaflet-color-markers/master/img/marker-icon-2x-red.png',
    shadowUrl: 'https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/images/marker-shadow.png',
    iconSize: [25, 41],
    iconAnchor: [12, 41],
    popupAnchor: [1, -34],
    shadowSize: [41, 41]
});

// Add markers for each talk
talks.forEach(function(talk) {
    var popupContent = '<strong>' + talk.title + '</strong><br>' +
                      talk.location + '<br>' +
                      'Year: ' + talk.year;
    
    if (talk.count) {
        popupContent += '<br>(' + talk.count + ' talks)';
    }
    
    L.marker([talk.lat, talk.lng], {icon: talkIcon})
        .addTo(map)
        .bindPopup(popupContent);
});
</script>

<style>
#map {
    height: 500px;
    width: 100%;
    margin-top: 2em;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.talks-map {
    margin: 2em 0;
    padding: 2em;
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.08);
}

.talks-map h2 {
    color: #C1694F;
    margin-top: 0;
}
</style>
