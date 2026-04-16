BakkerBartel
BakkerBartel is een webapplicatie voor het beheren van werknemers en vakantieaanvragen binnen een bakkerij.
De applicatie is gebouwd met ASP.NET Core Blazor Server, Entity Framework Core en SQL Server.

Functionaliteiten
werknemers beheren
werknemers actief of inactief zetten
vakantieaanvragen indienen
vakantieaanvragen goedkeuren of afwijzen
notities toevoegen aan aanvragen
kalenderoverzicht van aanvragen bekijken
bezettingscontrole bij het goedkeuren van aanvragen
Gebruikte technieken
C#
ASP.NET Core Blazor Server
Entity Framework Core
SQL Server / SQL Server Express
Blazorise
Radzen
Projectstructuur
Bakkerbartel/Bakkerbartel
De hoofdapplicatie.
Bakkerbartel/Bakkerbartel/Components
De pagina's en layout van de applicatie.
Bakkerbartel/Bakkerbartel/Entities
De domeinmodellen zoals Employee en VacationRequest.
Bakkerbartel/Bakkerbartel/Data
Databasecontext, repositories en seeddata.
Bakkerbartel/Bakkerbartel/Services
Businesslogica van de applicatie.
Benodigdheden
Voor het starten van dit project heb je nodig:

.NET 10 SDK
SQL Server of SQL Server Express
een lokale SQL Server instantie die bereikbaar is via localhost\\SQLEXPRESS
Database-instelling
De applicatie gebruikt standaard deze connection string in appsettings.json:

"DefaultConnection": "Server=localhost\\SQLEXPRESS;Database=BakkerBartelDb;Trusted_Connection=True;TrustServerCertificate=True;MultipleActiveResultSets=true"
Als jouw SQL Server instantie anders heet, pas dan de connection string aan in:

appsettings.json
Project opstarten
1. Open de juiste map
Ga in de terminal naar:

cd C:\.....\
2. Herstel de packages
dotnet restore
3. Build het project
dotnet build
4. Start de applicatie
dotnet run
Na het starten laat de terminal een lokale URL zien, bijvoorbeeld:

https://localhost:xxxx
Open die URL in de browser.

Database en seeddata
Bij het opstarten van de applicatie gebeurt automatisch het volgende:

de database wordt aangemaakt of bijgewerkt via Entity Framework migrations
voorbeelddata wordt ingeladen
Daardoor kun je de applicatie direct testen zonder eerst handmatig gegevens toe te voegen.

Testgebruik
Bij het openen van de app kun je op de homepagina een gebruiker kiezen.

Kies een beheerder om werknemersbeheer, kalender en aanvragenoverzicht te openen.
Kies een medewerker om eigen aanvragen te bekijken en nieuwe vakantieaanvragen in te dienen.
Belangrijke onderdelen in de code
Program.cs
Registreert services en start de applicatie.
ApplicationDbContext.cs
Regelt de databasekoppeling en relaties.
VacationRequestService.cs
Bevat de logica voor vakantieaanvragen.
EmployeeManagementService.cs
Bevat de logica voor werknemersbeheer.
Versiebeheer
Dit project is bedoeld om samen met git versiebeheer aan te tonen.
Voor het portfolio-examen kan naast deze repository ook bewijsmateriaal worden toegevoegd, zoals:

screenshot van de commit history
screenshot van branches
screenshot van pull request of merge request
Opmerking voor examinator
Dit project is een complete repository met werkende applicatiecode, businesslogica, databasekoppeling en gebruikersinterface.
De applicatie is lokaal op te starten met de bovenstaande stappen.

