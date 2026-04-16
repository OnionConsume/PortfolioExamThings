# Planning BakkerBV

## Huidige situatie (A)

Aan het begin van het project was er nog geen uitgewerkte webapplicatie voor Bakkerij Bartels. De repository bevatte nog nauwelijks projectinhoud en er was nog geen technische basis aanwezig voor de onderdelen die later nodig waren, zoals het beheren van medewerkers, het indienen van vakantieaanvragen en het tonen van planning of kalenderinformatie.

De eerste stap was daarom om het project technisch op te starten en een basis neer te zetten waarop latere functionaliteiten gebouwd konden worden.

## Doelsituatie (B)

De doelsituatie van dit project is een werkende administratie- en beheerapplicatie voor Bakkerij Bartels waarin medewerkers en beheerder digitale processen rondom vakantieaanvragen kunnen uitvoeren en volgen. Daarbij moet de applicatie:

- een duidelijke Blazor-interface hebben;
- medewerkers en aanvragen kunnen beheren;
- vakantieaanvragen kunnen opslaan in een database;
- medewerkers inzicht geven in hun eigen aanvragen;
- beheerders aanvragen laten beoordelen;
- controle uitvoeren op personeelsbezetting bij goedkeuring.

## Chronologische planning per sprint

## Sprint 1: Projectbasis en technische opstart

### Stap 1: Projectvoorbereiding en scope bepalen
- Oriëntatie op het project en bepalen welke hoofdonderdelen nodig zijn voor de applicatie.
- Verkennen van de eerste richting voor Blazor-interface, vakantieaanvragen en kalenderoverzicht.
- Vaststellen welke onderdelen eerst technisch voorbereid moesten worden voordat echte functionaliteit ontwikkeld kon worden.

**Gebaseerd op:**
- Dagverslag `23-03-2026`

### Stap 2: Repository en basisstructuur opzetten
- README en repositorywijzigingen verwerken.
- Eerste Blazor-projectopzet toevoegen.
- Basispagina's, layouts, routing en configuratie van de applicatie aanmaken.

**Gebaseerd op:**
- Commit `4b186d0` - README.md edited online with Bitbucket.
- Commit `c081b05` - Merged in SCRUM-60.
- Commit `0ebff49` - Initial Blazor project setup.
- Dagverslag `25-03-2026`

### Resultaat van sprint 1
- Er staat een technische basis waarop verdere functionaliteiten gebouwd kunnen worden.
- De applicatie is niet langer alleen een idee, maar heeft een werkende projectstructuur.

## Sprint 2: Kalender en basis van het aanvraagproces

### Stap 3: Kalenderpagina en eerste domeinmodellen opzetten
- Een kalenderpagina bouwen binnen de Blazor-interface.
- Een eerste Radzen scheduler opzetten.
- Modellen en services toevoegen voor medewerkers, afspraken en vakantieaanvragen.

**Gebaseerd op:**
- Commit `90570a5` - Add calendar page with Radzen scheduler setup.
- Dagverslag `27-03-2026`

### Stap 4: Reviewflow voor vakantieaanvragen verbeteren
- De flow voor het beoordelen van vakantieaanvragen verduidelijken.
- Een aparte pagina voor vakantieaanvragen toevoegen.
- Service-logica uitbreiden om aanvragen beter te verwerken.

**Gebaseerd op:**
- Commit `b9d8d34` - Refine vacation request review flow.
- Dagverslag `28-03-2026`

### Resultaat van sprint 2
- De applicatie heeft nu niet alleen een basisinterface, maar ook de eerste echte functionele onderdelen voor planning en vakantieaanvragen.
- De aanvraagverwerking begint zichtbaar vorm te krijgen.

## Sprint 3: Dataopslag en gebruikersflow uitbreiden

### Stap 5: SQL Server koppelen en gegevens persistent opslaan
- Een `ApplicationDbContext` toevoegen.
- Seeddata en een SQL-script maken.
- Services aanpassen zodat medewerkers en vakantieaanvragen niet alleen tijdelijk in geheugen staan, maar daadwerkelijk in de database worden opgeslagen.

**Gebaseerd op:**
- Commit `08ad04d` - SQL server persistecnce for vakantie aanvragen toegevoegd.
- Dagverslag `29-03-2026`

### Stap 6: Mijn aanvragen-overzicht en user context toevoegen
- Een pagina toevoegen waarop de werknemer zijn eigen aanvragen kan bekijken (`MyRequests`).
- Home- en kalenderpagina verder verbeteren.
- User context toevoegen, zodat de applicatie beter weet welke gebruiker is ingelogd en welke gegevens daarbij horen.

**Gebaseerd op:**
- Commit `0c84c8e` - Complete issue 13 and issue 36.
- Dagverslag `30-03-2026`

### Resultaat van sprint 3
- De applicatie heeft nu een werkende gebruikersflow waarin aanvragen niet alleen verwerkt, maar ook opgeslagen en per gebruiker weergegeven kunnen worden.
- De applicatie sluit beter aan op de user story waarin werknemers hun eigen vakantieaanvragen kunnen bekijken.

## Sprint 4: Validatie en personeelsbezetting

### Stap 7: Controle op personeelsbezetting toevoegen
- Extra validatie toevoegen aan het goedkeuringsproces van vakantieaanvragen.
- Een aparte `IStaffingService` en `StaffingService` ontwikkelen.
- Controleren of goedkeuren mogelijk is zonder dat de personeelsbezetting in gevaar komt.

**Gebaseerd op:**
- Commit `db94d60` - Add staffing approval check for SCRUM-15.
- Dagverslag `31-03-2026`

### Stap 8: Gebruikersmeldingen en testbaarheid verder verbeteren
- Controleren of meldingen in de interface duidelijk genoeg zijn.
- De werking van goedkeuren en afkeuren verder nalopen.
- Zorgen dat de functionele logica niet alleen technisch klopt, maar ook bruikbaar is voor de eindgebruiker.

**Gebaseerd op:**
- Vervolgstap uit dagverslag `31-03-2026`

### Resultaat van sprint 4
- De applicatie ondersteunt nu niet alleen het indienen en bekijken van aanvragen, maar ook inhoudelijke controle op basis van personeelsbezetting.
- Daarmee wordt het proces slimmer, realistischer en beter toepasbaar in de praktijk van Bakkerij Bartels.

## Samenvatting van de planning

De planning laat een logische opbouw zien:

1. Eerst is de technische basis van het project neergezet.
2. Daarna zijn kalender en aanvraagverwerking opgebouwd.
3. Vervolgens is de databasekoppeling toegevoegd en is de gebruikersflow uitgebreider gemaakt.
4. Tot slot is extra bedrijfslogica toegevoegd in de vorm van bezettingscontrole bij goedkeuren.

Deze volgorde is realistisch, omdat latere functionaliteiten afhankelijk waren van eerder werk. Zonder projectopzet was er geen interface, zonder services en modellen was er geen aanvraagproces, zonder database was er geen blijvende opslag en zonder die basis kon geen inhoudelijke validatie op personeelsbezetting worden toegevoegd.

## Relatie met opdracht 1.3

Deze planning ondersteunt criterium `1.3`, omdat duidelijk wordt:

- welke onderdelen van het project wanneer zijn ontwikkeld;
- dat de werkzaamheden in logische stappen zijn opgebouwd;
- dat de planning aansluit op de user stories en het projectdoel;
- dat de voortgang terug te leiden is naar concrete commits en dagverslagen.
