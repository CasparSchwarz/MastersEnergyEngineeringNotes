Die Alterung von Batterien ist stark abhängig von:
- Temperatur
- Ladezustand
- Stromstärke bei der Aufladung
- Zyklentiefe

Dementsprechend gibt ist über die Nutzungsdauer deutliche Alterungsunterschiede zwischen Batterien, je nach Art der Nutzung.
# Batterieüberwachung
Um die Batterie vernünftig zu managen, muss die Batterie überwacht werden. Dabei werden folgende Zustände bestimmt:
- Ladezustand
- Alterungszustand (Innenwiderstand, Restkapazität)
- Leistungsfähigkeit & Leistungsprognose

Diese Größen können **nicht** direkt gemessen werden, sondern werden mit Hilfe von Modellen aus Messgrößen bestimmt.

Zusätzlich werden Grenzwerte überwacht:
- Temperatur (typisch -10 °C bis 40 °C)
- Spannung
- Maximaler Entladestrom
- Maximaler Ladestrom

# Optimierung des Batteriemanagements
- Volladen erst dann, wenn es notwendig ist -> *Kommunikation mit Kunden, automatische Evaluierung der Nutzungsprofile*
- Nachladung abhängig von aktuellem Ladezustand und absehbarem Bedarf -> *Vermeidung von Zyklisierung über kritische Zustände hinweg*
- Asymmetrische Belastung von Batteriepacks in modularen Systemen unter Kriterium "Maximierung der Gesamtlebensdauer"
	- Wie werden welche Batteriepacks belastet?
	- Wird Leistung oder Energiedichte benötigt?
- Kundenspezifische Ausnutzung der vorhandenen Kapazität -> Kein festgelegter und limitierter SOC-Nutzungsbereich
- On-board-Modelle für Zustandsbestimmung der Batterie z.B. für alterungsminimierendes Laden