Ein Regler sorgt für die Rückführung der Regelabweichung auf die Stellgröße und erzeugt einen geschlossenen Wirkungsablauf; den Regelkreis. In einem Kältekreis ist die Aufgabe des Reglers die Regelung der Vorlauftemperatur. Dabei ist die 
- Vorlauftemperatur die Führungsgröße,
- die Verdichterdrehzahl die Stellgröße und
- die Rücklauftemperatur eine der Störgrößen.
Zusätzlich muss die Überhitzung des Kältemittels am Verdichtereingang durch die Stellung des Expansionsventils geregelt werden.

Der Unterschied einer Steuerung zu einer Regelung ist der, dass bei einer Steuerung der funktionale Zusammenhang der Störgrößen auf die Regelgröße bekannt sein muss.

![[Pasted image 20231208144515.png]]


**Begriffsdefinitionen**:
- W: Führungsgröße (Soll-Wert)
	- Gewünschte / vorgegebene Temperatur
- X: Regelgröße (Ist-Wert)
	- Gemessene Raumtemperatur
- Y: Stellgröße
	- Heizungsventilstellung
- Z_1, Z_2: Störgrößen
	- Äußere Einflüsse, wie Sonne und geöffnete Fenster
- Regler: Mensch - Stell-Ventil

## Anwendung in der Praxis
- Regelstrecke für Vorlauftemperatur Komplex
	- Viele Eingangsgrößen
	- Viele Nichtlinearitäten
- Integration Regelung
	- Rückführen der Regelgröße
- PI-Regler typisch zur Verdichterregelung
- Sollwertermittlung häufig durch Heizkurve
![[Pasted image 20231208145506.png]]

- Regelung der Vorlauftemperatur durch On/Off Betrieb (kein Inverter)
	- Vorteile: Günstig
	- Nachteile
		- Regelung nur durch unstetige Regler (2-Punkt-Regler)
		- Häufiges Takten bei Teillast
- Regelung der Vorlauftemperatur durch Drehzahlregelung
	- Vorteile
		- Präzise Regelung der Temperatur durch stetige Regler
		- Wenige Startvorgänge -> Erhöhung Lebensdauer
	- Nachteile
		- Kosten
		- Zusätzliche Verluste
- Regelung der Sollvorlauftemperatur durch Systemregler
	- In Abhängigkeit von Außentemperatur -> Heizkurve
	- Prädiktiv durch MPC
