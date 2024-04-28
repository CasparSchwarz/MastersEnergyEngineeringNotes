#Brennstoffzelle
# Aufbau eines elektrochemischen Reaktors
![[Pasted image 20240204154137.png]]

## Elektroden
**Anode**: 
- Elektrode an der **Oxidationsreaktion** stattfindet
- nimmt Elektronen auf

**Kathode**:
- Elektrode an der **Reduktionsreaktion** stattfindet
- gibt Elektronen ab

**Pluspol** -> Elektronenüberschuss (Anode)
**Minuspol** -> Elektronenmangel (Kathode)

## Elektrolyt
Ein Elektrolyt ist ein Stoff oder eine Stoffmischung in der sich geladene Atome oder Moleküle frei bewegen können. Aufgabe eines Elektrolyts ist dabei:
- Transport der Ionen von Anode zur Kathode
- Trennung der Elektroden
- Transport von Edukten zur Reaktionsfläche
- Abtransport von Produkten

Ein Elektrolyt muss chemisch Stabil sein.

# Polarisierungsdiagramm
![[Pasted image 20240204154338.png]]
Das Polarisierungsdiagramm beschreibt die Charakteristik einer Brennstoffzelle, wobei die Zellspannung über dem Zellstrom aufgetragen werden. Somit kann die Leistung als Produkt von Spannung und Stromstärke bestimmt werden. Es ist ein Maximum der Leistung zu erkennen.

## Verluste von Brennstoffzellen
![[Pasted image 20240204154527.png]]
**Aktivierungsverluste**: Verluste durch elektrochemische Reaktionen

**Ohm'sche Verluste**: Verluste durch Ionen und Elektronenleitung (Ionenleitung ist in den meisten Fällen deutlich relevanter)

**Verluste durch Stofftransport**: Ab einem bestimmten Punkt können nicht mehr genug Edukte zugeführt oder die Produkte nicht schnell genug abgeführt werden.

# Reaktionskinetik
#Butler-Volmer #Gleichung
Siehe [[Reaktionskinetik]] für Grundlagen

Bei Brennstoffzellen finden Heterogene Reaktionen an der Elektrodenoberfläche statt, welche anstatt der Konzentration mit der Reaktionsdichte $J$ beschrieben werden: $J=\frac{1}{A}\frac{dn}{dt}$

Bei Brennstoffzellen ist der Strom durch die Reaktionsrate gegeben
$j=j_{ox}+j_{red}=z\cdot F\cdot k_{ox}\cdot C_{red}-z\cdot F\cdot k_{red}\cdot C_{ox}$
- $j$ Durchtrittsstromdichte
- $z$ Freie Elektronen pro Reaktion
- $F$ Faraday Konstante
- $k$ Reaktinosgeschwindigkeit

Es entsteht ein dynamisches elektrochemisches Gleichgewicht. Dabei sind Vorwärts- und Rückwärtsreaktion gleich. $j_0$ ist die Austauschstromdichte im dynamischen Gleichgewicht:
$j_0=j_{ox}=-j_{red}$

## Butler-Volmer Gleichung
Die Stromdichte hängt von der Potentialverteilung $\varphi$ ab. Die Reaktionsgeschwindigkeit von Oxidation und Reduktion kann somit durch folgende Gleichungen beschrieben werden:
$j_{ox}=z\cdot F\cdot k_{ox,0}\cdot C_{red}\cdot exp(\frac{\alpha z F}{RT}\Delta\varphi)$
$j_{red}=-z\cdot F\cdot k_{red,0}\cdot C_{ox}\cdot exp(\frac{(1-\alpha) z F}{RT}\Delta\varphi)$
- $\alpha$ Druchtritts- oder Symmetriefaktor oder Ladungstransferkoeffizienz, $0<\alpha<1$
- $\Delta\varphi$ Elektrodenpotenzial

Durch Stromfluss gerät die Elektrode aus dem Gleichgewicht und eine Überspannung $\eta_{act}$ stellt sich ein:
$\eta_{act}=\Delta\varphi-\Delta\varphi_0=\varphi_{Elektrode}-\varphi_{0, Elektrode}$
Somit kann die Stromdichte in einen Gleichgewichts- und Überspannugnsteil aufgeteilt werden:
$j_{ox}=j_0\cdot exp(\frac{\alpha z F}{RT}\eta_{act})$
mit $j_{0}=z\cdot F\cdot k_{ox,0}\cdot C_{red}\cdot exp(\frac{\alpha z F}{RT}\Delta\varphi_0)$

Die #Butler-Volmer Gleichung beschreibt damit die Druchtrittsstromdichte $j$ als Funktion der Überspannung $\eta_{act}$
$j_{ox}=j_0\cdot [exp(\frac{\alpha z F}{RT}\eta_{act})-exp(-\frac{(1-\alpha)zF}{RT}\eta_{act})]$

Die Butler-Volmer Gleichung ist nur für einfache Elektronentransferreaktionen gültig. Dabei muss die Elektronentransferreaktion der geschwindigkeitsbestimmente Schritt in Mehrschrittreaktionen sein.

Es gibt zwei Bereiche der Butler-Volmer Gleichung
- Linearer Bereich bei kleiner Überspannung
- Logarithmischer Bereich wenn Überspannung groß

$\eta_{act}=a+b \ ln \ j$

## Ohm'sche Verluste
In guter Näherung werden die Spannungsverluste auf die Ohm'schen Verluste im ELektrolyt begrenzt:
$R_{elektrolyt}=\frac{L}{A\sigma}$
mit $\sigma$ Leitfähigkeit

Area-specific resistance $ASR=A\cdot R_{elektrolyt}=\frac{L}{\sigma}$
-> $\eta_{ohm}=ASR\cdot j$

## Transportverluste
Die maximale Stromdichte wird durch den maximalen Stofftransport begrenzt. Dabei spielt das Fick'sche Gesetz eine Rolle:
$j=zFD\frac{C_R^0-C_R^*}{\delta}$
mit $D$ Diffusionskoeffizient
$C_R^0$ Ionenkonzentraion im Fluid
$C_R^*$ Ionenkonzentraion an der Elektrode
$\delta$ Dicker der Diffusionsschicht
Bei unendlich schneller Chemie: $C_R^*=0$

Aus Nernst Gleichung -> $\eta_{conc}=c \ ln\frac{j_L}{j_L-j}$
mit $c$ empirische Konstante

# Vereinfachtes Modell einer BSZ
Für ein vereinfachtes Modell werden von dem thermodynamischen Potential aus die Verlustterme subtrahiert:
$V=E_{thermo}-\eta_{act}-\eta_{ohmc}-\eta_{conc}$
Mit Termen oben
$V=E_{thermo}-(a_A+b_A \ ln j)-(a_C+b_C \ ln \ j)- (j \ ASR_{ohmic})-(c \ ln \frac{j_L}{j_L-j})$
![[Pasted image 20240204163244.png]]

Zusätzlich zu den oben genannten Verlusten kommt es in realen System zur Leckage. Diese wird durch einen Leckagestrom $j_{leak}$ beschrieben. Dieser hat jedoch keine Auswirkung auf die ohm'schen Verluste, da nur Ionen des Nutzstroms fließen.
![[Pasted image 20240204163625.png]]
$V=E_{thermo}-(a_A+b_A \ ln(j+j_{leak}))-(a_C+b_C \ ln(j+j_{leak}))- (j \ ASR_{ohmic})-(c \ ln \frac{j_L}{j_L-(j+j_{leak})})$mit $a=-\frac{RT}{\alpha zF}ln \ j_0$, $b=\frac{RT}{\alpha zF}$

# PEM-Brennstoffzelle
#PEM 
Polymermembran-Brennstoffzelle (PEMFC) oder auch Protonenaustauschmemebrand-Brennstoffzelle

- Vorteile
	- Höchste Leistungsdichte aller Brennstoffzellenklassen
	- Gute Start-Stop Eigenschaften
	- Geringe Betriebstemperatur
- Nachteile
	- Teueres Platin wird als Katalysator benötigt
	- Polymermembran teuer
	- Aktives Wassermanagement häufig erforderlich
	- Geringe Toleranz gegenüber CO und S

## Komponenten
- Strömungskanal
	- Konvektier Transport von Edukten zur Gasdiffusionsschicht
	- Konvektiver Abtransport von Produkten an der Gasdiffusionsschicht
- Gasdiffusionsschicht
	- Diffusion von Edukten zur Katalysatorschicht
	- Diffusion von Produkten zum Strömungskanal
	- Leitung von Elektronen
	- Abtransport von flüssigem Wasser
	- Typischerweise aus Karbonfasern mit hydrophober Behandlung hergestellt
- Elektrolytmembran
	- Verwenudung eines Polymers als Elektrolyt
	- Meistverbreitete Polymer ist Nafion
	- Hydrophile Schwefelsäuregruppen ($SO_3^-$) an den Kettenenden führen zur Bildung von Wasserkanälen
	- Ionentransport findet im Wasser statt
	- $H^+$ verbinden sich mit $H_2O$ Molekülen zu $H_3O^+$
	- Wassergehalt im Polymer extrem wichtig für Leitfähigkeit
- Katalysatorschicht
	- Anoden- und Kathodenreaktion finden an Phasengrenzen zwischen der Gasphase, der elektronenleitenden Elektrode und dem ionenleitenden Elektrolyt statt -> Triple-Phase-Boundary
	- Wasserstoff bzw. Sauerstoff müssen in die Katalysatorschicht diffundieren können -> Verwendung von hoch-porösen Materialen
	- Verwendung von Kohlenstoffträgerpartikel die mit Platin Nanopartikeln beschichtet sind

# Weitere Brennstoffzellen
## Protonenaustauschmembran-Brennstoffzelle (PEMFC)
- Vorteile
	- Höchste Leistungsdichte aller Brennstoffzellenklassen
	- Gute Start-Stop Eigenschaften
	- Geringe Betriebstemperatur
- Nachteile
- Teueres Platin wird als Katalysator benötigt
- Polymermembran teuer
- Aktives Wassermanagement häufig erforderlich
- Geringe Toleranz gegenüber CO und S

**Hauptanwendungsgebiet**: Mobilität
## Methanolbrennstoffzelle (MFC)
- Unterkategorie von PEMFC (Direkte und Indirekte Methanolbrennstoffzelle)
- Vorteile
	- Flüssiger Brennstoff (Hohe Energiedichte)
- Nachteile
	- Teures Platin wird als Katalysator benötigt
	- Additionen zum Katalysator nötig, um Vergiftung mit CO zu verhindern
	- Wesentlich geringere Leistungsdichte als $H_2$-PEMFC

**Hauptanwendungsgebiet**: Mobile Stromversorgung (Wenn Energiedichte wichtiger als Effizienz, da Methanol höhere Energiedichte als Wasserstoff)
## Festoxid-Brennstoffzelle (SOFC)
- Vorteil
	- Brennstoffflexibel
	- Keine Edelmetallkatalysatoren
	- Hochwertige Abwärme (800-1000 °C) für KWK
	- Festes Elektrolyt
	- Relativ hohe Leistungsdichte
- Nachteile
	- Hohe Temperaturen nötig
	- Schlechte Ionenleitfähigkeit des Elektrolyts
	- Temperaturverträglichkeit der Materialien
	- Teure Materialien

**Hauptanwendung**: Stationäre Strom- & Wärmeversorgung

## Schmelzkarbonatbrennstoffzelle (MCFC)
- Vorteile
	- Brennstoffflexibel
	- Kein Edelmetallkatalysator
	- Hochwertige Abwärme (~650 °C) für KWK
- Nachteile
	- Geschlossener $CO_2$ Kreislauf benötigt
	- Korrosives, geschmolzenes Elektrolyt
	- Relativ teure Materialien

**Hauptanwendungsgebiet**: Stationäre Strom- & Wärmeversorgung

## Phosphorsäurebrennstoffzelle (PAFC)
- Vorteile
	- Erprobte Technologie
	- Sehr zuverlässig / Lange Laufzeiten
	- Vergleichsweise günstiges Elektrolyt
- Nachteile
	- Platin als Katalysator nötig
	- Geringe Toleranz gegenüber CO und S (jedoch deutlich höher als PEMFC)
	- Elektrolyt ist korrosiv und muss während des Betriebs aufgefüllt werden

**Hauptanwendungsgebiet**: Stationäre Strom (+Wärme) Versorgung

## Alkaline Fuel Cell (AFC)
- Vorteile
	- Geringe Kathodenverluste
	- Edelmetallkatalysatoren nicht unbedingt nötig
	- Geringe Materialkosten / sehr günstiges Elektrolyt
- Nachteile
	- Betrieb nur mit reinem $H_2-O_2$ (Kein $CO_2$ aus der Luft!)
	- Kaliumhydroxid-Elektrolyt muss aufgefüllt werden
	- Wasser muss abgeführt werden

**Hauptanwendungsgebiet**: Raumfahrt / Teilweise wieder aktuelle Forschung, wegen geringen Kathodenverlusten

# Elektrolyseur
#elektrolyse
Die Elektrolyse ist ein Prozess, in dem Moleküle durch elektrischen Strom aufgeteilt werden. Beispielsweise liefert die Elektrolyse von Wasser -> Wasserstoff und Sauerstoff. Der Elektrolyseur ist somit das Gegenstück zur Brennstoffzelle.

## Reversible PEMFC
- Reversible PEMFC können sowohl als Brennstoffzelle als auch als Elektrolyseur betrieben werden
- Vorteile
	- Weiter Betriebsbereich
	- Tolerant gegenüber Strom- und Spannungsschawnkungen
	- Geringe Komplexität
- Nachteile
	- Geringer Wirkungsgrad (40-50 %)

-> Geeignet für die Speicherung von erneuerbarer Energien und Ausgleich von Lastspitzen im Stromnetz

## Festoxid-Elektrolyseur
- Elektrolyt aus fester Oxidkeramik
	- Typischerweise Yttrium-sabilisiertes Zirkonoxid
- Sehr hohe Betriebstemperaturen (500 - 850 °C)
- Sehr hoher Wirkungsgrad (bis zu 90 %)
- Nachteile
	- Lange Aufheizzeit
	- Wenig tolerant gegenüber Lastfluktuationen

-> SOEC geeignet für Dauerbetrieb bei konstanter Last

# Batterien
Eine Batterie ist die Zusammenschaltung von baugleichen galvanischen Zellen.
**Parallelschaltung**: $U_{ges}=U_i$ und $i_{ges}=\sum_i^n i_i$
**Reihenschaltung**: $U_{ges}=\sum_i^n U_i$ und $i_{ges}=i_i$

**Primärzelle**: Energieumwandlung nur in eine Richtung
**Sekundärzelle**: Energieumwandlung in beide Richtung

## SpeicherfähigkeitDelta
Spezifische Ladung einer Batterie: $q_{spez,Bat}=\frac{zF}{\sum_i^n \nu_i'M_i}$
Theoretisch speicherbare Energie: $e_{spez}=q_{spez}\cdot U_{rev}$

## Charakterisierung
- Charakterisierung der Leistungsfähigkeit
	- Polarisationskurven
	- Spannungsabfall während der Entladung
	- Bewertung Leistungsfähigkeit anhand Entladekurve

Entladestrom als C-Rate: $C-Rate=\frac{i_0}{i}$, mit $i_0 = \frac{Nennkapazität}{1 \ h}$

Lade/Entladezyklus von Sekundärbatterien: $\eta_{Speicher}=\frac{E_{Entlade}}{E_{Lade}}$
