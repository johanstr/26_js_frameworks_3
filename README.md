# MODULE 26: JavaScript Frameworks 3
|   |   |
|---|---|
| Demo versie  | 1.0  |
| Auteur | J.J. Strootman (SMN) |
| Framework | VueJS Versie 3.3.4 |
|||  
  
*Demonstratie project ten behoeve van de instructies*  
  
## Een Game Webshop
In dit project is een simpele (maar niet volledige) **webshop** gemaakt.  
  
### Navigatiebalk
Op de navigatiebalk vind je twee menu items terug. De eerste brengt je terug naar de startpagina, de tweede brengt je naar de winkelwagen.  
Daarnaast zie je rechts op de balk een icoon van een winkelwagen. In dit icoon wordt met een getal aangegeven hoeveel items(games) er in de winkelwagen zitten.  
  
### Startpagina
Op de startpagina zien we een overzicht van games. In dit overzicht kun je een game toevoegen aan de winkelwagen. Het effect van het toevoegen zien we in de navigatiebalk (rechts) terug in een icoon. Het aantal items in de winkelwagen wordt hier getoond. De info button bij iedere game is niet geïmplementeerd.  
  
### Winkelwagen
De winkelwagen wordt als een tabel getoond. Per game in de winkelwagen zien we een rij in de tabel met de ID, de titel, de stuksprijs, het aantal van de game en het subtotaal voor deze ene game. In de laatste kolom vinden we per game een icoon terug waarmee we de game uit de winkelwagen verwijderen.  
Onderaan de tabel vinden het totaal bedrag voor de gehele winkelwagen terug.  
Het aantal van een game kan met iconen (links en rechts van het aantal) aangepast worden. Is het aantal teruggebracht naar 0 dan zal de game automatisch verwijdert worden uit de winkelwagen.  
  
## Technieken toegepast

| Techniek | Versie | Opmerkingen  |
|---|---|---|
| Pinia  | 1.0 | Een statemanager voor VueJS |
| Vue-router | 4.2.5 | Routing systeem voor VueJS |
| VueJS | 3.3.4 | JavaScript Framework
|||  
  
### Pinia
Met Pinia kunnen we werken met persistente data. Data die dus blijven bestaan en beschikbaar zijn in alle delen van de applicatie.  
  
### Vue-router
Vue-router stelt ons in staat om met clean-urls de verschillende pagina's van onze applicatie te bereiken.  
  
## Clonen van de repository
### Pre-requisites
#### NodeJS
Een voorwaarde voor het werken met deze repository is dat je NodeJS hebt geïnstalleerd op je computer.  
  
#### Git
Een tweede voorwaarde is dat je git-bash hebt geïnstalleerd om via de terminal de git opdrachten te kunnen gebruiken.  
  
Je kan uiteraard ook een UI interface gebruiken.

### Clonen
Clone de repository op je lokale schijf met de volgende terminal opdracht:  
  
```bash
git clone https://github.com/johanstr/26_js_frameworks_3 webshop
```  
  
Daarna moeten alle javascript packages en bibliotheken nog geïnstalleerd worden. Dit doe je met de volgende terminal opdracht:  
  
```bash
cd webshop
npm install
```  
  
Om je applicatie in een browser te openen start je de applicatie met de volgende terminal opdracht:  
  
```bash
npm run dev
```  
  
Je ziet als resultaat van deze laatste opdracht een URL staan. Met CTRL+klik kun je deze URL openen in de browser.