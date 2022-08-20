---
layout: page
title: Social Event
---

This year's State of the Map is complemented with a get-together where you can have some nice food and drinks, have a chat with friends, make new contacts and more.

The social event is hosted at <a href="https://www.mercatocentrale.com/florence/">Mercato&nbsp;Centrale</a> in the centre of Florence.

The party will take place on Saturday, August 20, starting at 8pm. The venue is open until midnight.

<div id="map" style="height:420px; width:100%"></div>

## How it works

At the conference registration desk, you will be provided with a special voucher card with which you can get food from the different stalls in the Mercato on Saturday evening. The card has a credit of €40 that can be spent directly in all the shops of the venue (excluding The Pantry and Tosca restaurant), where you will have the opportunity to choose the dishes that are most suitable for you. There are all kinds of food and drinks <a href="https://www.mercatocentrale.com/florence/artisans/">offered</a>, from local Italian food to various international specialities. You will also be able to find many vegetarian and vegan dishes. If you have any special dietary requirements (for example uncommon food allergies), let us know via an email to [sotm@openstreetmap.org](mailto:sotm@openstreetmap.org), such that we can check whether there will be adequate options available for you at the venue.

The venue is not exclusively booked for State of the Map, so please expect that there will also be non-SotM-attendees at the Mercato. There will however be tables reserved for us in a dedicated section of the seating area of the venue: Look out for SotM signs and people in SotM shirts. Please also bring your conference badge with you, such that the staff can easily direct you to our space. Our tables are located on an entire aisle of the brewery and the three areas above the Tosca restaurant.

* The credit (€40) loaded on the cards will be spendable only on the day of the event until midnight
* Any remaining credit on the cards cannot be combined with other cards or paid out in cash
* The card can be used to buy takeaway products
* The cards can only be used inside the shops at the Mercato (excluding The pantry and Tosca restaurant)
* Please pay particular attention to not lose the card as they cannot be replaced
* Find here a map of the [food stalls](https://www.mercatocentrale.com/wp-content/uploads/2022/08/MCF22_WS_MAPPA_digitale_luglio_ITA-2048x1554.png) in the Mercato.

<script>
  document.addEventListener('DOMContentLoaded', function() {
    var map = L.map('map').setView([43.7766, 11.2532], 15);
    L.control.scale().addTo(map);
    L.tileLayer('{{ site.map_tiles.url}}', {
      attribution: '{{ site.map_tiles.attribution }}',
      maxZoom: {{ site.map_tiles.maxZoom}}
    }).addTo(map);
    map.scrollWheelZoom.disable();
    L.marker([43.77642, 11.25282], {icon: L.icon({
      iconUrl: "{{ "/img/logo/sotm_2022-logo.svg" | prepend: site.baseurl }}",
      iconSize: [40, 40],
      iconAnchor: [20, 40]
    })}).bindPopup("<h3>Mercato Centrale</h3><h4>Social Event Venue</h4><p><a href='https://www.openstreetmap.org/?mlat=43.7766&mlon=11.2532#map=16/43.7766/11.2532' target='_blank'>Open location on osm.org</a>.</p>").addTo(map);
  }, false);
</script>
