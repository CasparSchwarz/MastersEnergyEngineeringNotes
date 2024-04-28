## Wärmeintegration
Bei der Energieumwandlung entsteht Abwärme. Diese Abwärme gilt es zu nutzen und nennt sich "Wärmerückgewinnung" (WRG).
Beispiel: Rekuperative Verbrennungsluft-Vorwärmung
- Verbrennung von Brennstoff in Gastherme
- Wärme wird nicht vollständig an Wasser abgegeben (vorgegebene Vorlauftemperatur)
- Hinter Gas/Wasser-WÜ kommt Luft/Abgas-WÜ um Zuluft vorzuwärmen

**Brennwertkessel**
Bei einem Brennwertkessel wird die Verdampfungsenthalpie des Wasserdampfes im Abgas genutzt um die Zuluft vorzuwärmen. Problem: Flüssiges Wasser wirkt korrosiv auf den Kessel, da Schadstoffe (Schwefel) im Wasser gelöst sind.

### Wärmeübertrager
Pinch Methode:
1. Bilde die Summenkurven
2. Schiebe die Summenkurven so weit aneinander übereinander
3. bis zur minimalen Temperaturdifferenz,
4. woebi oberhalb des Pinch nur geheizt und unterhalb des Pinch nur gekühlt werden darf

**Drei wichtige Regeln:**
- Nicht unterhalb des PINCH heizen
- Keine Wärme über PINCH übertragen
- Nicht oberhalb des PINCH kühlen

Die Temperatur kann in Abhängigkeit des Enthalpiestroms dargestellt werden:
$T_{i,a}=T_{i,e}+\frac{\Delta H_i}{\dot{m}_ic_{p,i}}$
Somit entstehen Geraden im $T-\dot{H}$ - Diagramm.

### Leitfaden zur Berechnung
1. Stromdiagramm zeichnen
![[Pasted image 20240108145437.png]]
2. Wärmekaskade in Tabelle berechnen
	1. Intervalle definieren (siehe Abbildung)
	2. Ein- und Ausganstemperatur für jeweiliges Interval bestimmen
	3. Temperaturdifferenz über Interval berechnen
	4. Summe der Wärmekapazitätsströme pro Interval berechnen $\sum \dot{m}c_p$
	5. Wärmeströme berechnen $\dot{Q}_i=(\dot{m}c_p)_i\cdot\Delta T$
	6. Wärmestromänderung berechnen: $\Delta\dot{Q}_i=\dot{Q}_i+\Delta\dot{Q}_{i-1}$ mit $\Delta\dot{Q}_0 = 0$
	7. Wärmestromänderungen um maximale Änderung verschieben: $\Delta\dot{Q}^*_i=-\max{\Delta\dot{Q}_i}+\dot{Q}_i$
3. Temperatur über $-\Delta\dot{Q}^*_i$ in Diagramm eintragen
-> $\dot{Q}_{H,min}=\max{\Delta\dot{Q}_i}$; $\dot{Q}_{K,min}=\Delta\dot{Q}^*_{i=n}$

### Wärmeübertragernetzwerke
Zur Auslegung von Netzwerken zur Wärmeintegration ist die Wirtschaftlichkeit sehr wichtig. Dazu muss die kostenoptimale, minimale Temperaturdifferenz ermittelt werden. Dabei setzten sich die Gesamtkosten aus den Betriebskosten und den Kapitalkosten zusammen.

>Besser **wenige große** als viele kleinen Wärmeübertrager!

### Euler-Theorem
Das Euler-Theorem in der Graphentheorie beschäftigt sich mit der Problemstellung, so viele Punkte mit so wenig Strecken wie möglich zu verbinden. Dadurch ergibt sich eine obere Grenze für die minimale Anzahl an Wärmeübertragern für ein vollständig wärmeintegriertes Netzwerk (MER = maximum energy revocery). Dabei wird das theorem einmal unter dem Pinch und einmal ober dem Pinch angewendet.

$N_{min,MER}\leq (N_{heiß}+N_{kalt}+N_{Betriebsmittel}-1)_{oberhalb \ Pinch}+(N_{heiß}+N_{kalt}+N_{Betriebsmittel}-1)_{unterhalb \ Pinch})$
![[Pasted image 20231116093501.png]]

### Wärmepumpeneinsatz
Einsatz einer Wärmepumpe:
- Wärme von niedrigen Temperaturniveau auf hohes Temperaturniveau
- Um Pinch herum
- Benötigt elektrische Leistung

## Organic Rankine Cycles
Historische Betrachtung einer Wärmekraftmaschine:
- Wärmezufuhr bei hohem Temperaturniveau
- Wärmeabfuhr bei niedrigem Temperaturniveau
- Abfuhr von technischer Leistung

Ein Organic Rankine Cycle (ORC) kann unterhalb des Pinch integriert werden. Im klassischen Fall wird als Arbeitsfluid Wasser verwendet. Beim ORC werden **organische Arbeitsfluide** verwendet, da bei diesen die Siedetemperatur deutlich unter der von Wasser liegt. Damit kann auch bei einem niedrigen Temperaturniveau Leistung über einen Rankine-Prozess entnommen werden.

ORC können genutzt werden um aus Wärme bei einem niedrigen Temperaturniveau technische Leistung zu erzeugen. Dabei ist die Leistungsausbeute jedoch relativ gering.

## Fortwärmewirtschaft
In der Fortwärmewirtschaft geht es um die Nutzung von An- oder Fortwärme außerhalb des Prozesses, in dem die Wärme anfällt. Ein Beispiel dafür sind Fernwärmenetze, in denen Abwärme von Industrie oder Energieerzeugung genutzt wird um Wohnräume zu heizen.

### Bewertung der Abwärmenutzung
1. Abschätzung des Potenzials von **Abwärmequellen**
	- Temperaturniveau
	- verfügbare Abwärmeleistung bzw. Energiemenge
	- Medium der Abwärme
	- Verschmutzung des Abwärmemediums
	- zeitliche Verfügbarkeit
2. Bewertung der Nutzungsmöglichkeiten
	- Temperatur Wärmequelle > Temperatur Wärmesenke?
	- Leistung der Wärmequelle >= Wärmesenke
	- Verschmutzungsgrad Wärmequelle tolerierbar
	- Gleichzeitigkeit Verfügbarkeit Abwärme und Bedarf Wärmesenke?
	- räumliche Entfernung Quelle-Senke?
	- Bauraum verfügbar?
	- Genehmigungen notwendig?
3. Bewertung der Wirtschaftlichkeit

## Deman-Side Management (DSM)
**Ziel**: Beeinflussung von Niveau und zeitlichem Verlauf der Nachfrage nach Arbeit und Leistung
- hauptsächlich für Strom, aber zunehmend andere Betriebsmittel (z.B. Gas, Wasser)
- effizienzsteigernde Maßnahmen
- Lastmanagement für Energieversorger
- Umsetzung beim Kunden durch Aufklärung und finanzielle Anreize
![[Pasted image 20231214132410.png]]