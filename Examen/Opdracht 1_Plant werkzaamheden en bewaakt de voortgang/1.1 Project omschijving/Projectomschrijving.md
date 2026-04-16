# Projectomschrijving: Administratie- en Beheerapplicatie

| | |
|---|---|
| **Bedrijf** | Bakkerij Bartels |
| **Team** | BakkerBV |
| **Doel** | Het digitaliseren en centraliseren van administratieve processen binnen de bakkerij, zodat medewerkers en beheerder sneller, duidelijker en met minder kans op fouten kunnen werken. |

## Overzicht

Voor Bakkerij Bartels werk ik aan een webapplicatie waarmee een aantal administratieve en organisatorische processen binnen het bedrijf op een centrale plek worden beheerd. In de huidige situatie verlopen veel handelingen nog via mondeling overleg, losse notities of verspreide bestanden. Dat maakt het lastiger om informatie terug te vinden, aanvragen te volgen en overzicht te houden op de planning van medewerkers.

Met dit project ontwikkel ik een applicatie die deze processen digitaliseert. Het doel is om belangrijke gegevens niet langer verspreid te laten staan, maar samen te brengen in een duidelijke en toegankelijke omgeving. Daardoor wordt het voor medewerkers eenvoudiger om acties uit te voeren, terwijl de eigenaar of beheerder beter inzicht krijgt in wat er speelt binnen het bedrijf.

## Aanleiding

Binnen een bakkerij is het belangrijk dat de personeelsplanning en de dagelijkse organisatie goed op elkaar aansluiten. Wanneer informatie over medewerkers, aanvragen en beschikbaarheid niet centraal wordt beheerd, kost dat extra tijd en ontstaat sneller onduidelijkheid. Denk bijvoorbeeld aan vakantieaanvragen die via losse berichten binnenkomen, of aan situaties waarin niet direct zichtbaar is of de personeelsbezetting voldoende blijft.

De aanleiding voor dit project is daarom het verbeteren van deze werkwijze. Door een digitale oplossing te bouwen, kunnen processen beter worden vastgelegd, sneller worden verwerkt en eenvoudiger worden gecontroleerd.

## Doel van het project

Het project heeft als doel om een gebruiksvriendelijke administratie- en beheerapplicatie te realiseren voor Bakkerij Bartels. De applicatie moet helpen bij het beheren van medewerkersgegevens, het indienen en beoordelen van vakantieaanvragen en het creëren van meer overzicht in de planning en bezetting.

Daarbij richt ik mij niet alleen op het tonen van gegevens in de interface, maar ook op de onderliggende logica. De applicatie moet namelijk niet alleen informatie opslaan, maar ook ondersteunen bij beslissingen. Een voorbeeld hiervan is het controleren of een vakantieaanvraag wel kan worden goedgekeurd zonder dat de personeelsbezetting in de knel komt.

## Belangrijkste functionaliteiten

De applicatie bestaat uit meerdere onderdelen die samen het administratieve proces ondersteunen:

- Een overzicht van medewerkers en hun gegevens.
- Een functionaliteit waarmee medewerkers zelf vakantieaanvragen kunnen indienen.
- Een beheerscherm waarin aanvragen kunnen worden bekeken, goedgekeurd of afgewezen.
- Een kalender- of planningsweergave om beter inzicht te geven in afspraken, aanvragen en beschikbaarheid.
- Controle op personeelsbezetting bij het verwerken van aanvragen.
- Opslag van gegevens in een database, zodat informatie bewaard blijft en later opnieuw gebruikt kan worden.

Door deze onderdelen te combineren ontstaat een applicatie die zowel praktisch inzetbaar is voor dagelijks gebruik als technisch voldoende uitgebreid is om te laten zien dat de software aansluit op echte wensen en eisen uit de praktijk.

## Gebruikers en stakeholders

De belangrijkste gebruikers van deze applicatie zijn:

- **Medewerkers van Bakkerij Bartels:** zij moeten op een eenvoudige manier aanvragen kunnen indienen en hun gegevens of aanvragen kunnen terugzien.
- **Eigenaar / beheerder:** deze gebruiker moet overzicht houden, aanvragen kunnen beoordelen en inzicht krijgen in de personeelsbezetting.
- **Ontwikkelteam / student:** ik gebruik dit project om te laten zien dat ik wensen uit de praktijk kan vertalen naar werkende software met een duidelijke structuur.

Deze stakeholders hebben ieder een andere behoefte, maar allemaal profiteren zij van meer overzicht, minder losse communicatie en een duidelijker proces.

## Technische context

De applicatie wordt ontwikkeld als een webapplicatie met een Blazor-interface. Binnen het project werk ik met pagina's, componenten, services, modellen en database-opslag. Voor onderdelen zoals planning en kalenderfunctionaliteit wordt een scheduler-opzet gebruikt. Daarnaast is er logica toegevoegd voor vakantieaanvragen, validatie en personeelscontrole, zodat de applicatie niet alleen gegevens toont maar ook bedrijfsregels ondersteunt.

Ook wordt gebruikgemaakt van een databasekoppeling met SQL Server, zodat medewerkers en aanvragen niet tijdelijk in het geheugen blijven staan maar daadwerkelijk persistent worden opgeslagen. Hierdoor sluit het project beter aan op een realistische praktijksituatie.

## Afbakening

Binnen dit project ligt de focus op de administratieve en organisatorische processen rondom medewerkers en vakantieaanvragen. Het project richt zich dus niet op de verkoop, kassaprocessen of productie van de bakkerij, maar op het verbeteren van de interne ondersteuning en het beheer.

De nadruk ligt op:

- digitalisering van bestaande handmatige processen;
- duidelijk beheer van medewerkers en aanvragen;
- inzicht in planning en bezetting;
- een werkende, logische en uitbreidbare technische basis.

## Verwacht resultaat

Het eindresultaat van dit project is een centrale beheerapplicatie waarmee Bakkerij Bartels efficiënter kan werken. Medewerkers kunnen zelfstandig aanvragen indienen, de beheerder kan deze beoordelen op basis van duidelijke informatie, en belangrijke gegevens zijn terug te vinden op één plek. Daarmee levert het project niet alleen technisch werkende software op, maar ook een oplossing die aansluit op een concreet probleem uit de praktijk.

Deze applicatie vormt daarmee een goede basis voor verdere uitbreiding in de toekomst, bijvoorbeeld met extra personeelsfuncties, uitgebreidere planning of aanvullende beheeropties.
