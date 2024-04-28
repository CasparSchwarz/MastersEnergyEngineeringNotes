Das **V-Modell** ist eine oft angewendete Methode zur Entwicklung von Anlagen, Maschinen, Programme und mehr. Im V-Modell werden drei Prozessschritte definiert:
1. Entwicklung
2. Realisierung
3. Validierung
Un jedem Schritt der Validierung muss auf den entsprechenden Schritt der Entwicklung zurückgeschaut werden, um zu prüfen ob das finale Produkt den Anforderungen entspricht.
![[Pasted image 20231223095005.png]]

# Lastannahmen
Belastungsfälle:
- Produktionsbetrieb (Start, Nennbetrieb, Stillsetzen der Anlage)
- Sicherheitsrelevante Lastfälle (Notstopp, Fehler)
- Extremlastfälle (Böen, Turbulenzen)
- Montage, Transport, Wartung

Es gibt genormte Deisgn Load Cases:
- IEC 61400
	- Internationale Norm als Basis für Zertifizierung
	- Wesentliche Auslegungsanforderungen zur Sicherstellung der technischen Integrität einer WEA
	- Liefert keine vollständige Entwurfsgrundlage oder Bedienungsanleitung
- GL Wind (Germanischer Lloyd Wind, Zertifizierungsstelle für WEA)
	- Weitergehende Richtlinien mit Fokus auf der Auslegung der Bauteile
- DIBt (Deutsches Institut für Bautechnik)
	- Richtlinien für Turm und Fundament

Die Auslegung einer WEA erfolgt nach vorgegebene nAuslegungslastfällen:
- DLC1
	- Normaler Produktionsbetrieb
- DLC 2
	- Normaler Produktionsbetrieb und Fehler
- DLC 3
	- Start
- DLC 4
	- Normale Abschaltung
- DLC 5
	- Notabschaltung
- DLC 6
	- Parken
- DLC 7
	- Parken und Fehler
- DLC 8
	- Wartung / Reparatur
	- Transport
	- Montage

## Windannahmen
Nach IEC 61400:
- WEA Klassen III, II, I
- Klasse I hat höhere Windgeschwindigkeiten als III
- Klasse S ist Wildcard -> Werte werden von Hersteller angegeben
Nach DIBt:
- Deutschland ist in Zonen aufgeteilt
- Zone 4 mit höchsten Windgeschwindigkeiten
- Zone 1 mit niedrigsten Windgeschwindigkeiten
**Windzonen nach DIBt sind entgegengesetzt zu IEC 61400 definiert**

# Lastenrechnung
Die Lastenrechnung geschieht heutzutage maschinell über FEM oder Mehrkörpersimulation. Dabei müssen die Schnittgrößen berechnet werden um die Lasten innerhalb der Bauteile zu bestimmen.

## Simulation
In der Simulaion müssen verschiedene elastische Elemente miteinander gekoppelt werden. Dies geschieht in der Mehrkörpersimulation. Ein einzelnen Körper kann über die Finite-Elemente-Methode simuliert werden. Jedoch hat die FEM einen hohen Rechenaufwand zur Folge, weshalb das FE-Modell auf wenige diskrete Kraftangriffspunkte reduziert wird, damit das Gesamtsystem mit akzeptablen Rechenaufwand betrachtet werden kann.

# Systemprüfung
Zur Systemprüfung müssen Prüftstände errichtet werden. An diesen Prüfständen werden die Lastaufnehmenden Bauteile einer WEA geprüft. Dafür müssen die Prüfstände Lasten bei Nennleistung bereitstellen, weshalb mit jeder neuen Generation von WEA auch neue Prüfstände errichtet werden müssen.

![[Pasted image 20231223101023.png]]

# Komponentenprüng
## Kaltes Klima
- Voraussetzung
	- WEA mus bei geringen Temperaturen von -40 °C anfahren können
	- Schmierstoffversorgung der Lager und Verzahnungen msus gegeben sein
	-> Entwicklung spezieller Anfahrprozeduren nötig
- Klimakammer
	- Durchführung von Versuchen mit Fokus auf die Anfahrmomente
- Hauptgetriebe
	- Typischer Schmierstoff hat eine Viskosität von ISO VG 320
- Besonderheiten
	- Trudeln und Stromprudktion erfolgt erst bei erhöhten Getriebe- bzw. Öltemperaturen
	- Heizpatronen im Öl
	- Pumpbarkeit

## Getriebeprüfstände
**Elektrisch geschlossener Kreis**
- Rückgewinnung der Bremsleistung über zusätzlichen Generator
- Kopplung von Antrieb und Abtrieb im DC-Zwischenkreis
- Nur die Verlustleistungen in den Komponenten müssen vom Netz eingespeist werden
-> für Getriebe in großen Leistungsklassen ökonomisch
- Nur geringe Leistung des netzseitigen Umrichters erforderlich
![[Pasted image 20240226144734.png]]

**Back-to-Back Getriebeverspannungsprüfstand**
- Elektrischer Verspannungsprüfstand
- Zwei Getriebe in reziproker Anordnung
- Geringe Rüstzeiten, da in einem Aufbau zwei Getriebe geprüft werden können
- Horizontale Anordnung entspricht nicht der realen Einbaulage von 5°-6°
- Im HIlfsgetriebe ist zwar die korrekte Zahnflanke im Eingriff, die Drehrichtung ist jedoch verkehrt
![[Pasted image 20240226144801.png]]

**Mechanisch geschlossener Kreis**
- Mechanische Rückführung der Antriebsleistung
-> aufgrund des typischen Aufbaus von WEA Getrieben schwierig zu realisieren
- Nur die Verlustleistungen in den in den Komponenten müssen vom Netz eingespeist werden
-> für Getriebe in großen Leistungsklassen ökonomisch
- Nur geringe Leistung des netzseitigen Umrichters erforderlich
![[Pasted image 20240226144834.png]]

# Zertifizierung
- Komponentenzertifikat
	- Gilt jeweils für eine Hauptkomponente einer WEA
- Typenzertifikat
	- WEA einschließlich Turm und Fundament und der Verbindung zwischen Turm und Fundament
- Prototypzertifikat
	- Gilt für WEA, die noch nicht zur Serienproduktion bereit ist
	- Ist nur für eine beschränkte Dauer gültig
- Projektzertifikat
	- Eine oder mehrere WEA einschließlich Fundamenten und weitere Installationen am Standort mit Standortbewertung und Fundamentenkonstruktionsbewertung