# Waste POI Dash - INEOS OXIDE

Waste POI Dash is een webapplicatie voor het visualiseren en beheren van afvalinzamelpunten en -routes bij INEOS OXIDE (Nieuwe Weg 1, 2070 Zwijndrecht, België). Dit dashboard maakt gebruik van Mapbox GL JS voor de interactieve kaart, Firebase Firestore voor het opslaan van markers en lijnen, en biedt een moderne, mobielvriendelijke zijbalk voor gemakkelijke toegang tot alle functies.

## Functies

- **Interactieve kaart**: Aangedreven door Mapbox GL JS, met ondersteuning voor meerdere stijlen (standaard/satelliet) en geolocatie.
- **Sidebar menu**: Accordion-gebaseerde zijbalk om kaartacties, markers, lijnen te beheren en filters toe te passen.
- **Markerbeheer**: Voeg afvalpunten toe, bewerk, verwijder en filter markers (containers, ecopark containers) opgeslagen in Firestore.
- **Lijnen tekenen**: Teken, sla op en verwijder routes direct op de kaart en sla ze op in Firestore.
- **Filteren**: Zoek en filter markers op naam, afvalstof en type (container/ecopark).
- **Responsief ontwerp**: Geoptimaliseerd voor desktop en mobiel met een inklapbare zijbalk.

## Gebruikte technologieën

- **Mapbox GL JS**: Voor het renderen van interactieve kaarten en besturingselementen.
- **Firebase Firestore**: Voor realtime opslag en ophalen van marker- en lijndata.
- **JavaScript (ES modules)**: Voor alle hoofdlogica en UI-interacties.
- **HTML/CSS**: Maatwerk stijlen voor moderne UI en zijbalk layout.

## Aan de slag

### Vereisten

- Moderne webbrowser (Edge, Chrome, Firefox, Safari)
- Mapbox account ([Haal een access token op](https://www.mapbox.com/))
- Firebase project ([Firestore opzetten](https://firebase.google.com/docs/firestore))

### Installatie

1. **Kloon de repository**:
   ```bash
   git clone https://github.com/VandenOstende/wastedash.git
   cd wastedash
   ```

2. **Configureer Mapbox en Firebase**:
   - Werk je Mapbox access token bij in het JavaScript-gedeelte van `index.html`.
   - Vervang de Firebase-configuratie door jouw projectgegevens.

3. **Open `index.html` in je browser**:
   Geen build-stappen nodig. Alle afhankelijkheden worden via CDN geladen.

## Gebruik

- **Kaartbediening**: Gebruik de zijbalk om naar de vaste INEOS locatie te gaan, je eigen locatie te tonen en van kaartstijl te wisselen.
- **Markers**: Voeg nieuwe markers toe via "Voeg marker toe" en klik op de kaart. Bewerk/verwijder markers door erop te klikken of dubbelklikken.
- **Lijnen**: Klik op "Lijn tekenen" om een route te tekenen. Sla de getekende lijn op of verwijder via de popup.
- **Filters**: Filter markers op naam, afvalstof of type via de zijbalk.

## Voorbeeld Firebase-configuratie

```js
const firebaseConfig = {
  apiKey: "JOUW_API_KEY",
  authDomain: "JOUW_AUTH_DOMAIN",
  projectId: "JOUW_PROJECT_ID",
  storageBucket: "JOUW_STORAGE_BUCKET",
  messagingSenderId: "JOUW_SENDER_ID",
  appId: "JOUW_APP_ID",
  measurementId: "JOUW_MEASUREMENT_ID"
};
```

## Voorbeeld Mapbox-setup

```js
mapboxgl.accessToken = 'JOUW_MAPBOX_ACCESS_TOKEN';
```

## Licentie

MIT License. Zie [LICENSE](LICENSE) voor details.

## Auteur

- [VandenOstende](https://github.com/VandenOstende)

## Live demo

Open gewoon `index.html` in je browser—dit is het enige bestand dat je nodig hebt om het dashboard te starten!

---

Voor vragen of bijdragen, open een issue of pull request op GitHub.
