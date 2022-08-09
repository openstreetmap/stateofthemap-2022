---
layout: page
title: Social Event
---

This year's State of the Map is complemented with a get-together where you can have some nice food and drinks, have a chat with friends, make new contacts and more.

The social event is hosted at <a href="https://www.mercatocentrale.com/florence/">Mercato&nbsp;Centrale</a> in the centre of Florence.

The party will take place on Saturday, August 20, starting at 8pm.

<div id="map" style="height:420px; width:100%"></div>

## How it works

You will be provided with a special voucher card with which you can get food from the different stalls in the Mercato. There are all kinds of food and drinks offered, from local Italian food to various international specialities.

The venue will not be exclusively booked for the State of the Map only, so please expect that there are also non-SotM attendees at the Mercato. There will however be tables reserved for us in a dedicated section of the seating area of the venue: Look out for SotM signs and people in SotM shirts. Please also bring your conference badge with you, such that the staff can easily direct you to our space.

<script>
  document.addEventListener('DOMContentLoaded', function() {
    var map = L.map('map').setView([43.7766, 11.2532], 15);
    L.control.scale().addTo(map);
    L.tileLayer('{{ site.map_tiles.url}}', {
      attribution: '{{ site.map_tiles.attribution }}',
      maxZoom: {{ site.map_tiles.maxZoom}}
    }).addTo(map);
    map.scrollWheelZoom.disable();
    L.marker([43.7766, 11.2532], {icon: L.icon({
      iconUrl: "{{ "/img/logo/sotm_2022-logo.svg" | prepend: site.baseurl }}",
      iconSize: [40, 40],
      iconAnchor: [20, 40]
    })}).bindPopup("<h3>Mercato Centrale</h3><h4>Social Event Venue</h4><p><a href='https://www.openstreetmap.org/?mlat=43.7766&mlon=11.2532#map=16/43.7766/11.2532' target='_blank'>Open location on osm.org</a>.</p>").addTo(map);
  }, false);
</script>
