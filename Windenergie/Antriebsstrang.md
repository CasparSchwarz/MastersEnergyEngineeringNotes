## Mechanischer Antriebsstrang
Der mechanische Antriebsstrang ist verantwortlich für die Aufnahme von Kräften und Momenten, die durch Wind, Gewichtskräfte und Kipp- und Giermomente entstehen.

### Triebstranglagerung
1. Wellenlagerung
	- 3-Punkt Lagerung
	- 4-Punkt Lagerung
2. Momentenlagerung (zweireihiges Kegelrollenlager)
3. Integrierte Lagerung
4. Zapfenlagerung / Nabenlagerung
	- Angestellte Lagerung
	- Fest / Los Lagerung

|Lagerungskonzept|Charakteristische Eigenschaften|Verwendete Lagertypen|
|-|-|-|
|Wellenlagerung: 3-Punkt Lagerung|Teilintegrierte Bauform; Getriebe wird durch Biegung und Torsion belastet|Hauptlager / Festlager: 2-reihige Pendellrollenlager oder Kegelrollenlager in X-Anordnung;; Steglager / Plantenlager: Zylinderrollenlager|
|Wellenlagerung: 4-Punkt Lagerung|Zwei Hauptlager; Aufsteckgetriebe mit Drehmomentstütze; Großer Bauraum, hohes Gewicht|Drehmomentstütze|
|Momentenlagerung|Hauptlager in Getriebe integriert; Aufnahme von Axial- und Radialkräften und Biegemomenten; Besonders kompakte Bauform|2-reihiges Kegelrollenlager in O-Anordnung; 3-reihiges Zylinderrollenlager|
|Zapfen- / Nabenlagerung|Zwei Hauptlager bilden die Lagerung; Einsetzbar für Getriebeanlagen und getriebelose Anlagen; Minimale Schub und Biegebelastungen auf Getriebe||


### Maschinenträger
- Zentrales Bauteil der Gondel einer Windenergieanlage
- Sichert die statische Festigkeit der GEsamtkonstruktion
- Trägt Rotor, Getriebe und Generator
- Aufnahme zum Teil sehr hoher Torotmomente
-> Unterliegt hohen dynamischen Lasten
-> Hohe Torotmomente erfordern besonders steife Bauweise
-> Hohe Qualitätsanforderungen im Herstellprozess

### Getriebekonzepte
**Anforderungen**
- Übertragung und Wandlung von Drehmoment und Drehzahl
- Zuverlässig & wartungsarm
- Dauerfest
- Hohe Leistungsdichte
- Hoher WIrkungsgrad
- Geräuscharm
- Schwingungsarm
- Kostengünstig

#### Planetengetriebe
Vorteile:
- Geringes Bauvolumen und Gewicht
- Leistungsverzweigung
- Koaxiale Lage von An- und Abtrieb
- Große Übersetzungsverhältnisse
- Hoher Wirkungsgrad

Nachteile
- Statisch überbestimmtes System bei mehr als drei Planeten
- Planschverluste insbesondere bei hohen Umlaufgeschwindigkeiten
![[Pasted image 20231219094831.png]]
**Berechnung**
- Unterteilung des komplexen Drehzahlverhaltens in zwei Teilbewegungen
	1. Bewegung des Standgetriebes
		- Festhalten des Steges führt zum Standgetriebe
		- Zentralräder bewegen sich mit Relativdrehzahlen gegenüber dem Steg
		- Bewegung rein durch Abwälzen beschrieben
		- Standübersetzung: $i_{12S}=\frac{n_{1S}}{n_{2S}}=\frac{z_2}{z_2}$
		- Da Hohlrad innenverzahnt: **Hohlrad-Zähnezahl ist negativ**
	2. Kupplungsanteil
		- Die Zentralräder 1 und 2 sowie der Steg S laufen als Block, wie eine starre Kupplung rum $n_1=n_2=n_S$
- Drehzahlgrundgleichung für Umlaufrädergetriebe nach WILLIS: $n_1-i_{12}\cdot n_2-(1-i_{12})\cdot n_S$

Elastische Planetenaufnahme:
- Verwendbarkeit hoher Anzahlen von Planeten
- Gleichmäßige Lastverteilung auf alle Planeten
- Selbstausgleich durch elstiasche Verformungen
- Elastizitäten können zu schlechten Zahnkontakten führen
- Zahnkorrekturen werden aufgehoben
- Zahnradschäden aufgrund unterwünschter Zahnkontakte

#### Alternative Konzepte
|Konzept|Vorteil|Nachteil|
|-|-|-|
|Mechanisch Mid Speed|Kompakte Bauform|Keine elektrische Isolation|
|Hydrodynamisches Verstellgetriebe|Geregelte Ausgangsdrehzahl|Große Baulänge|
|Elektro-mechanisch|Synchrongenerator direkt am Netz|FRT / Schwarzstart|
|Hydrostatisches Getriebe|Anschluss mehrere Generatoren|Hydrospeicher benätigt|

## Elektrischer Antriebsstrang
### Elektrotechnische Grundlagen
- Ohm'sches Gesetz $U=R\cdot I$
- Elektromagnetische Induktion $U=\frac{d\Phi}{dt}$
- Magnetischer Fluss $\Phi = B\cdot A$
- Elektrische Leistung $P = U\cdot I$
- Ohm'sche Verlustleistung $P_v = R\cdot I^2$

### Synchrongenerator
|Synchrongenerator|Stator|Rotor|
|-|-|-|
|Permanenterregt|Statorwicklungen 3-phasig|Permanentmagnet (Neodyn)|
|Fremderregt|Statorwicklungen 3-phasig|Polrad; Rotorwicklung; Bürstenapparat|

Bei **permanenterregten Synchrongeneratoren** werden die Magente aus Neodym gefertigt, wobei jedoch ein chinesisches Monopol auf Neodym besteht. Neodym kann auch in Deutschland abgebaut werden, jedoch ist die Gewinnung von Neodym extrem Umweltkritisch, da dabei radioaktive Elemente aus dem Boden gelöst werden.

Bei **fremderregten Synchrongeneratoren** werden Elektromagneten anstatt Permanentmagneten verwendet. Die Elektromagneten müssen mit Gleichstrom über einen Bürstenapparat versorgt werden.

Die **elektrische Polpaarzahl** bestimmt die erzeugte Netzfrequenz bei einer bestimmten Drehzahl: $n\cdot p = f$

### Ansynchrongenerator
- Drehzahl ist asynchron zur Netzfrequenz
	- Generatorbetrieb $n_S < n$
	- Motorbetrieb $n_S > n$
- Induzierte Läuferspannung ist proportional zum Schlupf
- Passiver Rotor ist sehr robust

**Kurzschlussläufer**
- Passiver Rotor
	- Squirrel Cage
	- Leiterstäbe
	- Kurschlussring zum kurzschließen
- Stator ähnlich wie Synchronstator
-> Drehzahlvariabler Betrieb nicht möglich

**Doppelt gespeister Asynchrongenerator (DFIG)**
- Aktiver Rotor mit
	- Zusatzwiderständen
	- Schleifringen
	- Rotor ist an einen Umrichter angeschlossen
	- Rotor kann unter- und übersyncrhon laufen, je nachdem speist der Generator den Umrichter oder der Umrichter den Generator
- Stator
	- Statorwicklungen direkt mit Stromnetz verbunden
-> Drehzahlvariabler Betrieb möglich

### Umrichter
Die Aufgabe eines Umrichters ist die Spannungstransformation und Frequenzanpassung um Strom in das bestehende Stromnetz einzuspeisen.

**Aufbau**
- Gleichrichter: Wandelt Wechselstrom in Gleichstrom
- Wechselrichter: Wandelt Gleichstrom in Wechselstrom
- Zwischenkreis: Lamm uir Nereotsteööigm vpm Göeocjstrp, f+r das Rptpr,agmetfeöd om Symcjrpmgemeratoren verwendet werden
-> Umrichter ändern Spannung und Frequenz und können Blindleistung bereit stellen

### Generatorkonzepte
#### Synchrongenerator mit direkter Netzkopplung
- Drehzahl fix durch Netzfrequenz
- Netzsynchronisation erforderlich
- Schleifkontakte erforderlich
- Empfindlich gegenüber Schwankungen in Netz und Wind
- Hohe Belastung des Triebstrangs
- Veraltetes System für die Windenergie
![[Pasted image 20231219102652.png]]

#### Synchrongenerator mit Vollumrichter
- Permanenterregter Synchrongenerator
	- Keine Erregerleistung erforderlich daher guter Wirkungsgrad
	- Keine Schleifkontakte erdorderlich
	- Teure Permanentmagnetmaterialien
	- Umwandlung der erzeugten Frequenz auf Netzfrequenz im Umrichter
- Fremderregter Synchrongenerator
	- Gleichstromerregung über Schleikontakte
	- Umwandlung der erzeugten Frequenz auf Netzfrequenz im Umrichter
![[Pasted image 20231219102859.png]]

#### Asynchrongenerator mit direkter Netzkopplung
- Keine Schleikontakte
- Keine Drehzahlregelung möglich
- Hohe Anlaufströme
- Veraltetes System
- Erfüllt nicht die aktuellen Netzanschlussrichtlinien
![[Pasted image 20231219102958.png]]

#### Ansynchrongenerator mit Vollumrichter
- Keine Schleifkontakte
- Drehzahlregelung über Umrichter
- Hohe Umrichterleistung (teuer)
![[Pasted image 20231219103043.png]]

#### Asynchrongenerator doppelt gespeist
- Drehzahlregelung über Variation der Frequenz des Rotorstroms
- Über- und untersynchroner Betrieb
- nur ca. 30 % Umrichterleistung
![[Pasted image 20231219103321.png]]

