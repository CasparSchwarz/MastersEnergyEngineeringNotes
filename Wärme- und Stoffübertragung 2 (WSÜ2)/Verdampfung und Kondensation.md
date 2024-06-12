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
## Van der Vaals Gleichung
Bisher ist das **ideale Gasgesetz** bekannt:
- Keine Interaktion zwischen Molekülen
- Moleküle nehmen kleinen Raum ein, Bahnlänge zwischen Stößen ist groß
-> Versagt bei hohen Drücken

Zustandsgleichung von Van der Vaals:
- 