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

# Abschätzung der Batteriegröße
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

