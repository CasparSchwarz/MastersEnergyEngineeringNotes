Speicherung von Energie wird mit dem Zuwachs an erneuerbaren Energien im Energiesystem immer wichtiger, da die Stromerzeugung durch erneuerbare Energien weniger vorhersehbar ist, als die Stromerzeugung aus fossilen Primärenergieträgern. Somit müssen Last- und Erzeugungsspitzen durch  Speicher ausgeglichen werden.

Speicher werden wie folgt klassifiziert:
- Physikalisch
	- Thermisch, Chemisch, Elektrisch, Mechanisch
- energetisch
	- Leistung und Energie
- zeitlich
	- Kurzzeit und Langzeit
- räumlich
	- Zentral, Dezentral, Ortsfest, Mobil
- ökonomisch
	- Marke, Kapitalkosten, Betriebskosten

# Mathematische Beschreibung
Eingespeicherte Energiemenge:
$E_x=\int_{t=0}^{t_x}P_x(t)dt$

Gesamtwirkungsgrad des Speichersystems:
$\eta_{ges}=\eta_{ein}\cdot\eta{sp}\cdot\eta{aus}=\frac{E_{aus}}{E_{ein}}$

Energiedichte und spezifische Energie:
$e_V=\frac{E_{sp}}{V}$, $e_m=\frac{E_{sp}}{m}$

# Thermische Speicher
Thermische Speicher speichern thermische Energie indem sie Wärme oder kälte aufnehmen. Es wird unterschieden zwischen
- sensiblen (fest, flüssig),
- latenten (fest-flüsssig, flüssig-gasförmig, fest-fest) und
- thermo-chemischen (Sorption, chemisch reversibel) Speichern.

## Sensible Wärmespeicherung
Als sensible Wärme wird die Wärme verstanden, die bei Zufuhr oder Abfuhr eine Temperaturänderung zur Folge hat. Dementsprechend ist die Wärmeaufnahme / -abgabe fühlbar.

Häufig wird Wasser als sensibler Wärmespeicher verwendet, da Wasser
- eine hohe Wärmekapazität besitzt,
- umweltverträglich ist,
- eine hohe Verfügbarkeit existiert und
- die Kosten  gering sind.

Wärmemenge: $Q=m\cdot c_w\cdot\Delta T$

Sensible Wärmespeicher sind Verlustbehaftet, da mit der Zeit Wärme aus dem Speicher an die Umgebung abgegeben wird.

Verlustwärmestrom: $\dot{Q}_{Verlust}=U\cdot A\cdot (T_S-T_U)$

## Latente Wärmespeicher
Als Latente Wärme wird die Wärme bezeichnet, die bei Wärmezufuhr / -abfuhr keine Temperaturänderung zur Folge hat, sondern einen Phasenwechsel bei konstanter Temperatur herbeiführt.

$Q=m\cdot (c_{fe}\cdot\Delta T_{fe}+\Delta h_s + c_{fl}\cdot \Delta T_{fl})$

# Thermochemische Speicher
In thermochemischen Speichern wird Rekationsenergie von reversiblen chemischen Prozessen oder von Oberflächenreaktionen genutzt, um Energie zu speichern.

Vorteile:
- Besonders hohe Energiedichte
- Keine thermischen Verluste während der Speicherung
- Lange Speicherdauern möglich
Nachteil: Aus wirtschaftlicher Sicht uninteressant

Chemisch reversible Prozesse:
- Thermodynamische Gleichgewichtstemperatur entscheident
- T>T_gg: Endotherme Reaktion -> Beladung
- T<T_gg: Exotherme Reaktion -> Entladung

Adsorptionsspeicher: Physikalische Anlagerung von Molekülen an die Oberfläche eines Adsorbens

Absorptionsspeicher: Chemische Einlagerung  eines Moleküls in die absorbierende Schicht.

# Chemische Speicher
Chemische Speicher nutzen chemische Umwandlungsprozesse oder Stoffe um Energie zu speichern. Dabei sit zwischen elektrochemischen Speichern und stofflichen Speichern zu unterscheiden.

## Elektrochemische Energiespeicher
Als elektrochemischer Energiespeicher wird im Allgemeineneine Galvanische Zelle verstanden. Dabei wird Energie über Oxidation und Reduktion von Anode und Katode gespeichert.

## Stoffspeicher
Als Stoffspeicher wird das Speichern von Energie in chemischen Bindung verstanden. Der Stoff kann dabei im festen, flüssigen oder gasförmigen Zustand sein. Bei der Speicherung von Gasen wird das ideale Gasgesetz verwendet,  um auf das Nennvolumen Gas zurückzuschließen. Das  ist notwendig, da sich die gespeicherte Masse in Abhängigkeit vom Druck bei gleichem Volumen ändert.

Ideales Gasgesetz: $pV=nRT$
Normzustand: $p_nV_n=nRT_n$ mit $p_n=1,01325 \ bar$, $T_n=273,15 \ K$

Zur Beschreibung von realen Gasen muss das ideale Gasgesetz mit einem Realgasfaktor $Z$ beaufschalgen.

Reale Gase: $pV=nZRT$
Normzustand: $p_nV_n=nZ_nRT_n$
Kompressibilitätszahl: $K=\frac{Z_1}{Z_n}=\frac{p_1V_1T_n}{p_nV_nT_1}$

Für Erdgas entspricht die Kompressibilitätszahl zwischen 12 °C und 70 °C: $K=1-\frac{p_1}{450\ bar}$

# Elektrische Speicher
Unter einem elektrische Speicher wird im Allgemeinen ein Kondensator verstanden, welcher in einem elektrischen Feld Energie speichert.

Kapazität: $C=\epsilon_0\epsilon_r\cdot\frac{A}{d}$
Gespeicherte Energie: $W=\frac{1}{2}\cdot C\cdot  U_c^2$

Spezielle Kondensatoren  sind Superkondensatoren. Zu diesen Zählen Doppelschichtkondensatoren, Pseudokondensatoren und Hybridkondensatoren.

# Mechanische Speicher
Mechanische Speicher speichern Energie in Form von mechanischer Energie. Diese kann in kinetischer oder in potenzieller Form vorliegen. Zu den üblichen Speichern gehören
- Druckluftspeicherkraftwerke
- Pumpspeicherkraftwerke
- Schwungradspeicher

## Druckluftspeicher
In Druckluftspeichern wird Überschussstrom genutzt um Umgebungsluft in  unterirdische Kavernen zu pumpen. Durch die Druckerhöhung wird Energie gespeichert.

In einem **adiabaten Kraftwerksprozess** wird die bei der Kompression entstehende Wärme in einem Wärmespeicher eingespeichert. Beim Entladen kann somit die Wärme dem entspannten Gas wieder zugeführt werden. Wird die Wärme genutzt kann ein Wirkungsgrad von ca. 70 % erreicht  werden.

## Schwungradspeicher
In einem Schwungradspeicher wird Energie in Form von kinetischer Energie eines sich drehenden Schwungrades gespeichert. Hierbei wird ein Schwungrad durch einen Elektromotor auf hohe Drehzahlen beschleunigt. Beim Ausspeichern wird der Elektromotor als Generator betrieben.