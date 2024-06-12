Unter Verdampfung und Kondensation werden jeweils der Phasenwechsel von flüssig zu gasförmig und gasförmig zu flüssig verstanden (siehe auch [[Verdampfung & Kondensation]]).
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
## Van der Waals Gleichung
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