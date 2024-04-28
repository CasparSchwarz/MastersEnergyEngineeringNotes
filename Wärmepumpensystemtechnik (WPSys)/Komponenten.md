## Verdichter
Verdichter im Kältekreis übernehme die Aufgabe der Kompression des Kältemittels. Dabei wird der Druck und die Temperatur des Kältemittels erhöht. Somit kann Wärme bei einem hohen Temperaturniveau abgegeben und bei einem niedrigen Temperaturniveau aufgenommen werden.

Zur Erfüllung der Funktion saugt der Verdichter Kältemittel an und komprimiert dieses im Verdichtungsraum. Der Verdichter wird dabei von einem Elektromotor angetrieben und die beweglichen Teile müssen mit Öl geschmiert werden. Die Hauptaufgaben des Öls sind
- Schmieren
- Kühlen und
- Dichten
Das Öl muss bei ausgeschaltetem Verdichter beheizt werden, damit die rheologischen Eigenschaften beibehalten werden. Das Öl löst sich im Kältemittel und beide bilden eine homogene Phase. Ist die **Löslichkeit** $\omega$ hoch, kommt es zu Leistungsverlusten in den WÜ, bei niedriger Löslichkeit ist der Öltransport problematisch.

### Bauweisen
- Offener Verdichter
	- Externer Antrieb über Welle
	- Trennung von Motor und Kältemittel
	- Bei Korrosionsgefahr bei korrosivem Kältemittel
- Halbhermetischer Verdichter
	- Reparaturen möglich
	- Komponenten austauschbar
	- Motor suaggasgekühlt
	- Öl einfach austauschbar
- Vollhermetischer Verdichter
	- Kompakt, leise und günstig
	- Dicht verschweißt
	- Reparaturen kaum möglich
	- Motor sauggasgekühlt
	- Höhere Endtemperatur

|Verdichtertyp|Funktionsweise|Eigenschaften|Sonstiges|
|--------------|---------------|-----------|-------|
|Hubkolbenverdichter (Verdrängungsverdichter)|Kolben wird vor- und zurückbewegt|Ölschmierung erforderlich aber günstige Fertigung|Sehr breites Leistungsspektrum (Vollhermetisch: 40 W bis 5 kW, Andere: 1 kW bis 80 kW)|
|Scrollverdichter (Verdrängungsverdichter)|Kontinuierliche Verkleinerung des Verdichtungsraums durch kreisende Bewegung exentrisch gelagerter Schnecke|Geringe Reibung und Geräuschemissionen|Breites Leistungsspektrum (300 W bis 50 kW)|
|Rollkolbenverdichter (Verdrängungsverdichter)|Kontinuierliche Verdichtung durch exentrisch gelagerter Kolbenring in kreisförmiger Kammer|Reibungsarm, höchste isentrop Wirkungsgrade, breiter Drehzahlbereich|Für kleine Leistungen (100 W bis 10 kW)|
|Schraubenverdichter (Verdrägngungsverdichter)|Verdichtung durch Profil zwei ineinandergreifender Schrauben. Konvexe Schraube wird angetrieben und konkave Schraube über Getriebe|Reibungsarm, theoretisch ölfrei, höhere Spaltverluste|Für größere Leistungen (30 kW bis 500 kW)|
|Turboverdichter (Dynamischer Verdichter)|Axial- und Radialverdichter verdichten Fluid|Keine Reibung -> Ölfrei, Magnetgelagerte Welle| Für sehr große Leistungen (300 kW bis 1500 kW)|
|Dampfeinspritzung|Einspritzung von Dampf zur Verdichtung|Hohe Verdichtungsendtemperaturen bei reduziertem isentropen Wirkungsgrad|Erweiterung des Kältekreises um Expansionsventil und Gasabscheider|
|Enhanced Vapor Injection (EVI)|Einspritzleistung mittig des Verdichtungsprozesses, Kühlung und Reduktion der Endtemperatur|Höhere elektrische Leistungsuafnahme bei höherer Effizienz|
![[Pasted image 20231106163359.png]]
![[Pasted image 20231106163509.png]]

### Leistungsregelung
Bei dynamischen Lasten muss die bereitgestellte Kühl-/Heizleistung angepasst werden. Dafür können folgende Maßnahmen getroffen werden:
- Zylinderabschaltung (bei offenen / semihermitischen Hubkolben)
- Drehzahlregelung (über Frequenzumrichter)
- Verbundsysteme
	- Erster Verdichter ist drehzahlgeregelt
	- Zweiter Verdichter ist Fixed Speed Verdichter

Zur Regelung des Elektromotors wird ein Frequenzumrichter benötigt. Dieser Wandelt Wechselspannung in eine konstante Gleichspannung und daraufhin in eine modulierte Wechselspannung um den Motor anzusteuern. Frequenzumrichter haben einen Wirkungsgrad von 90 % bis 95 %.

### Bilanzierung
Erster Hauptsatz (stationär): $P_{el}=\frac{\dot{m}}{\eta^{is}_{Verdichter}}\cdot\int v\cdot dp$
Zweiter Hauptsatz (stationär): $0=\dot{m}\cdot(s_1-s_2)+\frac{\dot{Q}}{T_{m,12}}+\Delta\dot{S}_{irr}$
KM: Kältemittel
SF: Sekundärfluid
Erster Hauptsatz: $\dot{Q}=\dot{m}_{KM}\cdot(h_{KM,aus}-h_{KM,ein}=\dot{m}_{SF}\cdot(h_{SF,ein}-h_{SF,aus})$
Zweiter Hauptsatz um KM: $0=\dot{m}_{KM}\cdot(s_{KM,ein}-s_{KM,aus})+\frac{\dot{Q}}{T_{m,KM}}+\Delta\dot{S}_{irr}$
Wobei $\Delta\dot{S}_{irr}=0$ da $dp=0$
Zweiter Hauptsatz um Wand: $\Delta\dot{S}_{irr}=\dot{Q}\cdot(\frac{1}{T_{m,KM}} - \frac{1}{T_{m,SF}})\geq 0$
**Isentroper Wirkungsgrad:** $\eta^{is}_{Verdichter}=\frac{h^{'}_2-h_1}{h_2-h_1}$
**Volumetrischer Wirkungsgrad (Liefergrad)**: $\lambda=\frac{tatsächlicher \ Volumenstrom}{geometrischer \ Volumenstrom}$
### Verlustmechanismen
- Elektrische Verluste
- Strömungsverluste
- Reibungsverluste
- Leckage- / Rückströmungsverluste
- Weitere Verluste
	- Druckpulsationen
	- Aufheizung
	- Ruckexpansion

## Wärmeübertrager
Wärmeübertrager werden als Schnittstelle zwischen Umwelt und Kältekreis eingesetzt. Dabei wird ihnen die Aufbabe zugesprochen, dass Wärme bei niedriger Temperatur und Druck aufgenommen und bei hoher Temperatur und Druck abgegeben werden muss.

Wärmeübertrager können im
- Gleichstrom
- Gegenstrom oder
- Kreuzstrom
ausgeführt werden. Hierbei ist zu beachten, dass beim Phasenwechsel die Temperatur des Fluids, welches den Phasenwechsel durchläuft, (nahezu) konstant ist. Für mehr infos siehe [[WüDe]]

**Bauformen**:
- Lamellenwärmeübertrager
- Plattenwärmeübertrager
- Micro Channel HX
	- Sehr hohes Oberflächen-Volumen-Verhältnis
	- viele kleine Kanäle erhöhen die effektive Wärmeübertragungsfläche
- Doppelrohrwärmeübertrager
- Rohrbündelwärmeübertrager
### Grundlagen des Wärmetransports
- Wärmetransport durch Strahlung: $\dot{Q}_{Stahlung}\sim\alpha_S\cdot\sigma\cdot T^4$
- Wärmetransport durch Leitung: $\dot{Q}_{Leitung}\sim\frac{\lambda}{\delta}\cdot\Delta T$
- Wärmetransport durch Konvektion: $\dot{Q}_{Konvektion}\sim\alpha_K\cdot\Delta T$
#### Grundlagen Wärmeleitung
- Leitung durch Medium (fest/flüssig/gasförmig)
- Treibend dabei ist Temperaturpotential
- Abhängig von
	- Wärmeübertragender Fläche
	- Räumlicher Temperaturgradient
	- Materialeigenschaften
- Fouriersches-Gesetz: $\frac{\dot{Q}_{Leitung}}{A}=\dot{q}^{''}=-\lambda\cdot\frac{dT}{dx}$
#### Grundlagen Konvektion
- Transport innerhalb und zwischen Medien
- Abhängig von:
	- Wärmeübertragender Fläche
	- Räumlicher Temperaturgradient
	- Materialeigenschaften + Strömungseigenschaften
- Natürliche und erzwungene Konvektion
- Nusselt Korrelationen: $\overline{Nu}_L=\frac{\alpha_K\cdot L}{\lambda}=f(Re,Pr,...)=f(Gr,Pr;...)$

**Dominierend sind Konvektion und Wärmeleitung**

### Verdampfer
Im Verdampfer wird Wärme von der Wärmequelle aufgenommen um das Kältemittel zu verdampfen. Dabei können verschiedene Wärmequellen genutzt werden:
- Ab-/ Flusswasser
	- Vorteile Abwasser
		- Dort Verfügbar wo Bedarf an Wärme ist (Urbaner Raum)
		- Kein Eingriff in Ökosystem
	- Herausforderungen:
		- Integration in bestehende Kanalisation
		- Mögliche Beeinflussung von biologischen Prozessen in der Abwasserreinigungsanlage
- Geothermie
- Luft

|Wärmequelle|Temperaturbereich|Einbindung|Einsatz|
|-|-|-|-|
|Ab-/Flusswasser|Flusswasser: 4°C-25°C; Abwasser: 10°C-20°C|Direkt (Wasser wird durch Verdampfer geleitet): Gefahr von Verschmutzung; Indirekt (Einsatz eines Wasserkreislaufs)|Großwärmepumpe|
|Geothermie|Geringe Tiefe: 10°C; Tiefengeothermie > Höhengeothermei|Erdkollektor (Kunststoffrohr), Erdwärmesonde (Koaxialsonden), Zweibrunnensystem (Kontakt mit Grundwasser)|Jede WP|
|Luft|Hohe Temperaturschwankungen (Außentemperatur)|Direkte Nutzung von Luft als Sekundärfluid (Reifbildung möglich)|An Quasi jedem Standort möglich (Garten, Dach, Wand)|
#### Verluste
**Bereifung**
1. Kalte Luft kann weniger Wasserdampf aufnehmen
2. Luftstrom wird abgekühlt
3. Wasser fällt aus und gefriert am Verdampfer -> **Reifbildung**
4. Höherer Wärmewiderstand + Verringerung des Strömungsquerschnitts -> größerer Druckverlust
**Fouling**
1. Unreinheiten in Fluiden oder WÜ fördern Wachstum von Mikro- Makroorganismen
2. Ausbildung von Ablagerungen
3. Zusätzlicher Wärmedurchgangswiderstand
4. Erhöhung des Druckverlustes
Arten von Fouling:
- Partikelfouling
- Korrosionsfouling
- Biofouling
Maßnahmen gegen Fouling:
- Chemikalien
- Änderung der Strömungsformen
- Beschichtung
- Wartung
**Druckverluste**
- Abhängig von Strömungsgeschwindigkeit
- Längen / Durchmesser-Verhältnis
- Rohrreibungskoeffizient
## Expansionsventil
Zu den Hauptaufgaben des Expansionsventils zählt die **Reduktion des Kältemittelsdrucks** auf Saugdruck, **Regelung der Überhitzung** und der **Schutz des Verdichters** vor Flüssigkeitsschlag.

Die Überhitzung wird am Saugstutzen des Verdichters gemessen und mit der Sättigungstemperatur verrechnet. Die Sättigungstemperatur wird über den Druck in der Saugleitung ermittelt.

**Prinzip**:
- $\Delta T_{SH} < \Delta T_{SH,set}$ : Öffnungsgrad runter -> Massenstrom runter -> $\Delta T_{SH}$ hoch
- $\Delta T_{SH} > \Delta T_{SH,set}$ : Öffnungsgrad hoch -> Massenstrom hoch -> $\Delta T_{SH}$ runter

### Bauarten
- Thermostatisches Expansionsventil **TEV**
	- Druck des gasgefüllten Fühlers äquivalent zu gemessener Temperatur
	- Druckausgleich zur Kompensation von Druckverlusten über Verdampfer möglich
	- Träge
	- Öffnungsgrad abhängig von Federdruck und Fühlerdruck
![[Pasted image 20231208141403.png]]
- Elektronisches Expansionsventil **EEV**
	- Schnell und präzise
	- Erfordert Druck- und Temperatursensoren -> teuer
	- Stellmotor und Nadelventil mit über 5ßß Positionen
	- Spezifische Einstellung zum Start der Wärmepumpe
	- Moderne Regelungsverfahren möglich

### Minimale stabile Überhitzung (MSS)
- Flüssigkeitstropfen am Temperaturfühler des Überhitzungsreglers
	- Gemessene Temperatur sinkt schnell
	- Regler reagiert schnell mit Ventilschluss
	- Instabiles Regelverhalten
- MSS-Kennlinie ist Auslegungskriterium und ergibt sich aus Zusammenspiel von E-Ventil und Verdampfer
- Hunting Effekt
	- Abwechselnd große Überhitzung und Überflutung des Verdampfers
	- Mögliche Gründe: Inkorrekte Auslegung von EV oder Verdampfer, falsche Position des Temperatursensors

## Weitere Komponenten
### Sammler
- Funktion
	- Bereitstellung eines Kältemittelpuffers für dynamische Lasten
	- Gasabscheider -> Sicherstellung einer flüssigen Phase vor dem E-Ventil
- Einbau in Flüssigkeitsleitung
- Puffervolumen als Flüssigkeitsabscheider auch in Saugleitung möglich
- Nicht notwendig in Kältekreisen mit statischen Lasten
	- Kühlschränke
	- Tiefkühllung
	- Serverklimatisierung

### Vier-Wege-Umkehrventil
- Funktion
	- Kältekreis umkehren (Verdampfer und Kondensator tauschen Funktion)
	- Abtauung des Verdampfers
	- Kühlung mittels Fußbodenheizung
- Magnetspule bewegt kleinen Schieber
	- Anlegen von Druckpotentialen an großem Schieber
	- Differenzdruck bewegt großen Schieber

### Ölabscheider
- Funktion: Vom Verdichter ausgeworfenes Öl zurückführen
- Einbau hinter Verdichter
- Abscheideeffekt durch Trägheitseffekt
	- Abtropfgitter
	- Filter
	- Strömungsumlenkung
- Abscheidegrad $A=\frac{\dot{m}_{Öl, ab}}{\dot{m}_{Öl, ges}}$

### Trockner
- Funktion
	- Feuchtigkeit absorbieren
	- Säure neutralisieren
	- Feststoffe abscheiden
- Bausweisen
	- Vollhermetisch -> Kompletter Austausch notwendig
	- Halbhermetisch -> Filterkartusche austauschbar
- Einbauort
	- Standardmäßig in Flüssigkeitsleitung
		- Filterung aus der Flüssigphase
		- EV-Schutz
	- Nach Verdichterdefekt in die Saugleitung
		- Säurebildung wird neutralisiert

# Anlagensicherheit
> Ziel von Anlagensicherheit und Störfallvorsorge ist es, Störungen in Anlagen, in denen mit Gefahrstoffen umgegangen wird, zu verhindern. Die Auswirkungen von Störungen, die dennoch eintreten, gilt es für Mensch und Umwelt zu begrenzen.

- Sicheres Design und Installation (Physischer Aufbau verhindert Defekte oder Unfälle)
- Verwendung sicherheitstechnischer Komponenten
	- Bei Unter- oder Überschreitung festgelegter Grenzwerte messtechnisch erfasster Zustandsgrößen werden Anlage oder Komponenten ausgeschaltet
- Infrastruktur
	- Technische Überwachung
	- Zugangsberechtigungen
	- Einzuhaltende Rahmenbedingungen

## Kategorisierung von Zugangsbereichen

| Kategorien | Eigenschaften | Beispiele |
| ---- | ---- | ---- |
| Allgemeiner Zugangsbereich <br>**a** | Keine Schlafeinrichtungen<br>Personen in ihrer Bewegung eingeschränkt<br>unkontrollierte Anzahl von Personen<br>jede Person Zutritt hat | Krankenhäuser, Gerichtsgebäude, Gefängnisse, Theater |
| Überwachter Zugangsbereich<br>**b** | Begrenzte Anzahl von Personen<br>Einige mit Sicherheitsvorkehrungen der Einrichtung vertraut | Büro- oder Geschäftsräume<br>Laboratorien |
| Zugangsbereich, zu dem nur befugte Personen Zutritt haben<br>**c** | Nur Personen, die mit allgemeinen und besonderen Sicherheitsvorkehrungen der Einrichtung vertraut sind | Produktionseinrichtungen für Chemikalien, Nahrungsmittel, Eis, Raffinerien, nicht öffentliche Bereiche in Supermärkten |
## Klassifizierung von Aufstellungsorten
I. **Mechanische Geräte im Personen-Aufenthaltsbereich**
- Sofern die Kälteanlage oder die kältemittelführenden Teile sich im Personen-Aufenthaltsbereich befindet / befinden

II. **Verdichter im Maschinenraum oder im Freien**
- Sofern sich alle Verdichter und Druckbehälter im Maschinenraum oder im Freien befinden (gilt nicht für Rohrschlangen und Rohrleitungen)

III. **Maschinenraum oder im Freien**
- Sofern sich alle kältemittelführenden Teile in einem Maschinenraum oder im Freien befinden
- Maschinenraum nach EN 378-3

IV. **Belüftetes Gehäuse**
- Sofern sich alle kältemittelführenden Teile in einem belüfteten Gehäuse befinden
- Gehäuse nach EN 378-2 und EN 378-3

## Begrenzung von Füllmengen
- LFL - untere Explosionsgrenze
**LFL_R32 = 0,307 kg/m³**
**LFL_R290 = 0,038 kg/m³**
- Wandmontage: 1,8
- Fenstermontage: 1
- Deckenmontage: 2,2

$m_{max}=2,5\cdot LFL^{5/4}\cdot h_0\cdot A^{1/2}$
mit:
- $LFL$ Unterer Explosionsgrenze
- $h_0$ Höhenfaktor
- $A$ Raumfläche

Für R32
![[Pasted image 20240130171403.png]]

Für R290:
![[Pasted image 20240130171429.png]]

## Maximal zulässiger Druck
- Maximal zulässig
	- Sättigungsdruck bei Konstruktionstemperaturen der Tabelle
	- Für einzelne Komponenten, Abschnitte sowie Gesamtanlage
	- Sicherheitschalteinrichtung lösen bei <= 1 * PS aus
- Kategorisierung nach Übereinstimmung mit PED
	- Kategorie < I -> Keine Konformitätserklärung erforderlich
	- Kategorie = I -> Konformitätserklärung nach PED erforderlich
	- Kategorie >= II -> Konformitätserklärung nach PED und / oder weiteren Richtlinien erforderlich

![[Pasted image 20240130171854.png]]


## Typische Fehler und Ursachen in Kältekreisen
- Kondensator:
	- Pumpenausfall der Sekundärseite
	- -> Hochdruckstörung
- Verdichter:
	- Beschädigung durch Flüssigkeit
	- -> Ineffiziente Verdichtung oder vollständiger Ausfall des Verdichters
	- -> Beschädigung weiterer Komponenten durch Verunreinigungen oder Säurebildung
- Verdampfer:
	- Lüfterausfall oder Verlaubung
	- -> Niederdruckstörung
- Expansionsventil:
	- Beschädigung durch Gasblasen
	- -> Regelung der Überhitzung nicht möglich
	- -> Beschädigung des Verdichters