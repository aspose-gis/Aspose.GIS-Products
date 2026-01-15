---
title: GeoJSON naar SVG Converter
linkTitle: GeoJSON naar SVG Converter
weight: 10
description: Converteer GeoJSON data naar SVG formaat voor visualisatie en gebruik in webapplicaties.
url: /nl/net/viewer/geojson-to-svg/
aliases: [geojson2svg, geojson svg converter]
---

## Introductie

Deze tool converteert GeoJSON data naar SVG (Scalable Vector Graphics) formaat.  SVG is een XML-gebaseerd vectorafbeeldingsformaat dat geschikt is voor webapplicaties en visualisaties. Deze conversie maakt het mogelijk om geografische gegevens op een schaalbare en interactieve manier weer te geven in browsers.

## Functionaliteit

De GeoJSON naar SVG converter biedt de volgende functionaliteiten:

*   **GeoJSON input:** Accepteert GeoJSON data als invoer, of via een URL of een bestandsupload.
*   **SVG output:** Genereert SVG code op basis van de ingevoerde GeoJSON data.
*   **Stijlcafé:** Biedt opties om de stijl van de SVG elementen te beïnvloeden, zoals lijnkleur, vulling en breedte.
*   **Projectie:** Ondersteunt verschillende projecties voor nauwkeurige weergave van geografische data.
*   **Filtering:** Mogelijkheid om features op basis van attributen te filteren.

## Gebruik

1.  **Invoer:** Voer GeoJSON data in via een URL, bestandsupload of direct als tekst.
2.  **Configuratie (optioneel):** Pas de stijlinstellingen en projectie aan indien nodig.
3.  **Conversie:** Klik op de "Converteer" knop om de conversie te starten.
4.  **Output:** De gegenereerde SVG code wordt weergegeven in een tekstvak, klaar om gekopieerd en gebruikt te worden.

## Voorbeelden

### Eenvoudige puntlocatie

GeoJSON:

```json
{
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [10.45, 59.95]
  },
  "properties": {
    "name": "Amsterdam"
  }
}
```

SVG:

```xml
<svg width="200" height="200">
  <circle cx="100" cy="100" r="10" fill="red"/>
</svg>
```

### Lijnlocatie

GeoJSON:

```json
{
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [[10.45, 59.95], [10.50, 60.00]]
  }
}
```

SVG:

```xml
<svg width="200" height="200">
  <line x1="100" y1="100" x2="110" y2="110" stroke="blue" stroke-width="2"/>
</svg>
```

## Geavanceerde opties

*   **Projectie:** Selecteer een projectie om de geografische data correct weer te geven.  Veelgebruikte projecties zijn bijvoorbeeld Mercator en Lambert Azimuthal Equal Area.
*   **Stijlen:** Pas de stijl van de SVG elementen aan met behulp van CSS-achtige eigenschappen.  Je kunt bijvoorbeeld de kleur, breedte en vulling van lijnen en polygonen wijzigen.
*   **Filtering:** Filter features op basis van hun attributen om alleen relevante data weer te geven.

## Ondersteunde GeoJSON types

De converter ondersteunt de volgende GeoJSON geometrietypes:

*   Point
*   LineString
*   Polygon
*   MultiPoint
*   MultiLineString
*   MultiPolygon
*   GeometryCollection

## Probleemoplossing

*   **Ongeldige GeoJSON:** Zorg ervoor dat de ingevoerde GeoJSON data geldig is.  Gebruik een online GeoJSON validator om fouten te identificeren en te corrigeren.
*   **Onverwachte SVG output:** Controleer de stijlinstellingen en projectie om er zeker van te zijn dat ze correct zijn geconfigureerd.
*   **Performance problemen:** Voor grote datasets kan de conversie lang duren.  Overweeg om de data te filteren of te vereenvoudigen om de performance te verbeteren.

## Contact

Voor vragen of feedback, neem contact op met [support@example.com](mailto:support@example.com).
---
