# Testscenario's BakkerBartel

## Case 1: Werknemer opent eigen aanvragen

### 1. Testscenario
Werknemer opent de applicatie, kiest zichzelf op de homepagina en opent de pagina met eigen vakantieaanvragen.

### 2. Testdata
- Werknemer: **Sanne de Vries**
- Pagina: **Mijn vakantieaanvragen**

### 3. Verwacht resultaat
- De homepagina laadt correct.
- De werknemer kan gekozen worden.
- De pagina **Mijn vakantieaanvragen** opent correct.
- Het formulier voor een nieuwe aanvraag is zichtbaar.

### 4. Werkelijk resultaat
De homepagina laadde goed, Sanne de Vries kon gekozen worden en de pagina **Mijn vakantieaanvragen** ging gewoon open.

### 5. Status
Geslaagd

---

## Case 2: Aanvragenpagina zonder gebruiker

### 1. Testscenario
Gebruiker probeert de aanvragenpagina te openen zonder eerst een werknemer te kiezen.

### 2. Testdata
- Geen actieve gebruiker gekozen

### 3. Verwacht resultaat
- De applicatie toont een melding dat eerst een werknemer gekozen moet worden.
- De gebruiker kan niet direct verder naar de aanvragenpagina.

### 4. Werkelijk resultaat
De applicatie gaf gewoon netjes aan dat eerst een werknemer gekozen moest worden.

### 5. Status
Geslaagd

---

## Case 3: Ongeldige vakantieaanvraag zonder reden

### 1. Testscenario
Werknemer probeert een vakantieaanvraag in te dienen zonder reden.

### 2. Testdata
- Geldige startdatum
- Geldige einddatum
- Reden: leeg

### 3. Verwacht resultaat
- De aanvraag wordt niet opgeslagen.
- De applicatie toont een foutmelding of waarschuwing.

### 4. Werkelijk resultaat
De applicatie hield de aanvraag tegen en gaf aan dat de aanvraag niet volledig was.

### 5. Status
Geslaagd

---

## Case 4: Beheerder opent kalender en beoordeelt aanvragen

### 1. Testscenario
Beheerder opent de applicatie en gaat naar het kalenderoverzicht om openstaande aanvragen te bekijken.

### 2. Testdata
- Beheerder: **Bakkerbartel**
- Openstaande aanvragen in het systeem

### 3. Verwacht resultaat
- Het kalenderoverzicht opent correct.
- Openstaande aanvragen zijn zichtbaar.
- De beheerder ziet opties om aanvragen te beoordelen.

### 4. Werkelijk resultaat
De beheerder kon het kalenderoverzicht openen en het onderdeel **Aanvragen beoordelen** was zichtbaar.

### 5. Status
Geslaagd

---

## Case 5: Beheerder opent werknemerbeheer

### 1. Testscenario
Beheerder opent werknemerbeheer en bekijkt de werknemerslijst.

### 2. Testdata
- Beheerder
- Bestaande werknemers in de database

### 3. Verwacht resultaat
- De pagina **werknemerbeheer** opent correct.
- Werknemers zijn zichtbaar.
- De beheerder kan werknemers beheren.

### 4. Werkelijk resultaat
De werknemerslijst laadde goed en de beheeropties waren zichtbaar.

### 5. Status
Geslaagd
