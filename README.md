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


### Article page
De artikel pagina is eerst ontworpen en vervolgens gebouwd met dynamische data die wordt opgehaald uit de database. De artikel pagina bevat:
1. Coverafbeelding
2. Titel
3. Intro-tekst
4. Comments plaatsen, en deze comments bekijken

<img width="1853" height="898" alt="image" src="https://github.com/user-attachments/assets/723c162c-203c-4bb7-85ff-11e07a08e6da" />

https://github.com/IsaacEswa/pleasurable-ui/blob/b91812a7ede0afc4e9951a679d121df96e921e91/public/styles/style.css#L587-L599

https://github.com/user-attachments/assets/70a0a910-4f5b-43b3-b599-d855cf75ae59

Binnen de pagina word er gebruik gemaakt van een view transition.

https://github.com/user-attachments/assets/59394378-755f-49d5-8548-fec3ee9d3bf9


Ook is het mogelijk om een comment te plaatsen op verschillende artikelen. Elk district heeft z'n eigen huisstijl, deze huisstijl is toegepast op de card van deze `section`.


## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met JS gedaan en hoe? Misschien heb je iets met NodeJS gedaan, of heb je een framwork of library gebruikt? -->

### Article page

https://github.com/user-attachments/assets/70a0a910-4f5b-43b3-b599-d855cf75ae59

Op de article page zijn scroll-driven animations toegepast. Deze animaties zijn gekoppeld aan de scrollpositie van de gebruiker, waardoor elementen geleidelijk verschijnen of bewegen tijdens het scrollen. Dit zorgt voor een moderne gebruikerservaring, trekt de aandacht naar belangrijke content en verbetert de leesbaarheid van de pagina. Daarnaast zijn deze animaties efficiënt omdat ze geen gebruik maken van javascript.

https://github.com/IsaacEswa/pleasurable-ui/blob/b91812a7ede0afc4e9951a679d121df96e921e91/public/client.js#L1-L61
Binnen de pagina kan een comment geplaatst worden zonder een full page refresh. Dit kan door client side javascript, inplaats van de server. Binnen de client word een nieuwe fetch gedaan, en de nieuwe comment word automatisch toegevoegd bij de comments section.

https://github.com/IsaacEswa/pleasurable-ui/blob/b91812a7ede0afc4e9951a679d121df96e921e91/public/styles/style.css#L711-L718
Om te voldoen aan de contraststandaarden gebruik ik voor verschillende knoppen de CSS-waarde `contrast-color`. Deze functie kiest automatisch een tekstkleur die de beste contrastverhouding biedt op basis van de achtergrondkleur.

## Installatie
<!-- Bij Instalatie staat hoe een andere developer aan jouw repo kan werken -->

## Bronnen

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
