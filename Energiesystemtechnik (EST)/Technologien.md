# Wärmepumpen
[Wärmepumpen](WPSys) sind Maschinen, die Wärme von einem niedrigen auf ein hohes Temperaturniveau transportieren. Dabei wird
1. Bei niedriger Temperatur Kältemittel verdampft,
2. Das Kältemittel verdichtet,
3. Bei hoher Temperatur das Kältemittel kondensiert und
4. über ein Drosselventil entspannt.

Für genauere Informationen siehe [[WPSys]]

- Wärmepumpen sind häufigste Wärmeerzeuger in Neubauten und Sanierungen
- WP sind notwendig um die Klimaziele zu erreichen (80 % CO2-Einsparung bis 2050)

## Betriebsweisen
Wärmepumpen können auf verschiedene Arten betrieben werden ([[Anwendungen von Wärmepumpen#Bivalente Systeme]]):
- monovalent
- bivalent
- monoenergetisch
Im bivalenten Betrieb wird die Wärmepumpe durch einen zweiten Wärmeerzeuger unterstützt (Gaskessel, Widerstandsheizung). Dabei wird unterschieden zwischen:
- bivalent-alternativ
	- Über einer bestimmten Temperatur wird nur WP verwendet
	- Unter der Temperatur wird nur der sekundäre Wärmeerzeuger verwendet
- bivalent-teilparallel
	- Ab einer bestimmten Temperatur werden beide Erzeuger gleichzeitig genutzt
	- Ab einer tieferen Temperatur wird nur Sekundärerzeuger genutzt
- bivalent-parallel
	- Ab einer bestimmten Temperatur werden beide Erzeuger gleichzeitig genutzt

## Bewertung von Wärmepumpen
siehe [[Anwendungen von Wärmepumpen#Bewertung von Wärmepumpen]]
- Jahresarbeitszahl: $\beta=\frac{Q_N}{W_{el}}=\frac{\int\dot{Q}_Nd\tau}{\int P_{el}d\tau}=\frac{\int md\tau}{\int\frac{m}{\varepsilon(\tau)}}$
	- Belastungsgrad $m=\frac{\dot{Q}_N}{\dot{Q}_{Norm}}$
- [[Anwendungen von Wärmepumpen#Mögliche Systemgrenzen]]

Nach Norm wird ein SCOP bestimmt, welcher die Leistungszahl bei verschiedenen Lastszenarien abbildet. Zudem beinhaltet der SCOP auch die anderen Verbraucher im Gesamtsystem der Wärmepumpe.

## Kältemittel
- Notwendig für den Betrieb von Wärmepumpen
- Kältemittel sind oft umstritten und müssen verschiedenen Vorgaben gerecht werden
	- Politische Vorgaben
	- Technische Vorgaben
	- Für Kreisprozesse geeignete Vorgaben

# Thermische & Offene WP und Kältemaschinen
**Klassifizierung von Wärmepumpen**
![[Pasted image 20231222135621.png]]

## Absorptionskältemaschine
![[Pasted image 20231222135722.png]]
Absorptionskältemaschine nutzen als treibende Kraft nicht mechanische Arbeit sondern Wärme. Dabei wird über einen Absorber und Austreiber das Kältemittel thermisch verdichtet.

Absorptionskältemaschinen ermöglichen die Erzeugung von Kälte aus Wärme

Das Wärmeverhältnis $\beta_0$ beschreibt das Verhältnis von Kühlleistung zu zugeführter Wärmeleistung. Dabei ist:
$\beta_0=\frac{Q_0}{Q_{zu}}$

## Gasmotor-WP und Elektromotor-WP
![[Pasted image 20231222135436.png]]
Gasmotor-WP können Abwärme nutzen um die Wärme auf ein höheres Temperaturniveau zu bringen. Damit wird ebenso ein höherer Verbundwirkungsgrad erzielt.

# KWK
Unter Kraft-Wärme-Kopplung (KWK) wird die Abwärmenutzung von Stromerzeugenden Maschinen verstanden. Dabei kann der Ausnutzungsgrad von Maschinen deutlich erhöht werden.

|  | Dampfkraftwerk | Gasturbine | GuD | MHKW |
| ---- | ---- | ---- | ---- | ---- |
| Anlaufdauer | Langsam | Schnell | Langsam | sehr schnell |
| Teillast | Gut | Schlecht | Gut | Gut |
| Investition | 450-1250 | 850-1150 | 500-900 | 500-2000 |
| Personal | 8-20 | 0,5-5 | 5-20 | 0,5-5 |
| Wartung | 2-3 | 1,5-2 | 3,25 | 8-10 |
| Platzbedarf | 70-120 | 10-30 | 30-50 | 50-120 |
Brennstoffausnutzungsgrad: $\omega=\frac{P_{el}+\dot{Q}_H}{\dot{m}_BH_u}=\eta_{el}+\alpha$
Stromkennzahl: $\sigma=\frac{P_{el}}{\dot{Q}_H}$
## KWK mit Dampfturbinen
Gegendruckschaltung:
- Wärmeverbraucher sitzt direkt hinter der Dampfturbine
- Leistungsverlust durch Durckverluste im Wärmeverbraucher
Entnahme-Kondensation:
- Wärmeverbraucher an früherer Stelle der Entspannung
- Kondensator hinter Turbine
- Wärme auf zwei Temperaturniveaus
Bei KWK in der Dampfturbine kommt es zu Einbußen im elektrischen Wirkungsgrad, da Nutzwärme bei einem höheren Temperaturniveau bereitgestellt werden muss als bei vollständiger Entspannung zur Verfügung stehen würde:
$\eta_{el,KWK}=\frac{\eta_{el,KKW}}{1+\gamma/\sigma}$, mit $\gamma$: Stromverlust-Kennziffer, KKW: Kondensationskraftwerk
## KWK Verbrennungsmotor
Im Verbrennungsmotor kann Wärme aus dem Kühlwasser und aus dem Abgas entnommen werden. Dabei wird zuerst dem Kühlwasser und anschließend dem Abgas Wärme entnommen, da das Temperaturniveau des Kühlwassers unter dem des Abgases liegt.
## Primärenergieeinsparung
Mit KWK kann Primärenergie eingespart werden. Dafür wird zuerst eine Bilanz für den konventionellen Fall aufgestellt:
$(PE)*=PE_K+PE_{KKW}=\frac{\dot{Q}}{\eta_K}(1+\sigma\frac{\eta_K}{\eta_{KKW,el}})$
Darauf aufbauend wird eine Primärenergiebilanz für die KWK aufgestellt:
$PE=PE_{KWK}+PE_K+PE_{KKW}$
Somit kann eine Primärenergieeinsparung $\frac{PE}{PE*}$ definiert werden und in Diagrammen dargestellt werden.
![[Pasted image 20240122144931.png]]
## Kraft-Wärme-Kälte-Kopplung
Die erzeugte Wärme von thermischen Maschinen kann genutzt werden, um in Sorptionskältemaschine Kälte zu erzeugen. Dabei muss Abgewägt werden, ob wirklich eine Einsparung an Primärenergie erzielt wird, da Kältemaschinen im Regelfall einen Wirkungsgrad haben, der größer als 1 ist.
# Energieverteilung und -speicherung
Nah- und Fernwärmenetze dienen der Verteilung von Wärme. Dabei machen Raumwärme und Prozesswärme den größten Teil der Wärmenetze aus (49% und 37 %).

## Rohrauslegung
1. Netzschlechtpunkt
	- Ermittlung des Ortes mit **niedrigstem Leitungsdruck**
	- Verfügbarer Überdruck: $p_ü$
	- Druckverlust für einen Anschlusspunkt i $\Delta p_i=(\Delta p_R+\Delta p_{EW}+\Delta p_{RE}+\Delta p_a)_i$
	- EW: Einzelwiderstand
	- RE: Regelwiderstand
	- R: Reibungswiderstand
	- A: Anschlusswiderstand
2. Rohrreibungs-Druckverlust
	- Widerstandverhältnis $a=\frac{\Delta p_{EW}+\Delta p_{RE}}{\Delta p-\Delta p_A}$
	- $\Delta p=\frac{\Delta p_R}{1-a}+\Delta p_A$
	- Spezifischer Druckverlust $R_i=\frac{\Delta p_{R,i}}{l_i}=\frac{(1-a)(\Delta p-\Delta p_{A,i})}{l_i}$
3. Bestimmung von min($R_{s,i}$)
4. Rohrdurchmesser bestimmen
	- Zugehörigen Durchmesser bestimmen
	- Verfügbare Durchmesser wählen
	- Tatsächlichen Durchmesser wählen
	- Prüfe Geschwinddigkeit $c<c_{max}$
5. Weitere Rohrstrecken

## Speicher
**Speicherladesystem (direkt)**
Wärmeträger wird direkt gespeichert
- Guter Wärmeübergang
- Keine Temperaturdifferenz zwischen Be- und Entladung
- automatische Schichtung im Speicher
- NICHT mit anderen Wärmeträgern kombinierbar

**Speicherladesystem (indirekt Beladen, direkt Entladen)**
Speicher wird indirekt über Wärmeübertrager beladen; Wärmeträgermedium wird direkt aus dem Speicher entnommen
- Verschiedene Wärmeträger möglich
- Automatische Schichtung im Speicher
- JEDOCH Temperaturdifferenz zwischen Be- und Entladen

**Speicherladesystem (direkt Beladen, indirekt Entladen)**
Wärmeträger wird direkt in Speicher geladen. Über Wärmeübertrager wird Verteilungsseite beheizt.
- Vermeidung von Keimen
- ABER Temperaturdifferenz
- ABER große Wärmeübertragerflächen
- ABER Durchmischung im Speicher

**Latente und Sensible Wärme**
![[Pasted image 20240131152740.png]]
Exergieverlust: $E(Q)=T_UQ(\frac{\Delta T}{T_1T_2})$

# Andere Technologien
## Stirlingmotoren
Stirlingmotoren sind Hubkolbenmotoren die mit eine kontinuierlichen Wärmequelle arbeiten. Dabei wird Gas zwischen zwei Kolben - einem heißen und einem kalten Kolben - hin und her geschoben. Dabei dehnt sich das Gas bei Wärmezufuhr im heißen Kolben aus und zieht sich im kalten Kolben bei Wärmeabfuhr wieder zusammen.
![[Pasted image 20231214131845.png]]

## Thermoelektrische Generatoren
Thermoelektrische Generatoren basieren auf dem Seebeck-Effekt, bei dem eine Spannung durch einen Temperaturgradienten erzeugt wird.

Ein Prototyp wurde von BMW entwickelt um die Bordelektronik mit Strom zu versorgen. Dabei konnten Leistungen von ca. 200 Watt erzielt werden. Voraussichtlich sind in wenigen Jahren 1000 Watt realisierbar (Stand 2023).