# Windows-Server 2019
### R.A.I.D

Beim initialen Boot das Raid-Konfiguration ausführen

### Basis Konfiguration Server
1. Serverbetriebssystem installieren
2. Administrator-Kennwort ändern
3. Computername ändern (Systemeigenschaften)

##### Rollen und Features
1. Rollen und Features bearbeiten
2. Installationstyp: Rollenbasierte oder featurebasierte Installation
3. Rollen: DHCP-Server, DNS-Server, Active Directory-Domänendienste

Nach der Installation der Features müssen die Konfigurationen angepasst werden.

##### Server zum Domänencontroller heraufstufen
1. Neue Gesamtstruktur hinzufügen und Standarddomäne vergeben (endet auf .local !)
2. Gesamtstrukturfunktionsebene: Gibt an in welcher Version das Active Directory installiert wird
3. Domänenfunktionsebene: Gibt an in welcher Version das Active Directory installiert wird für die Domäne
4. Domänencontrollerfunktionen: 
> DNS-Server
> Globaler Katalog`
5. Kennwort für den Verzeichnis-Wiederherstellungsmodus

##### DNS-Server
1. Start > Alle Apps > Windows Verwaltungsprogramme
2. Forward-Lookupzone existiert bereits
3. Reverse Lookupzone einrichten (Rechtsklick > neue Zone)
4. Primäre Zone auswählen
5. [Domänenname].local
6. IPv4 Reverse Lookupzone wird noch benötigt
7. Netzwerk-ID eintragen

##### DNS-Weiterleitungen einrichten
1. Rechtsklick auf Domain-Server > Eigenschaften
2. Reiter Weiterleitungen und bearbeiten
3. Adresse Router eintragen

##### DHCP-Server 
1. Start > Alle Apps > Windows-Verwaltungsprogramme
2. Rechtsklick IPv4 > Neuer Bereich
3. Beschreibung definieren und Adressbereich für Clients zuweisen

##### Active Directory Benutzer und Gruppen erstellen
1. Tools > Active Directory-Benutzer und Computer
2. Sicherheits-Gruppen: 
Fi18
> FI-Systemintegration
> FI-Anwendungsentwicklung

3. Organisationseinheiten:
> Benutzer_FI-AE
> Benutzer_FI-SI

4. Benutzer 
> Kennwort und Name vergeben

