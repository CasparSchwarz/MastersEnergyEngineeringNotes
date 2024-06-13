Unter Verdampfung und Kondensation werden jeweils der Phasenwechsel von flüssig zu gasförmig und gasförmig zu flüssig verstanden (siehe auch [[Verdampfung & Kondensation]]).

Der Unterschied zwischen Verdunstung und Verdampfung ist, dass Verdunstung in Gegenwart anderer Gase geschieht und nicht isotherm sein muss. Verdampfung bezieht sich nur auf einen Reinstoff.
# Thermodynamische Grundlagen
![[SmartSelect_20240612_184032_Drive.jpg]]
Die verrichtete Arbeit berechnet sich wie folgt:
$$
\begin{align}
\partial a&=(v_g-v_{fl})\ dp \\\\
\partial a&=(s_g-s_{fl})\ dT
\end{align}
$$
Werden diese Formeln gleichgesetzt, kann eine Gleichung für die Dampfdruckkurve gefunden werden, die Gleichung von **Clausius und Clapeyron**:
$$
\begin{align}
\frac{\partial p}{\partial T}&=\frac{\Delta h_{V,m}}{T(v_{d,m}-v_{fl,m})}\\ \\
\text{Mit: }\Delta h_{V,m}&=T\cdot M\cdot (s_g-s_{fl})
\end{align}
$$
Wobei $v_{i,m}$ für das Molare Volumen steht.

Wird vereinfacht das Molare Volumen der Flüssigkeit als deutlich kleiner als das molare Volumen des Gases und das Gas als ideal angenommen:
$$
\frac{\partial p}{\partial T}=\frac{\Delta h_{V,m}\cdot p}{R\cdot T^2}
$$

Wenn der Druck erhöht wird, erhöht sich auch der Sättigungsdampfdruck. Analog dazu verringert sich der Sättigungsdampfdruck, wenn sich der Druck verringert. Dieses Verhalten kann mit dem chemischen Potential modelliert werden, da die Druckänderung das chemische Potential verschiebt:
$$
\begin{align}
\text{Dampfphase:  } d\mu_d&=v_{m,d}\cdot dp_i \\\\
\text{Flüssigphase: } d\mu_{fl}&=v_{m,fl}\cdot dp_{ges}
\end{align}
$$
Somit kann der verschobene Sättigungsdampfdruck wie folgt bestimmt werden:
$$
p^*_{sat}=p_{sat}\cdot exp(v_{m,fl}\cdot\frac{\Delta p}{RT})
$$
# Van der Waals Gleichung
Bisher ist das **ideale Gasgesetz** bekannt:
- Keine Interaktion zwischen Molekülen
- Moleküle nehmen kleinen Raum ein, Bahnlänge zwischen Stößen ist groß
-> Versagt bei hohen Drücken

Zustandsgleichung von Van der Waals:
- Bei hohen Dichten wird das Molekülvolumen berücksichtigt
- Intermolekulare Stöße werden berücksichtigt

1. Berücksichtigung des Molekülvolumens -> Korrektur des idealen Gasgesetzes:
$$
p(v_m-b)=RT
$$
2. Berücksichtigung von Intermolekulare Kräften (antiprop. zum Molvolumen)
$$
p_i=p+\frac{a}{v_m^2} 
$$
Wobei $a$ eine Stoffkonstante ist.

Somit folgt für die Zustandsgleichung von Van der Waals:
$$
p=\frac{RT}{v_m-b}-\frac{a}{v_m^2}
$$
Und geht damit ins ideale Gasgesetz ein.

Die Isothermen nach Van der Waals zeigen eine kubischen Verlauf und sorgen für ein Überschwingen im Zwei-Phasen-Gebiet. Werden die Minima bis zum kritischen Punkt und die Maxima vom kritischen Punkt miteinander verbunden, entsteht folgendes Diagramm:
![[SmartSelect_20240612_194516_Firefox.jpg]]
Von D bis C sind die Zustände physikalisch nicht möglich und dementsprechend instabil, da in dem Bereich ein höheres spezifisches Volumen mit einem höheren Druck korrelieren würde.

Der metastabile Bereich zeigt den Bereich, in welchem durch Druckverminderung bei Flüssigkeiten der flüssige Aggregatzustand gehalten werden kann, ohne dass sich Gasblasen bilden. In der Realität ist die Kurve von A nach D nur sehr schwierig umzusetzen und in industriellen Prozessen geht die Flüssigkeit direkt in siedendes Verhalten über. Analog dazu ist auch der metastabile Bereich der Gasphase beschrieben.
# Gekrümmte Phasengrenze
Gekrümmte Phasengrenzen kommen häufig vor, beispielsweise an einer Dampfblase in einer Flüssigkeit. Dabei erzeugt die Oberflächenspannung einen Drucksprung an der Oberfläche, wodurch das chemische und mechnische Gleichgewicht verschoben werden.
## Oberflächenspannung
Die Oberflächenspannung kann über ein Kräftegleichgewicht an der Dampfblase bestimmt werden. Durch Gleichsetzen von Druckkraft und Oberflächenkraft wird die Young-Laplace-Gleichung hergeleitet:
$$
p_g-p_{fl}=\frac{2\sigma}{R}
$$
Aber! $p_g$ und $p_{fl}$ entsprechen nicht dem Sattdampfdruck.
## Bestimmung $p_g$ und $p_{fl}$
Über das chemische Gleichgewicht können die Drücke bestimmt werden:
$$
\begin{align}
p_{fl}&=p_{sat}-\frac{\rho_{fl}}{\rho_{fl}-\rho_g}\frac{2\sigma}{R} \\\\
p_g&=p_{sat}-\frac{\rho_{fl}}{\rho_{fl}-\rho_g}\frac{2\sigma}{R}
\end{align}
$$
Für einen Flüssigkeitstropfen in Dampfatmosphäre ändert sich nur das Vorzeichen der Gleichung:
$$
\begin{align}
p_{fl}&=p_{sat}+\frac{\rho_{fl}}{\rho_{fl}-\rho_g}\frac{2\sigma}{R} \\\\
p_g&=p_{sat}+\frac{\rho_{fl}}{\rho_{fl}-\rho_g}\frac{2\sigma}{R}
\end{align}
$$
## Bestimmung $T_g$ und $T_{fl}$
Bei Vorgabe eines konstanten Drucks $p_0$ in der Dampfblase und der Flüssigkeit soll nun die zugehörige Temperatur bestimmt werden. Dafür kann mit der Clasius-Clapeyron-Gleichung ein Zusammenhang gefunden werden:
$$
\begin{align}
T_{fl}-T_{sat}=\frac{T_{sat}M}{\rho_g\Delta h_{v,m}}\frac{2\sigma}{R}\\\\
T_g-T_{sat}=\frac{T_{sat}M}{\rho_{fl}\Delta h_{v,m}}\frac{2\sigma}{R}
\end{align}
$$
# Ursache für Blasenbildung
In hochreinen Flüssigkeiten kann Blasenbildung unterdrückt werden. In der Realität gibt es jedoch sogenannte "aktive Zentren", an denen Verunreinigungen oder Vertiefungen für die Blasenbildung sorgen. Somit dehnt sich an diesen Stellen die Blase bei Wärmezufuhr aus bis zu groß genug ist und reist dann ab.