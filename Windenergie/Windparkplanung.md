# Rechtlicher Rahmen
## Flächenausweisung
**Windenergieanlagen sind im Außenbereich als privilegierte Anlagen zulässig**

Beschränkung durch **Flächennutzungsplan**
- Ermöglicht einer Kommune die Ausweisung von Flächen zur Windenergienutzung
- Eine anderweitige Nutzung der Gebiete wird damit ausgeschlossen
- Grundlage für den Flächennutzungsplan ist eine Flächenanalyse

Bei **Tabuzonen** wird zwischen harten Tabuzonen und weichen Tabuzonen unterschieden:
- **Harte Tabuzone**: aus tatsächlichen und/oder rechtlichen Gründen ausgeschlossen (bspw. Naturschutzgebiete)
- **Weiche Tabuone**: Tatsächlich und rechtlich möglich, es soll aber keine WEA aufgestellt werden (bspw. Abstandsflächen zu Siedlungen)

# Planung durch Projektentwickler
**Ziel**: Die Entwicklung eines erfolgreichen Windparkprojektes bei gegebenen Randbedingungen

Relevante Faktoren und Randbedingungen:
- **Wirtschaftlichkeit**
- **Technische Machbarkeit**
- **Akzeptanz der Bevölkerung**
- Infrastruktur
- Artenschutz
- Netzanschluss
- Topologie
- Wettbewerb
- Naturschutz
- Flächensicherung
- Flächeneigenschaften
- Schatten- und Schallrestriktionen

## Standortanalyse
- Verfügbare Flächen
	- FNP (Konzentrationszonen)
	- Ausreichende Größe
- Kriterien für Projektierer
	- Windverhältnisse -> erwartbarer Ertrag
	- Größe und Topographie der Flächen
	- Netzanschluss
	- Mögliche Restriktionen
- Flächensicherung
	- Pachtvertrag mit Landbesitzer
	- Pachtpreise ca. 5-9 % der Einnahmen durch WEA
	- Teilweise fixe Nutzungsentgelte vor Baubeginn

### Windgutachten
**Windhöffigkeit** beschreibt das jährliche theoretische Energiemaximum an erzeugter Windenergie. Die reale Ausbeute liegt dabei unter der Windhöffigkeit und wird beeinflusst durch die tatsächliche Leistungsausbeute und gesetzliche Rahmenbedingungen, die einen durchgehenden Betrieb nicht zulassen.

$P=\frac{1}{2}\cdot c_p\cdot\rho\cdot A\cdot v^3\cdot\eta_{Anlage}$ -> Windgeschwindigkeit muss so genau wie möglich gemessen werden.
-> **Windmessmast**
- mindestens 2/3 Nabenhöhe oder höher
- Ausgestattet mit unterschiedlicher meteorologischer Sensorik
- Stationär
- 10 min Mittelwerte der Windgeschwindigkeit und Richtung

**SODAR** (Sonic Detecting and Rangeing)
- Funktion über Dopplereffekt
- Anfällig für Störgeräusche
- Anfällig für Regen
- Transport in einem Anhänger
- Messung konusförmig über dem SODAR (20 m bis 200 m)
- 10 min Mittelwerte von Windgeschwindigkeit und Richtung

**LiDAR** (Light Detection and Rangeing)
- Funktion über Dopplereffekt
- Höhere Genauigkeit als SODAR
- Störung durch Nebel und extrem klare Luft
- Transport in einem ANhänger
- Messung konusförmig über dem LiDAR (40 m bis 200 m)
- 10 min Mittelwerte von Windgeschwindigkeit und Richtung

### Leistungsausbeute
**Aerodynamische Abschattung**
- Eine WEA hinter einer anderen steht in dessen Windschatten -> verringerte Leistungsausbeute
	- Reduzierter Parkwirkungsgrad
	- Einfluss auf Statik aufgrund turbulenter Nachlaufströmungen
- Orientierung an Hauptwindrichtung auf Basis eines erstellten Windgutachtens

Nachlaufeffekte werden beschrieben durch:
$V_{nach}(X)=V_{vor}-(1-\sqrt{1-C_T})\cdot (1+\frac{skX}{D})^{-2}\cdot V_{frei}$
mit
- $V_{nach}$ Windgeschwindigkeit nach Trubine an Entfernung X
- $V_{vor}$ Anströmgeschwindigkeit vor Turbine
- $V_{frei}$ Ungestörte Windgeschwindigkeit
- $C_T$ Schubkoeffizient
- $k$ Nachlaufzerfallskonstante
- $X$ Abstand von Interesse
- $D$ Rotordurchmesser

## Netzanbindung
Zur Netzanbindung muss ein Antrag auf Anschluss der WEA bei dem Netzbetreiber gestellt werden. Der Netzbetreiber ermittelt daraufhin den optimalen Netzanschlusspunkt, womit die Innerparkverkabelung ausgelegt werden kann.

## Behördliche Auflagen
### Schallimmission
- Beurteilung mittels eines Beurteilungspegels anch DIN ISO 9613-2
- Beurteilung Schallimmission am Immissionspunkt unter Berücksichtigung von Abschirmwirkungen, Dämpfungen und Schallreflexionen
- ggf. Zuschläge für Ton- oder Impulshaltigkeit
- Zusätzlich müssen bereits existierende Zusatzbelastungen berücksichtigt werden

Bei Nicht-Einhaltung -> Möglichkeit eines schallreduzierten Betriebs
Schallreduzierung erfolgt durch Drosselung der Anlagenleistung -> Ertragsminderung

### Schattenwurf
Der rotierender Rotor führt zu einem sich bewegendem Schatten (Schlagschatten). Dieser stellt eine optische Belastung dar, welche maximal 30 min pro Tag oder 8 h pro Jahr bestehen darf. Wird das Pensum an maximalen Schattenwurf aufgebraucht, muss die WEA angehalten werden, bis der Schatten nicht mehr auf den den Immissionspunkt trifft.