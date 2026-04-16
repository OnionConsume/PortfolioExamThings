# User Story 1: Overzicht van mijn vakantieaanvragen

## Algemene informatie
- **ID:** US-01
- **Epic:** Vakantieaanvragen
- **Titel:** Werknemer kan eigen vakantieaanvragen bekijken
- **Prioriteit:** Must have
- **Status:** Done

## User story
**Als** werknemer van Bakkerij Bartels  
**wil ik** mijn ingediende vakantieaanvragen kunnen bekijken in de applicatie  
**zodat** ik altijd inzicht heb in welke aanvragen nog openstaan, welke zijn goedgekeurd en welke zijn afgewezen.

## Beschrijving
Binnen Bakkerij Bartels is het belangrijk dat medewerkers duidelijk kunnen zien wat de status is van hun vakantieaanvragen. In een handmatige of onduidelijke werkwijze kan snel verwarring ontstaan over de vraag of een aanvraag al is behandeld, nog in behandeling is of al is goedgekeurd. Dat kan leiden tot miscommunicatie tussen medewerker en beheerder.

Met deze functionaliteit krijgt de werknemer een eigen overzichtspagina binnen de applicatie. Op deze pagina worden alle eerder ingediende vakantieaanvragen van de ingelogde gebruiker getoond. Per aanvraag moet zichtbaar zijn over welke periode de aanvraag gaat en welke status deze momenteel heeft. Hierdoor hoeft een medewerker niet meer apart navraag te doen en ontstaat er meer duidelijkheid in het aanvraagproces.

Deze functionaliteit draagt direct bij aan het digitaliseren van het administratieve proces rondom verlof. De werknemer krijgt meer zelfstandigheid en de beheerder hoeft minder losse vragen te beantwoorden over de voortgang van aanvragen.

## Waarom deze functionaliteit belangrijk is
Deze user story is belangrijk omdat medewerkers snel en zelfstandig moeten kunnen controleren wat er met hun aanvraag is gebeurd. Zonder dit overzicht blijft de communicatie afhankelijk van mondeling overleg of losse berichten. Door een centraal overzicht aan te bieden wordt het proces transparanter, betrouwbaarder en gebruiksvriendelijker.

## Acceptatiecriteria
- De werknemer kan alleen zijn of haar eigen vakantieaanvragen zien.
- Per aanvraag is de begin- en einddatum zichtbaar.
- Per aanvraag is de status zichtbaar, bijvoorbeeld `In behandeling`, `Goedgekeurd` of `Afgewezen`.
- De aanvragen worden in een duidelijk overzicht getoond.
- Het overzicht is alleen toegankelijk voor ingelogde gebruikers.
- Nieuwe aanvragen verschijnen ook in dit overzicht nadat ze zijn opgeslagen.

## Definition of Done
- Er is een pagina of component waarin de werknemer zijn eigen aanvragen kan bekijken.
- De gegevens worden correct opgehaald op basis van de ingelogde gebruiker.
- De status van elke aanvraag wordt duidelijk weergegeven.
- De functionaliteit werkt zonder foutmeldingen in de interface.
- De functionaliteit is getest binnen de applicatie.

## Relatie met het project
Deze user story ondersteunt het doel van het project om de administratie binnen Bakkerij Bartels te digitaliseren. Medewerkers krijgen meer inzicht in hun eigen aanvragen en het verlofproces wordt overzichtelijker en minder foutgevoelig.

## Mogelijke technische invulling
Voor deze functionaliteit is een pagina nodig waarin de aanvragen van de huidige gebruiker worden opgehaald vanuit de database. Daarbij moet gebruik worden gemaakt van de gebruikerscontext, zodat alleen de juiste gegevens zichtbaar zijn. De interface moet de aanvragen in een logische lijst of tabel tonen met de bijbehorende status.
