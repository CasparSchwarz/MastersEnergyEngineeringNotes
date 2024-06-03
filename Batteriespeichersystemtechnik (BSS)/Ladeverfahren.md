# Ladeverfahren und Kriterien für die Detektion der Vollladung
## Lademanagement
Die Geschwindigkeit der Aufladung wird wesentlich von der Ladestrategie bestimmt:
- Dauer bis 80 % oder 100 % Aufladung
- Dauer des Nachladens für 100 km Reichweite

Ebenso sind Einflüsse auf die Lebensdauer zu beachten:
- Temperatur, Stromstärke, Spannung
- Überladen von Batterien kann zu schweren Unfällen sorgen

Um Netzüberlasten zu Vermeiden kann intelligentes Laden verwendet werden:
- koordiniertes Laden -> Leistungsspitzen und Netzüberlastungen vermeiden
- Vehicle-to-grid zur Strommarktstabilisierung

## Unterteilung des Ladevorgangs
Hauptladung
- Ladestrom fließt zum Großteil in die Hauptreaktionen
- Effekte der Nebenreaktionen spielen keine wesentliche Rolle

Nachladung
- Haupt- und Nebenreaktionen konkurrieren
- Ladegeschwindigkeit muss begrenzt werden
- Bei einigen Ladeverfahren: Dauer oder Intensität der Nachladephase in Abhängigkeit von der Hauptladung

Erhaltungsladung
- Kompensation der Selbstentladung
- Bei einigen Batterie-Technologien: Minimierung von Alterungseffekten

## Konstantstromladeverfahren (CC-Ladung)
- Ladeverfahren ist sehr einfach
- Konstantstromverfahren mit ein oder zwei Stromstufen üblich
- Abschaltkriterien zur Feststellung der Volladung bzw. der Beendung der Ladung wichtig:
	- Maximalspannung oder Gradient
	- Überschreitung der Maximaltemperatur oder des Temperaturgradienten

CC-Ladung am Zeitlimit
- Hauptladung mit konstantem Strom
- Überladen bei Erreichen des Volladezustands
	- Gesamter Ladestrom fließt in die Nebenreaktion
	- Signifikante Erwärmung der Batterie
	- Je nach Technologie: Zersetzung des Elektrolyten

CC-Ladung mit anderen Kriterien
- Realisierung kürzerer Ladezeiten durch höhere Ladeströme
- Geeignetes Abschaltkriterium nötig, abhängig von
	- Zelltyp
	- Ladegeschwindigkeit

## Abschaltkriterien bei CC-Ladung
- $U_{abs}$: kritisch, da temperatur-, alters- und typabhängig
- $-\Delta U$: häufig eingesetzt, kritisch bei hohen Temperaturen aufgrund von kleineren Spannungsmaxima
- $U_{max}$: prinzipiell optimal, aber hoher Aufwand und Kosten von Messtechnik
- $\frac{d^2U}{dt^2}=0$: Batterie noch nicht vollgeladen, daher Einsatz nur für Schnellstladung
- $T_{abs}$: kritisch, kann nur als Sicherheitskriterium dienen
- $\Delta T$: Abschalten nach einer Temperaturänderung seit Start des Ladevorgangs ist möglich, typischer Wert ca. 15 K
- $\frac{dT}{dt}$: Steigung der Temperatur liegt im Bereich 1...6 K/min. Gute Ermittlung der Vollladung möglich
- $\frac{d^2T}{dt^2}=0$: Temperatur liegt unter Umständen bei unerlaubt hohen Temperaturen, sodass Wendepunkt als Abschaltkriterium ungeeignet

## Konstantspannungsverfahren (U-Ladung)
- Ladung mit konstanter Spannung führt zu sinkendem Strom nach bestimmter Ladedauer
- Mit zunehmendem Ladezustand
	- Anstieg der Ruhespannung
	- Anstieg des Innenwiderstands
	- Kleiner werdende Spannungsdifferenz zwischen Ladegerät und Batterie
- Nachteil
	- Sehr hoher Ladestrom zu Beginn der Ladung (normalerweise keine reine U-Ladung)
	- Teures Ladegerät

