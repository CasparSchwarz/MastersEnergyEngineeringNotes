## Bewertung des Wärmepumpenprozesses
Wärmepumpenprozesse werden anhand ihrere Entropieproduktion bewertet. Dabei gibt es verschiedene Ursachen der Entropieproduktion an den verschiedenen Bauteilen einer Wärmepumpe:
- Treibende Temperaturdifferenz an Kondensator und Verdampfer
- Vollständige Dissipation reversibler Arbeit an Expansionsventil
- Reibungsverluste, Wärmeverluste & Strömungswiderstände am Verdichter (größte Verluste)

Exergieverlust: $\Delta\dot{E}_V=T_U\cdot\Delta\dot{S}_{irr}$
Exergetischer Wirkungsgrad: $\xi=\frac{\dot{E}_{ab}}{P_{el}}$

## Herausvorderungen bei Wärmepumpen
- Betriebsgrenzen durch Betriebsbereich des Verdichters festgelegt
- Maximale Prozesstemperatur durch Öl im Verdichter begrenzt
- Überdruck muss gewährleistet sein, da Unterdruck kritisch für die Dichtungen ist
- Maximales Druckverhältnis
- Bereitstellung der notwendigen Wärmeleistung

## Kreislaufvarianten
Wärmepumpen können entweder unterkritisch oder überkritisch betrieben werden:
- unterkritisch
	- Kältemittel bleibt unterhalb des kritischen Punktes
	- sensible und latente Wärme nutzbar
- überkritisch
	- Kältemittel wird außerhalb des kritischen Punktes genutzt
	- nur sensible Wärme nutzbar
	- Sehr hohe Drücke und Temperatur
### Rekuperator
- Erweiterung des Kreislaufes durch internen Wärmeübertrager
- Auslagerung der Überhitzung vom Verdampfer in den internen WÜ -> Bereitstellung notwendiger Überhitzung am Verdichtereintritt + zusätzliche Unterkühlung vorm Expansionsventil
![[Pasted image 20231030145757.png]]
Vorteile:
- Einfache Bauform
- Mäßige Zusatzkosten
- Erhöhung des unteren Druckniveaus
- Hohe Überhitzungen ohne Effizienzverluste
- Mäßige Erhöhung des Nutzwärmestroms
- Höhes Verbesserungspotential bei zeotropen Gemischen
Nachteile:
- IWÜ nciht ohne weiteres regelbar
- Erhöhte Verdichteraustrittstemperaturen
### Einspritzung
- Teilexpansion auf mittleres Druckniveau zum Zustand 4
- Phasentrennung
- Einspritzung des Dampfes in den Verdichter
- Angenähert durch zwei Verdichter
- Zweites Expansionsventil, Phasentrenner und Komplexerer Verdichter benötigt
- Erhöhung des Nutzwärmestroms durch höheren Massenstrom im Kondensator
- Kühlung des Fluidmassenstroms im Verdichter durch Einspritzung
![[Pasted image 20231030150038.png]]
Weitere Variante:
- Dampfeinspritzung mit Wärmeübertrager
	- Dadurch zusätzlicher Freiheitsgrad & erhöhte Steuerbarkeit
	- Erhöhte Kosten und komplexere Regelung
Vorteile:
- Absekung der Verdichteraustrittstemperatur
- Deutliche Erhöhung der Wärmeleistung
- Erhöhung des Betriebsbereichs von Wärmepumpen
- Erhöhte Effizienz aufgrund der reduzierten Verluste in Kondensator & Expansionsventil
Nachteile:
- Deutlich höhere Kosten
- Verdichter mit Einspritzung nicht für alle Kältemittel vorhanden
- Zusätzliche Vibration -> schlechtere Akustik
- Hohe Komplexität -> komplexe Regelung

### Kombination aus Rekuperator und Einspritzung
- Für hohe Leistungen
- Industrieanwendungen
- Hochtemperaturwärmepumpen
- Mehrfamilienhäuser

### Ejektor
- Teilnutzung von Druckenergie nach Kondensator
- Erhöhung des Druckniveaus am Verdichter
- Ejektor ist komplexes Bauteil mit fester Geometrie
- Ejektor und Phasentrenner notwendig
- Angewendet in quasi-stationären Prozessen bei konstantem Betriebspunkt & bei hohen Druckdifferenzen
![[Pasted image 20231030152810.png]]
Funktionsweise Ejektor:
1. Beschleunigung der Massenströme
	- Statischer Druck nimmt ab
	- Geschwindigkeit nimmt zu
2. Mischung beider Ströme
3. Verzögern des Massenstroms führt zu Druckaufbau
Vorteile:
- Hohes Potential für Prozesse mit hohen Druckdifferenzen und quasi-statischen Betrieb
- Vergrößerung des Betriebsbereichs
Nachteile:
- Potential stark betriebspunktabhängig
- Schlechtes Teillastverhalten
- Hohe Komplexität

### Wärmepumpenkaskade
- Kopplungen von zwei oder mehreren Kreisläufen
- Zwischen-WÜ ist Verdampfer und Kondensator zugleich
- Anwendung bei großem Temperaturhub für Hochtemperatur, Tieftemperatur, Ultratieftemperatur
![[Pasted image 20231030153319.png]]
Vorteile:
- Reduktion der maximal Prozesstemperatur
- Optimierung des Fluids der jeweiligen Stufe notwendig
- Sehr hohe Temperaturhübe (>100 K) möglich
- Erhöhte Effizienz durch verbesserten Verdichterbetrieb
Nachteile
- Zusätzliche Bauteile
- Erhöhte Investitionen
- Umfangreichere Regelung