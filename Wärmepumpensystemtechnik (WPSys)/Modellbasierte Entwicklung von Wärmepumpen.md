## Grundlagen der Produktentwicklung
Bei der Entwicklung eines neuen Produkts ist das Ziel, einen Mehrwert für den Kunden und die Gesellschaft zu schaffen. Dazu gehören bspw. bessere Qualität und neue Funktionalitäten. Ebenso muss auf auf neue Vorgaben (Gesetze und Regularien) geachtet werden.

Durch die hohen Anzahl an Stakeholdern und Beteiligten bei der Produktentwicklung sowie die steigende Komplexität der Produkte ist eine **systematische Vorgehensweise** notwendig.

### V-Modell nach VDI 2206
Das V-Modell beschreibt die systematische Vorgehensweise bei der Produktentwicklung.
1. Systementwurf
	- Anforderung an Gesamtsystem (bsp. Produkt muss auf Europalette passen)
	- Anforderung an Einzelkomponenten
	- Detaillierungsgrad steigt stetig
2. Systemintegration
	- Von Einzelkomponente zum Gesamtsystem
	- Eigenschaftsabsicherung als Kontrollmechanismus
![[Pasted image 20231207151113.png]]
Das Vorgehen in der Realität ist iterativ, sodass einzelne Schritte mehrfach durchgeführt werden müssen. Eine klare und konkrete Anforderungsermittlung ist dabei Entscheidend für eine funktionierende Produktentwicklung und sollte nicht übergangen werden.

### Integrierte Produktentwicklung
Bei der integrierten Produktentwicklung wird nicht nur das Produkt sondern auch das Verbundsystem betrachtet, in welchem das Produkt verwendet werden soll.

## Grundlagen der Modellierung und Simulation
Ein **Modell** ist eine vereinfachte Nachbildung eines geplanten oder existierenden Systems mit seinen Prozess in einem anderen begrifflichen oder gegenständlichen System. Es unterscheidet sich hinsichtlich der untersuchungsrelevanten Eigenschaften nur innerhalb eines vom Untersuchungsziel abhängigen Toleranzrahmens vom Vorbild.

Eine **Simulation** ist ein Verfahren zur Nachbildung eines Systems mit seinen dynamischen Prozessen in einem experimentierbaren Modell, um zu Erkenntnissen zu gelangen die auf die Wirklichkeit übertragbar sind.

### Klassifizierung von Modellen
Modelle unterscheiden sich in:
- Räumlich diskrete Modelle
	-  0-D Modell:
		- Keine räumliche Auflösung
		- Fokus auf Zustandsänderung gesamter Komponente
	- 1-D Modell
	- 2-D Modell
	- 3-D Modell
- Zeitlich diskrete Modelle
	- Stationäre Modellierung
		- Zeitlich konstant
		- Ein spezifischer Betriebspunkt
		- Keine Dynamiken
	- Transiente Modellierung
		- Zeitliche Differnetialgleichungen
		- Dynamischer Betrieb möglich
		- Hoher numerischer Rechenaufwand
	- Quasi-Stationär
		- Aneinanderreihung stationärer Zustände
		- Sprunghafte Zustandsänderung
		- Erhöhte numerische Stabilität
- ihrem Modellansatz (Physikalisch, Semi-physikalisch, etc.)
- Datenbasiert / Physikalisch
	- White-Box
		- Genaue Prozesskenntnisse
		- Basiert auf mathematischen Beschreibungen von physikalisches Gesetzmäßigkeiten
		- Grundlegendes Systemverständnis notwendig
	- Black-Box
		- Keine Prozesskenntnisse
		- Basiert auf Messdaten, die in Experimenten generiert werden
		- Keine physikalische Beschreibung der Beobachtungen
		- Keine Extrapolation möglich
	- Grey-Box
		- Einige Prozesskenntnisse
		- Kombination aus Black- und White-Box


### Wahl des Modells
Die Wahl des Modells ist davon abhängig, was modelliert werden soll:
- Komponentenentwicklung
	- Leistungsanforderungen in definierten Betriebpunkten
	- Wechselwirkungen zwischen Komponenten, Verschaltungen und Kältemittel
	- Komplexe thermodynamische Zusammenhänge
	- -> Detaillierte Modelle notwendig
	- -> tendenzielle (quasi-) stationäre Modelle
- Reglerentwicklung Kältekreis
	- Fokus auf Dynamik des Kältekreises
	- Lastwechsel / Kontinuierlich ändernde Randbedingungen
	- -> Transiente Modelle
	- -> Hoher Rechenaufwand
	- -> Erste Vereinfachungen
- Systementwicklung Gebäudeebene
	- Mehrere Systemkomponenten (WP, Speicher, PV)
	- Betrachtungszeitraum ~ Jahr
	- Optimierung
- Dimensionierung Energiesystem
	- Mehrere Erzeuger und Nutzer
	- Betrachtungszeitraum ~ Jahr(-zehnte)
	- Optimierung

## Modellansätze für Wärmepumpen
Für die Modellierung von Wärmepumpen gibt es zwei Ansätze:
- Modellierung der Wärmepumpe als ein Bauteil
- Explizite Modellierung des Kältekreises

### Wärmepumpe als ein Bauteil
- Konstanter COP
	- Sehr starke Vereinfachung
	- Geeignet für komplexe Rechnungen von Energiesystemen
- Carnot-COP + Carnot-Effizienz (konstant)
	- Abbildung der Temperaturabhängigkeit des COP
- Carnot-COP + Carnot-Effizienz (variabel)
	- Abbildung von Teillastverhalten des COP
- Komplettes Kennfeld der Wärmepumpe
	- Datengetriebenes Black-Box Modell
- Komponentenweise erstelltes Modell
	- Verdichter, Wärmeübertrager, Kältemittel

### Verdichter
- CFD Modelle
	- Detaillierte Geometriekenntnisse
	- Mehrdimensionale Navier-Stokes-Gleichungen
	- Geeignet für Konzeptionierung von Verdichtern
- Modellierung über Effizienzmodelle
	- Isentroper Wirkungsgrad
	- Volumetrischer Wirkungsgrad
	- Mech. + el. Wirkungsgrad
- Modellierung mittel Tabellen / Polynomen
	- Black-Box-Modelle
	- Herstellerangaben

### Wärmeübertrager
- Phasenwechsel in WÜ
- Methode der zusammengefassten Parameter
	- Vereinfachung des WÜ zu einem Kontrollvolumen
	- Gemittlete Sotff- und WÄrmeübertragereigenschaften
	- Anwednung der NTU-Methode nach VDI-Wärmeatlas
- Zonierungsmodell - Moving Boundary Modelly
	- Unterteilung in Zonen
	- Berücksichtigung unterschiedlicher Eigenschaften in verschiedenen Phasen
- Finite-Volumen-Methode (FVM)
	- Unterteilung in konstante Volumina
	- Hoher Rechenaufwand aufgrund von hoher Diskretisierung

### Kältemittel
- Abbildung von Stoffeigenschaften und Transporteigenschaften
	- Enthalpie, Entropie usw
	- Wärmeleitfähigkeit, Viskosität
- Stoffdaten auf Basis von Fundamentalgleichungen
	- Helmholtz-Funktion
	- Basierend auf Messdaten
- Implizite und explizite Berechnungsmethoden
	- Polynominale Ansätze interpolationsbasiert
	- Vereinfachte Methode
- Blackbox Modelle
	- Neuronale Netze zur Vorhersage von thermodynamischen Eigenschaften