# Integration von Wärmepumpen in Gebäuden
Im Neubausenktur werden seit 2021 mehr als 50 % Wärmepumpen als Wärmeerzeuger eingebaut. Auch im Renovierungsbereich nimmt der Anteil von Wärmepumpen zu. Jedoch machen Wärmepumpen in der Gesamtbilanz aller verbauten Wärmepumpen nur 2,6 % der Erzeuger aus (2020).

### Anforderungen im Gebäudesektor
![[Pasted image 20231218140338.png]]

Bewertung der unterschiedlichen Wärmequelle im Gebäudesektor

|Quelle|Anschaffung|Betrieb|Besonderheiten|
|-|-|-|-|
|Luft|Geringer Invest und Simple Installation|Geringere Effizienz & weniger planbar|Bereifung & Akustik und komplexere Auslegung|
|Sole|Hoher Invest durch Erdreichbohrung|Hohe Effizienz und Frostschutz|Genehmigung bei Tiefbohrung erforderlich|
|Grundwasser|Hoher Invest|Hohe Effizienz und Frostschutz|Genehmigung erforderlich und Einfluss auf Grundwasser|

Bewertung der unterschiedlichen Wärmesenken im Gebäudesektor

|Senke|Gebäude|Trägheit|Kühlung|Temperatur|
|-|-|-|-|-|
|Heizkörper|Altbau und Sanierung|Gering aber Speicher nötig|Nur bedingt|Funktion von Fläche, Art...|
|Flächenheizung|Neubau und Sanierung|Hoch|Ja|Gering, da große Flächen|
|Zuluft|Neubau da Kanalnetz vorhanden|Gering|Ja|Mittel (25-52 °C; 15-20 °C)|


Bei wasserbasierten Wärmesenken gibt es je nach Anwendung unterschiedliche Anforderungen:
- Warmwasser für Duschen und Trinken
	- Normative Temperaturanforderungen zwischen 25°C und 55°C
	- Durch hohe Leistungsanforderung ist Speicher notwendig
	- Legionellenwachstum muss unterbunden werden (Erhöhung von Wasser über 60 °C)
- Warmwasser im Sommer
	- Häufiges Takten der Wärmepumpe
	- Einfluss auf Lebensdauer der Wärmepumpe
-> Nutzung separater Brauchwasserwärmepumpen

## Auslegung
Aufgrund hoher Anschaffungskosten muss eine genaue Auslegung der Wärmepumpe erfolgen. Bei der Auslegung von Wärmepumpen existiert eine Antiproportionalität zwischen Angebot und Nachfrage:
- Mit steigender Außentemperatur
	- Sinkt Wärmebedarf (Nachfrage)
	- Steigt Wärmepumpenleistung (Angebot)
Daraufhin kann die Wärmepumpe auf zwei Arten ausgelegt werden:
- Monovalent
	- Hohe Anschaffungskosten
	- Häufiges Takten
- Bivalent
	- Deckungsanteil nicht 100 %
	- Ggf. höhere Betriebkosten
Demnach ist die optimale Auslegung abhängig von:
- Anteil Invest zu Betriebskosten
- Strom- und Gaspreise
- Betriebsführung
- Standort
- Nutzerverhalten

## Bivalente Systeme
- Betrieb von sekundärem Gerät wenn Außentemperatur < Bivalenztemperatur
- Im Regelfall Wärmepumpe mit Heizstab

Verschiedene Verschaltungsmöglichkeiten
- Mit / ohne Speicher
- Speicher in Reihe / Parallel (hydraulische Weiche)
- Mehrere Heizkreise
- Mit / ohne TWW-Erwärmung
- Unterschiedliche Orte für bivalente Erzeuger
Diverse Leitfäden und Verschaltungen
- Bundesverband Wärmepumpe (BWP): 11 Arten
- Bundesverband der Deutschen Heizungsindustrie (BDH): 6 Arten
- Hersteller nochmals mit eigenen, anderen Lösungen
Schnittstellen der Regelung
- Bei einer bestehenden Gastherme ist Kommunikation der Geräte nicht gegeben
- Gleiche Regelgrößen können kontraproduktiv sein
### Bivalent alternativ
- Abschaltung der Wärmepumpe wenn Außentemepratur < Bivalenztemperatur
- Üblicherweise für Wärmepumpe und Gastherme
- COP der Wärmepumpe muss größer als Strom-Gaspreisverhältnis sein

### Bivalent teilparallel
- Wenn Bivalenzpunkt nicht der optimalen Ausschalttemperatur entspricht
- Fast nur Vorteile gegenüber alternativer Betriebsweise
- Nachteil: Kompliziertere Steuerung

#### Verschaltungsmöglichkeiten
|Verschaltung|Vorteile|Nachteile|
|-|-|-|
|Serie mit Speicher|Einfache Produktion & Einfacher Einbau|Nur ein Massenstrom möglich & Zwei Geräte regeln auf eine Größe|
|Parallel WP und Heizstab|Einfache Produktion & Zwei Massenströme möglich|Komplexere Regelung der Ventile, Zwei Geräte regeln auf eine Größe & Mischungsverluste|
|Hinter Speicher|Unterschiedliche Regelgrößen|Viele Bauteile nötig, Komplexere TWW Beladung & Komplexerer hydraulischer Abgleich|


# Wärmepumpen für Industrieanwendungen
In der Industrie werden im Großteil Hochtemperaturwärmepumpen eingesetzt, da im Industriebereich neben Heizwärme auch Prozesswärme bereitgestellt werden muss. Bei Betrachtung des Temperaturniveaus in der Industrie liegen 44 % in einem Bereich, der durch Wärmepumpen bereitgestellt werden kann (0 °C - 200 °C). Oberhalb von 200 °C muss beispielsweise grüner Wasserstoff eingesetzt werden (für Schmelz- oder Gießprozesse).
## Kältemittel
Herausforderungen:
- Chemische Stabilität (mit höherer Temperatur werden die Moleküle instabiler)
- Taulinie wird bei Hochtemperaturkältemitteln oft steiler
	- Tropfenschlag kann Problem werden
	- Höhere Überhitzungen notwendig
Andere Temperaturanforderungen als Gebäudewärmepumpen
- Weniger potentielel Kältemittel aufgrund spezieller Anforderungen
- Problematik mit Tieftemperatur
	- Wärme muss immer noch abgegeben werden
	- Nutztemperaturniveaus liegen bei -50 °C / -80 °C
	- Sehr hohe Temperaturhübe erforderlich

**Ammoniak (R717)**
- Kritischer Druck von 113 bar
- Sehr kompakte Anlage aufgrund sehr hoher volumetrischer Heizenergie
- Führt zu sehr hoher Effizienz
- Toxisch und mäßig brennbar
- Hohes Maß an Sicherheitstechnik notwendig

**Wasser (R718)**
- Günstig, nicht brennbar, nicht toxisch, hohe chemische Stabilität
- Bei Betrieb unterhalb von 100 °C ist Unterdruck notwendig
- Verdichtung führt zu extrem hohen Temperaturen

**Wasser und Ammoniak haben hohe latente Wärmemengen, führen aber auch zu hohen Prozesstemperaturen (Zwischenkühlung nötig)**

## Kältekreise
- Deutlich höhere Leistungen in Industrieanwendungen als im Gebäudebereich
	- Betriebskosten überwiegen Invest
	- Häufig breiter Betriebsbereich notwendig
	- Anpassungen am Kreislaufschema rentieren sich schneller
- In Industrie häufig zusätzlicher interner Wärmeübertrager für Prozessstabilität
- Mögliche Kreisläufe der Industrie
	- Wärmepumpenkaskaden
	- Vorwärmung der Senke sowie Nutzung von Verdichterreihenschaltungen
	- Expandersysteme

## Prozessführung
- Parallelschaltung von Verdichtern
	- Regelung der Wärmeleistung über zu- und Abschalten von Verdichtern
	- Oft ein Drehzahlgeregelter Verdichter, Rest On-Off Verdichter
- Kaskadierung von Wärmepumpen
	- Kaskadierung nicht nur im Schema selbst möglich
	- Reihenschaltung oder Parallelschaltung von vollständigen Wärmepumpensystemen (Erhöhte Anforderungen an die Regelung des Gesamtsystems)
**Überkritische Prozessführung:**
- Effizient für Anwendungsfälle mit hoher Temperaturdifferenz der Senke
- Anwendung im Automobilsektor & Trocknungsprozessen
- Ab 30 K Spreizung in der Wärmesenke kann überkritische Prozessführung attraktiv werden

# Mobile Anwendungen und alternative Prozesse
- Keine brennbaren Kältemittel möglich -> Sehr starke Einschränkung aufgrund SIcherheitsanforderungen
- Eingeschränkter Bauraum
- Instationär
- Großer Einfluss von Störgrößen

| Kenngröße | Gebäuderaum | Fahrgastraum (PKW) |
| ---- | ---- | ---- |
| Volumen | Ca. 30 m³ | ca. 3 m³ |
| Volumen pro Person | > 10 m³ / Person | > 0,6 m³ / Person |
| Betriebsweise | Stationär | Instationär |
| Lufttemperatur | 15 °C - 30 °C | -25 °C - 80 °C |
| Oberflächentemperatur | 15 °C - 40 °C | -25 °C - 100 °C |
| Temperaturfeld | Nahezu homogen | Inhomogen |
| Strömungsfeld | Nahezu homogen | Inhomogen |
| Strahlungsfeld | Nahezu homogen | Inhomogen |
| Anströmungsgeschwindigkeit | ca. 0,2 m/s | < 5 m/s |
| Luftwechselrate | 2 - 8 1/h | 10 - 200 1/h |

# Bewertung von Wärmepumpen

**Jahresarbeitszahl (JAZ/SCOP)**:
- nach DIN EN 14825: Drei Klimazonen (Wärmer, Mittel, Kälter)
- VDI 4650:
	- Quelle Sole und Wasser: Eine Randbedingung
	- Quelle Luft: Drei Randbedingungen: -7, 2, 7°C

In den Verfahren zur Bestimmung der Leistungszahlen gibt es eine erhebliche Diskrepanz zwischen Norm und Realität. Grund dafür sind:
- Keine Betrachtung von Dynamiken
- Keine Betrachtung der Regelung
- Diskrepanz Wetter und Klimazonen

### Mögliche Systemgrenzen
- Bilanzgrenze entscheidet über SCOP
- Weitere Geräte müssen betrachtet werden
	- Ventilator
	- Pumpen
	- Heizstab
- Weiter Verluste
	- Speicher
	- Rohrleitungen

Für den Nutzer und Endkunden ist der SCOP des Gesamtsystems relevant, sodass alle Verbraucher des Heizsystems betrachtet werden müssen und nicht nur der Kältekreis.