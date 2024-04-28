Für die Modellierung von Windkraftanlagen werden die Annahmen nach der Theorie von Betz getroffen:
- eindimensional
- stationär
- inkompressibel
- keine WÄrmeströme
- reibungsfreie Strömung ohne Verluste
- der Rotor befindet sich in einer einzelnen Ebene
- Kein Einfluss der Rotation
- Kein Einfluss der Blattanzahl

## Physikalische Grundlagen
- Kinetische Energie: $E=0,5\cdot mv^2$
- Volumenstrom: $\dot{V}=v\cdot A$
- Massenstrom: $\dot{m}=\rho\cdot v \cdot A$
- Gesamtleistung: $P=\frac{1}{2}\rho v^3A$
- Mechanische Leistung: $P_{mech}=P_1-P_2$
-> $P=\frac{1}{2}\dot{m}(v_1^2-v_2^2)$

- Kraft auf die Turbine: $F=\dot{m}(v_1-v_2)$
- Leistung: $P=Fv^{'}$
- Geschwindigkeit in der Rotorebene: $v^{'}=\frac{1}{2}(v_1+v_2)$
- Massenstrom: $\dot{m}=\rho Av^{'}$
- Mechanische Leistung: $P=\frac{1}{4}\rho A(v_1^2-v_2^2)(v_1+v_2)$
- Gesamtleistung: $P_0=\frac{1}{2}\rho v_1^3A$
- Leistungsbeiwert $c_p = \frac{P}{P_0}=\frac{1}{2}[1-(\frac{v_2}{v_1})^2](1+\frac{v_2}{v_1})$
Der optimale Leistungsbeiwert liegt bei 16/27=0,59. Dadurch ergibt sich ein $v^{'}=\frac{2}{3}v_1$ und $v_2=\frac{1}{3}v_1$.
![[Pasted image 20231111143212.png]]

- tip speed ration: $\lambda=\frac{u}{v_W}=\frac{Umfangsgeschwindigkeit}{Windgeschwindigkeit}$

Es existieren zwei verschiedene Arten Windenergie in mechanische Energie umzuwandeln:
- Widerstandsnutzende Windenergiewandler
- Auftribsnutzende Windenergiewandler
Wie wiederstandsnutzenden erreichen jedoch nur ein $c_{P,max}=0,2$. Auftriebsnutzende Windenergiewandler erreichen höhere Werte für c_p.

Im Gegensatz zur Betzschen Theorie verhält sich die reale Welt jedoch anders:
- Die Luft erhält eine drehende Bewegung
- Drei räumliche Dimensionen
- Drehimpulserhaltung
- Rotationsenergie reduziert den nutzbaren Anteil der Gesamtenergie im Luftstrom
- Der Leistungsbeiwert wird kleiner als in der Betz-Theorie
- Der Leistungsbeiwert wird abhängig vom Verhältnis der tip speed ratio

Zur Annäherung der realen Verhältnisse existiert die **Blattelementtheorie**:
- Blattelemente im Abstand r von der Achse
- Vereinfachung: kein Einfluss der Elemente untereinander
- örtliche Rotorblatttiefe, radiale Erstreckung
- lokaler Anstellwinkel
- axiale Geschwindigkeit + Rotationsgeschwindigkeit = resultierende Anstellgeschwindigkeit
- Luftkraftbeiwerte aus Profilpolaren
Daraus folgt:
- Tangentialkräfte über Blattlänge
- Normalkräfte entlang der Blattlänge
Anströmgeschwindigkeit: $V_{res}=\sqrt{(\Omega\cdot r)^2+{V^{'}}^2}$
Kräfte am Element (für große Schnelllaufzahl):
- Auftrieb: $dA = \frac{1}{2}\rho V^2_{res}\cdot c_a\cdot l\cdot dr$
- Widerstand: $dW=\frac{1}{2}\rho V^2_{res}\cdot c_w\cdot l\cdot dr$
- Schub: $dF = dA\cdot cos\varphi + dW\cdot sin\varphi$
- Querkraft: $dQ = dA\cdot sin\varphi - dW\cdot cos\varphi$

## Rotornachlaufströmung
In Windparks stehen WKAs sehr nahe beieinander. Die WKAs beeinflussen sich gegenseitig durch den Nachlauf, wobei die Windgeschwindigkeit im Nachlauf vermindert ist und somit auch die Energieausbeute verringert wird. Zudem kommt es im Nachlauf zu höherer Turbulenz, welche die dynamischen Lasten erhöht.
- Nahbereich
	- Druckausgleich
	- Wirbelschleppen
	- Minimale Geschwindigkeit bei ca. 1 - 2 D
- Übergangsbereich
	- Erzeugung von Turbulenz in der Grenzschicht
	- Vermischung mit der Umgebung
	- Wirbel verschwinden weitgehend
- Fernfeld
	- Gauß-Verteilung der Geschwindigkeit
	- Mischung mit der Umgebung
	- hängt von der Tu-Intensität der Umgebung ab
![[Pasted image 20231111150942.png]]

## Leistungscharakteristik des Rotors
- Leistungsbeiwert wird für bestimmte Schnelllaufzahl berechnet
- Für mehrere Schnelllaufzahlen ergibt sich Kennlinie
$P_R=c_{PR}\frac{1}{2}\rho v^3_WA$
$M_R=c_{MR}\frac{1}{2}\rho v^2_WAR$
$c_{PR}=\lambda c_{MR}$
- Historsiche Rotoren mit Widerstand: c_PR = 0,2 .. 0,3
- Auftriebsnutzende Schnellläufer: c_PR bis 0,5
- Langsamläufer mit vielen Blättern haben ein hohes Moment

Bei Zunahme der Rotorblattanzahl steigt auch die Leistung. Dabei nimmt der Leistungszuwachs mit steigender Rotorblattanzahl ab. Demnach wird eine geringere Anzahl an Rotorblättern bevorzugt, um Mehrkosten durch weitere Rotorblätter zu vermeiden.

Optimale Form der Rotorblätter:
![[Pasted image 20231111153342.png]]
- Ideale Form ist hyperbolisch -> schwer zu fertigen
- Einfachere Formen sind linear und preiswert

Der Außenbereich der Rotorblätter ist aufgrund der hohen Geschwindigkeiten sehr wichtig:
- Profile müssen sorgfältig gewählt werden
- gute Oberflächenqualität ist nötig
- genaue Tiefenverteilung
Optimale Form des Blattumrisses:
- Gerade Hinterkante hält aerodynamisches Moment stabil -> günstiges Regelverhalten
- Spitzer Randbogen und Endplatten sind günstig für Geräuschemission
- Winglets beeinflussen Randwirbel -> Verringerung des Luftwiderstandes bei hohen Anstellwinkeln

### Profilgeometrie und Systematik
![[Pasted image 20231214134230.png]]
**4-ziffrige NACA-Profile**
1. maximale Wölbung f in %
2. Wölbungsrücklage xf in Zehnteln
3. größte Profildicke d
- Bsp.: NACA 4412:
	- 4 % Wölbung bei 40 % Profiltiefe
	- 12 % maximale Dicke

**5-ziffrige NACA-Profile**
1. Maß für Wölbungshöhe x 15 = Auftriebsbeiwert
2. doppelte Wölbungsrücklage
3. Form der Skelettlinie (0 ohne, 1 mit Wendepunkt)
4. Dicke in Prozent (4 und 5)
- Bsp.: NACA 23018
	- c_I = 0,3
	- maximale Wölbung bei 15 %
	- maximale Dicke 18 %

#### Laminarprofile
- 2 Regionen im Strömungsfeld
- Grenzschicht
	- Viskosität
	- Haftbedingung
	- Wandrauigkeit
	- Grenzschichttheorie von Prandtl
- äußeres Strömungsfeld
	- reibungsfrei
	- Potentialtheorie
- 2 Anteile des Widerstandes
	- Schubspannungen, Reibungen
	- Druck

Zur Grenzschicht:
- laminar am Anfang
- je nach Re-Zahl und Rauigkeit: Transition, Turbulenz, Wirbel, Mischung, Querbewegung
- Grenzschichtdicke wächst, löst ab
- veränderte Druckverteilung -> Druckwiderstand
- Turbulenz erhöht den Reibungswiderstand, stabilisiert aber die Grenzschicht
- Verschiebung der dicksten Stelle nach hinten -> Verzögerung ist später
- Strömung bleibt bis 60 % laminar

#### Verwindung der Rotorblätter
- Verwindung ist notwendig, da Strömungsbedingungen in der Wurzelregion völlig anders sind als an der Spitze
- Größere Umfangsgeschwindigkeit -> veränderter Anstellwinkel, effektive Anströmgeschwindigkeit
- Verwindungswinkel zwischen Sehen bei 70 % Radius
- Berechnung des Torsionswinkels geht nur für einen Betriebpunkt

#### Blattdicke
- Klassischer Konflikt zwischen Aerodynamik und Festigkeit
- Aedynamiker möchte dünne Rotorblätter mit hoher Leistung
- Strukturauslegung verlagnt nach ausreichenden Querschnitten
-> Optimierung der Kosten

### Auslegungsschnelllaufzahl
- hohe Schnelllaufzahl -> schlanke Blätter -> Steifigkeitsprobleme -> teure Materialien
- der maximale Leistungskoeffizeint hängt fast nicht von der Auslegungsschnelllaufzahl ab
- heutzutage: Geräuschentwicklung ist wichtiger -> eher niedrige Schnelllaufzahlen
- Typische Werte: 9-10 für 2 Blätter, 7-8 für 3 Blätter

### Aerodynamische Leistungskontrolle
- Anstellwinkel veröndern
- Verkleinern der Rotorangriffsfläche (aus dem Wind drehen)
- Veränderung der effektiven Anströmgeschwindigkeit
-> Variation der Drehzahl
- Regelung mit der Drehzahl ist nur begrenzt möglich (50 Hz)

#### Blatteinstellwinkelregelung
- mechanische Verstellung des Einstellwinkels it effektivste Methode
- Prinzipiell 2 Möglichekiten
	- Verringerung des aerodynamischen Anstellwinkels zur Reduzierung der Leistung
	- Vergrößerung des Anstellwinkels über den kritischen Winkel führt zur Strömungsablösung
- Stall geht auf kürzerem Weg