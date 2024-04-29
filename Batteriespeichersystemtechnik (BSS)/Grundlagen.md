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


