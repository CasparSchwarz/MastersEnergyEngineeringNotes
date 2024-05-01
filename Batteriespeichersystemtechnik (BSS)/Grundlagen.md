# Kapazität
Nominaler Strom = Nominalkapazität / Entladedauer.

**C-Rate** beschreibt das Verhältnis aus Nominalkapazität und Nominalstrom und gibt Auskunft über die Nominalentladedauer.
Bsp.: 
Nominalladedauer: 3h
Nominalkapazität: 60 Ah
Nominalstrom: 20 A
Kapazitätsbezeichnung: C/3

**Ladezustand** (SOC): $SOC(t)=SOC(t=0)+\frac{1}{C_{Nenn}}\int^t_{t=0}(I_{Batterie}-I_{Verlust})dt$

**Entladetiefe** (DOD, Depth of Discharge): $DOD=100\%-SOC$

$SOC_{CN}$: Nennkapazität bei Nennstrom und Nenntemperatur
$SOC_{CENAV}$: Verfügbare Kapazität bei Nenntemperatur nach echter Volladung
$SOC_{CENDIS}$: Verfügbare Kapazität bei aktueller Temperatur nach echter Volladung
$SOC_{CAV}$: Kapazität nach Betriebsladung bei Nenntemperatur
$SOC_{CAVDIS}$: Kapazität nach Betriebsladung bei aktueller Temperatur
$C_{rev}$: Reversibler Kapazitätsverlust (z.B. unvollständige Ladung)
$C_{irrev}$: Irreversibler Kapazitätsverlust durch Alterung

**Nennkapazität**: Entnehmbare Strommenge bei Nennbedingungen nach Volladung
**Betriebskapazität**: Kapazität unter Betriebsbedingungen
**Entladegrenze**: Die Kapazität wird nur bis zur Enladeschlussspannung entnommen

Die Kapazität steigt mit der Temperatur, da eine schnellere Diffusion eine geringere Überspannung bedingt. Dementsprechend sorgt eine geringere Temperatur für eine Abnahme der Kapazität.

Die Kapazität nimmt bei steigendem Entladestrom ebenfalls ab, da eine höhere Überspannung notwendig ist um die Reaktionsrate zu halten.
# Chemisches Rechnen
**Masseerrhaltung**: Masse kann nicht zerstört oder erzeugt werden
**Ladungserhaltung**: Ladungen können nicht zerstört oder erzeugt werden
**Molarität**: Konzentration in mol/l
**Molalität**: Konzentration in mol/kg

Ein mol beschreibt die Anzahl an Wasserstoffatomen die einem Gramm entsprechen. $N_A=6,023\cdot 10^{23}$ Wasserstoffatome entsprechen somit einem Gramm.

Die **Faraday'sche** Konstante entspricht der Ladung von einem Mol Elektronen: $F=N_A\cdot e=96485\ \frac{As}{mol}$
## Verschaltung
Die Verschaltung von Batterien lässt die Beeinflussung von Spannung und Kapazität zu. Eine **Serienschaltung** erhöht die Spannung, die Kapazität bleibt unverändert. Eine **Parallelschaltung** erhöht die Kapazität und hält die Spannung konstant.

Um eine höhere Redundanz zu erreichen werden Strangweise Parallelschaltugnen oder Parallelschaltungen auf Zellebene genutzt:
![[Pasted image 20240422100710.png]]

# Batteriespannung
Bei gleichbleibendem Entladenstrom sinkt die Spannung einer Batterie mit zunehmender Depth of Discharge.
![[Pasted image 20240419140620.png]]

Die **Batterieklemmspannung** setzt sich dabei aus verschiedenen Anteilen zusammen:
$U_{Batterieklemmspannung}=U_{Gleichgewicht}+U_{Widerstand}+U_{Reaktion}+U_{Diffusion}$
mit
- $U_{Gleichgewicht}$ Ist eine Funktion der Elektrolytkonzentration und der Temperatur; hängt in Bleibatterien stark vom Ladezustand ab (Auch Open Circuit Voltage genannt)
- $U_{Widerstand}$ beschreibt die ohm'schen Verluste in Polen, Ableitern, Gittern und Elektrolyten (Ohm'sches Gesetz)
- $U_{Reaktion}$ ist der Spannungsabfall durch die elektrochemischen und chemischen Reaktionen (Butler-Volmer-Gleichung)
- $U_{Diffusion}$: Spannungsabfall durch Defizit oder Überschuss von Reaktanten an den Reaktionsorten

$U_{Widerstand},\ U_{Reaktion},\ U_{Diffusion}$ i.A. negativ beim Entladen und positiv beim Laden

## Ruhespannung / Gleichgewichtsspannung
Die Ruhespannung kann an der Batterie im unbelasteten Zustand gemessen werden, wenn alle Ausgleichsvorgänge abgeklungen sind. Die Batteriespannung ist beim Entladen immer geringer als die Ruhespannung beim jeweiligen Ladezustand. Die Batteriespannung ist beim Laden immer höher als die Ruhespannung im jeweiligen Ladezustand.

Über die Ruhespannung kann der Ladezustand einer Batterie korreliert werden.

Die Gleichgewichtsspannung ist immer positiv definiert.

Bestimmung der Gleichgewichtsspannung über die Gibb'sche freie Energie:
$\Delta G=\Delta H-T\Delta S$

Freigesetzte Ladung: $\tilde{Q}=z\cdot F$ oder $Q=n_{mol}\cdot z \cdot F$
$$
\begin{align}
\Delta G &= -U_0\cdot\tilde{Q} \newline
\Delta G &=-U_0\cdot z\cdot F\newline
U_0&=-\frac{\Delta G}{z\cdot F}
\end{align}
$$

Die Gleichgewichtsspannung ändert sich jedoch mit der Ionenkonzentration, sodass bei höheren Elektrolytkonzentrationen die **Nernst-Gleichung** angewendet werden muss:
$$
\Delta G=\Delta G_S+RT\cdot(\sum ln[{a_i}^{j_i}]_{ende}-\sum ln[{a_i}^{j_i}]_{start})
$$
## Widerstandsspannung (Ohm'scher Verlust)
$U_{Widerstand}$ beschreibt Ohm'sche Verluste in Polen, Stromsammlern, Gittern und Elektrolyt. Die Verluste verhalten sich wie folgt:
- Direkt und linear proportional zu Lade- und Entladestrom
- Direkter Spannungsabfall bei Beginn eines Stromflusses
- Beim Entladen negativ, beim Aufladen positiv
- Widerstand des Elektrolyten der größte Beitrag
- Widerstand des Elektrolyten sinkt mit steigender Temperatur

## Reaktionsspannung
$U_{Reaktion}$ beschreibt den Spannungsabfall durch die elektrochemischen (Butler-Volmer-Gleichung [[Elektrochemie#Butler-Volmer Gleichung]]) und chemischen Reaktionen bei Stromfluss. Sie ist dabei proportional zur inneren Oberfläche und logarithmisch abhängig vom Batteriestrom.
- Wird bedingt durch den eigentlichen Lade-/Entladeprozess an beiden Elektroden
- Führt beim Laden der Batterie zu einer Erhöhung der Batteriespannung gegenüber der Gleichgewichtsspannung und beim Entladen umgekehrt

Zu jedem Zeitpunkt müssen anodische und kathodische Reaktion mit gleicher Rate $i_0$ ablaufen. Im Gleichgewichtszustand sind die Reaktionsraten gleich und **nicht Null**.
- Anodische Reaktion führt zur Entladung (Oxidation); Entzug von Elektronen
- Kathodische Reaktion führt zur Ladung (Reduktion); Zufuhr von Elektronen

Für kleine und große Ströme kann die Butler-Volmer-Gleichung vereinfacht werden:
$$
\begin{align}
Kleine\ Ströme:\ \Delta U &=\frac{RT}{F}\cdot \frac{I}{A\cdot i_0}
\newline
Große\ Ströme:\ \Delta U&=\frac{RT}{\alpha\cdot F}\cdot ln\left(\left|\frac{ I}{A\cdot i_0}\right|\right)
\end{align}
$$
Bei $\alpha=0,5$ laufen anodische und kathodische Reaktionen gleichschnell ab:
$$
\begin{align}
\Delta U&=\frac{1}{K}\cdot sinh^{-1}\left( \frac{I}{I_0} \right)
\newline
Mit \ K&=\frac{0,5\cdot n\cdot F}{RT}
\end{align}
$$
## Diffusionsspannung
$U_{Diffusion}$ beschreibt die aus dem Konzentrationsgradienten der Reaktanten resultierende Überspannung.
- wegen langsamen Austausch mit Elektrolytreservoir
- Kristallwachstum oder Abnahme der Porosität führt zu beschleunigter Abnahme der Reaktanten
- Abbau von $U_{Diffusion}$ dauert Zeit -> nach Wartezeit weitere Entladung der Batterie möglich
$$
(U-U_0)_{conc}=-\frac{RT}{n\cdot F}\cdot ln\left(\frac{c}{c_0}\right)
$$
Durch den elektrochemischen Prozess entstehen Ladungsträgergradienten, da der äußere Strom die Reaktionsrate bestimmt und somit Ungleichgewichte und Konzentrationsgradienten entstehen. Die Reaktionsgeschwindigkeit hängt von der Temperatur ab (siehe [[Reaktionskinetik]])
## Energie
Die Ruhespannung multipliziert mit der Kapazität definiert die maximal aus der Batterie entnehmbare Energiemenge. Die Kapazität hängt linear mit der Menge der vohandenen Elektrodenmaterialien zusammen. Dabei wird die Batteriezelle nie bis 0 V entladen.

# Wirkungsgrad
Ladefaktor: $L=\frac{eingeladene Ah}{entnommene Ah}$

Coulombscher Wirkungsgrad: $\eta_{Ah}=\frac{1}{L}$

Voltairscher Wirkungsgrad: $\eta_U=\frac{mittlere Entladespannung}{mittlere Ladespannung}$

Energetischer Wirkungsgrad: $\eta_{Wh}=\frac{entnommene Wh}{eingeladene Wh}$

# Ladung & Entladung
Bei der Entladung gibt es verschiedene Entladeregime:
![[Pasted image 20240419145841.png]]

Bei der Ladung werden ebenfalls verschiedene Methoden verwendet:
![[Pasted image 20240422115430.png]]

# Reversible und irreversible Wärme
Die sogenannte kaliometrische Spannung wird berechnet aus der Gleichgewichtsspannung und der reversiblen Wärme:
$$
\begin{align}
Q_{rev}&=T\cdot \Delta S=\Delta H-\Delta G
\newline
U_{cal}&=U_0-\frac{Q_{rev}}{n\cdot F}
\end{align}
$$
Die Änderung der thermischen Energie ist die Summe aus reversiblen Wärme und Joule'scher Wärme:
$$
\frac{dQ_{thermal}}{dt}=\frac{dQ_{Joule}}{dt}+\frac{dQ_{rev}}{dt}=(U-U_{cal})\cdot I
$$
Wird der Entladeprozess im Gleichgewicht gehalten nimmt die Temperatur ab. Da dies der facto nicht möglich ist und die Batterie bei Überspannung betrieben werden muss, erwärmt sich die Batterie über Ohm'sche Spannungsabfälle.

# Energiedichten
Elektrochemische Speicher sind massenbehaftete Speichersysteme. Dabei kann ein Atom oder Molekül eine maximale, diskrete Zahl von $n$ Elektronen speichern. Dadurch lassen sich theoretische maximale Energiedichten bestimmen, welchen sich asymptotisch genähert werden kann.

Praktische Energiedichten sind erheblich geringer (ca. 1/3 der theoretischen Energiedichte ist realisierbar), weil Trägermaterialien, Elektrolyte, Separatoren, Stromsammlern und Gehäuse benötigt werden.

Es gilt: Je höher das Potential, desto aggresiver die Materialien -> Sicherheitsrisiko, Lebensdauerproblem

$$
Speicherbare\ Energie:\ n\cdot F\cdot U_0
$$

# Wässrige Elektrolyten
Die Gasungsreaktion, bei der Wasserstoff und Sauerstoff entstehen, läuft immer ab, wenn die Zellspannung die Wasser-Zersetzungsspannung von 1,23 V überschreitet (siehe [[Elektrochemie#Elektrolyseur]]). Dabei entsteht an der positiven Elektrode Sauerstoff und an der negativen Elektrode Wasserstoff. Bei allen kommerziellen Batterien ist die Gasungsrate bei Raumtemperatur und Leerlaufspannung sehr gering. In Batterien mit wässrigem Elektrolyten muss nach einiger Zeit entionisiertes Wasser nachgefüllt werden, da durch den Gasungsprozess der Wasserspiegel sinkt.

# Ragone Diagramm
Das Ragone Diagramm zeigt die spezifische Leistung über der spezifischen Energie:
![[SmartSelect_20240501_093920_Drive.jpg]]
Dabei ist zu kennen, dass niemals eine hohe spezifische Leistung und eine hohe spezifische Energie realisiert werden können.

# Metall-Luft Batterien
In Metall-Luft Batterien reagiert Metall mit Sauerstoff aus der Luft. Die Oxidation setzt dabei Elektronen frei, welche in Form von elektrischen Strom nutzbar sind. In dieser Form von Batterie wird nur eine anstatt zwei Halbzellen benötigt. Zu möglichen Metall-Luft Systemen gehören:
- Zink-Luft
- Lithium-Luft
- Aluminium-Luft

