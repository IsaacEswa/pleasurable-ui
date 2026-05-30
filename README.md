# Pleasurable User Interface

Ontwerp en maak met een team voor een opdrachtgever een interface waar gebruikers blij van worden.

De instructie vind je in: [INSTRUCTIONS.md](https://github.com/fdnd-task/pleasurable-ui/blob/main/docs/INSTRUCTIONS.md)



## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Gebruik](#gebruik)
  * [Kenmerken](#kenmerken)
  * [Installatie](#installatie)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
<!-- Bij Beschrijving staat kort beschreven wat voor project het is en wat je hebt gemaakt -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->

## Gebruik
<!-- Bij Gebruik staat de user story, hoe het werkt en wat je er mee kan. -->
### Homepage
De homepage is eerst ontworpen en vervolgens gebouwd met dynamische data die wordt opgehaald uit de database. De homepage bevat:
1. Het meest recente artikel als eye-catcher
2. Daarnaast de 3 volgende meest recente artikelen
3. Daaronder de drie meest recente artikelen (card component) per district

De [Card Component](https://github.com/IsaacEswa/pleasurable-ui/blob/main/views/partials/cardComponent.liquid) bevat de volgende onderdelen:
1. Coverafbeelding
2. Doelgroep
3. Datum
4. Titel
5. Intro-tekst met een limiet van twee regels

De Card Component is mogelijk in [light en dark mode](https://github.com/IsaacEswa/pleasurable-ui/blob/fa0670932c3eab8f8733a9c3e4bbeacab39941a7/public/styles/styleguide.css#L8-L53). Ik heb `@media (prefers-color-scheme: dark)` gebruikt. 

De [coverafbeelding](https://github.com/IsaacEswa/pleasurable-ui/blob/fa0670932c3eab8f8733a9c3e4bbeacab39941a7/views/partials/cardComponent.liquid#L3-L21) wordt ingeladen met het `picture` element. Dit is beter voor de performance


## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met JS gedaan en hoe? Misschien heb je iets met NodeJS gedaan, of heb je een framwork of library gebruikt? -->

## Installatie
<!-- Bij Instalatie staat hoe een andere developer aan jouw repo kan werken -->

## Bronnen

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
