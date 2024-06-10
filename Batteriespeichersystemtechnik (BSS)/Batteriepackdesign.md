Ein Batteriepack beinhaltet die Batteriezellen, Elektronik, Anschlüsse nd thermische Elemente. Ein gesamtes Batteriepack kann somit direkt zum Ein- und Ausspeichern von elektrischer Energie genutzt werden.

Die Lebensdauer einer Batterie ist dabei von folgenden Faktoren abhängig:
- Packaufbau -> Temperierung
- Zellverschaltung -> Parallelschaltung vs. Serienschaltung
- Alterung abhängig von Betriebsbedingungen -> Lade- und Nutzungsmanagement
- Elektronik -> Balancingsystem

Entscheidend für den Erfolg eines Batteriespeichers sind die Kosten für den jeweiligen Speicher. 
# Sicherheit
![[Pasted image 20240610083601.png]]
Um die Sicherheit eines Batteriepacks zu gewährleisten, müssen während der Entwicklung einige Schritte berücksichtigt werden:
1. Im Vorfeld
	- Abschätzung der benötigten Batteriegröße
	- Auswahl einer Zellchemie
	- Auswahl eines Zelltyps
2. Systemauslegung
	- Schaltungskonzept
	- Zellverbinder / Anschlüsse
	- Schütze, Vorladung und Sicherungen
	- Kühlung und Heizung
	- Batteriemanagementsystem
3. Produktion & Betrieb
	- Aufbau
	- Prüfung
	- Betrieb und Wartung

![[Pasted image 20240610084019.png]]
# Auslegung
Elektrische Auslegung:
- Berechnung von
	- Leistung
	- Energie
- Abschätzung der Lebensdauer
	- zyklisch
	- kalendarisch

Auswahl einer passenden Batteriezelle
- Format
	- zylindrische Zelle
	- prismatische Zelle
	- Pouch-Bag Zelle
- Chemie
	- LFP, NMC, etc.

-> Elektrisches Konzept entwickeln (mit den gewählten Parametern, siehe oben)

Auslegung der Verschaltung
- Abschätzung der benötigten Batteriegröße
- Auswahl der Zellchemie
- Auswahl des Zelltyps
- Verschaltungskonzept

Systemkonfiguration
- Zellverbinder / Elektrische Verbindungen
- Schützbox (Schalter, Vorladung und Sicherungen)
- Kühlung und Heizung
- Batteriemanagement-system

Realisierung
- Struktur
- Testing
- Sicherheit auf Zellebene
- Sicherheit auf Systemebene
- Crashsicherheit

## Abschätzung der Batteriegröße
Wichtig für die Abschätzung der Batteriegröße sind Energie- und Leistungsdichte:
- Energiedichte
	- Energieinhalt pro kg
	- 80 .. 250 Wh/kg (Li Iionen)
- Leistungsdichtung (Leistung pro kg)

Es ist dabei zu unterscheiden zwischen theoretischen Energiedichten bezogen auf die Zellen und auf das Batteriepack. **Es ist nicht möglich, gleichzeitig hohe Leistungs- und hohe Energiedichte zu erreichen**. Oft sind auch die Energie- und Leistungsdichten in Bezug auf das Volumen sind relevant.

Im Batteriepack werden nur ca. 20 % bis 30 % der theoretischen Energiedichte des Materials erreicht.

Die Batteriewahl ist stark abhängig von der erwarteten Nutzung der Batterie:
- Elektromobilität
	- Privatnutzung: geringe regelmäßige Fahrleistung, wenige Langstrecken, kalendarische Alterung entscheidender Faktor
	- Flotteneinsatz: regelmäßige Nutzung, Batteriegröße kann optimal auf Anwendung angepasst werden, verfügbare Zyklenzahl wird tatsächlich genutzt
	- ÖPNV: ganztätige Nutzung, Batteriegröße und Ladeverfahren kann optimal auf Anwendung angepasst werden, verfügbare Zyklenzahl wird tatsächlich genutzt

Die Wahl der Batterie wird mit Hilfe des Ragone Diagramms realisiert.
## Modulare Batteriekonzepte
- Modularität erlaubt kundenspezifische Auslegung der Reichweite und Anpassung der Reichweite an veränderten Lebensbedingungen
- Hochleistungs- und Hochenergiebatterien können je nach Kundenwunsch kombiniert werden
- Mischen von Batteriepacks (Alter, Hersteller, Leistung)
- Teilasutausch der Batterie ist möglich

## Auswahl der Zellchemie
Faktoren für die Auswahl einer Zellchemie sind:
- Energiedichte
- Leistungsdichte
- Lebensdauer
- Thermisches Verhalten
- Lademöglichkeiten
- Kosten

Für Batteriepacks gibt es verschiedene Arten von elektrochemischen Speichern:
- Beli-Säure
- NiCd/NiMH
- Hochtemperatur (NaS, NaNiCl_2)
- Lithium-Ionen
- Redox-Flow

**Verschiedene Batterietechnologien im Vergleich**:
Blei-Säure Batterien:
- Große Anzahl an Installationen weltweit, erprobte Technologie
- Von zahllosen Herstellern kommerziell angeboten
- 80 bis 90 % Wirkungsgrad
- + Erfahrung, sichere Technologie, günstig
- - Lebensdauer, Gewicht

NiCd Batterien:
- Kommerzielles Produkt, verschiedene Hersteller am Markt
- Kosten 2-3 mal höher als Bleibatterien
- 70 bis 80 % Wirkungsgrad
- + Erfahrung, sichere Technologie, günstig
- - Lebensdauer, Gewicht
- - Umweltverträglichkeit Cadmium

NiMH (Nickel-Metallhydrid) Batterien:
- Einsatz vor allem in Hybridfahrzeugen
- Wenige Hersteller am Markt
- 70 bis 80 %
- + Gute Lebensdauer, robust, höhere Energiedichte als NiCd
- - Geringes Kostensenkungspotential, schlechtes Tief- und Hochtemperaturverhalten

Hochtemperatur Batterien:
- NaS: In Japan kommerziell genutzt als Netz-Energiespeicher
- NaNiCl_2: überwiegend im mobilen Bereich
- Jeweils nur ein Anbieter
- 70 bis 85 % Wirkungsgrad
- + Gute Zyklenlebensdauer
- - Jeweils nur ein Anbieter, thermisches Management aufwändig, hohe thermische Verluste

Redox-flow-Batterien:
- Demonstationsanlagen im Feld, auf dem Weg zur Kommerzialisierung
- 2 bis 3 komerzielle Anbieter
- Wirkungsgrad 70 bis 85 %
- Nur eingeschränkt USV-fähig
- + Energie und Leistung sind separat auslegbar, gute Zyklenlebensdauer
- - Vanadium ist teuer

Lithium-Ionen Batterien:
- Bereits vielfältige Anwendung im Consumer Bereich
- Hohe Energiedichte
- Stationärer Einsatz bei kurzen Entladezeiten
- Hohe Kosten, jedoch hohes Kostensenkungspotential
- Wirkungsgrad 90 bis 95 %
- + Sehr gute Zyklenlebensdauer
- - Teuer, aufwändiges Management

# Zellbauformen
Typische Bauformen von Batteriezellen sind
- prismatische Zellen
- puch-bag Zellen
- zylindrische Zellen

| Zylindrische Zelle                                                                 | Pouch-Bag Zelle                                       | Prismatische Zelle                                                         |
| ---------------------------------------------------------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------------------- |
| + Große Erfahrung aus Vonsumer-Produkten: sehr hohe Energiedichte, niedriger Preis | + Hohe Packungsdichte                                 | + Robust, hohe Steifigkeit                                                 |
| + Hohe intrinsische Sicherheit durch zellinterne Sicherheitsmechanismen            | + Einfache Kühlung bedingt durch große Oberfläche     | + Einfache Montage und Verkabelung                                         |
| - Zellgehäuse relativ teuer                                                        | + Variabel hinsichtlich Zellverkabelung über die Pole | +/- Kombiniert Eigenschaften der zylindrischen, sowie der Pouch-Bag Zellen |
| - Kühlung wegen des Oberflächen- / Volumenverhältnisses schwierig                  | - geringe Steifigkeit                                 | - Probleme mit internem Druck der Zellen                                   |
|                                                                                    | - Zellverspannung benötigt                            | - Kühlung wegen Oberflache zu Volumen schwierig                            |
|                                                                                    |                                                       | - Zellverspannung benötigt                                                 |
