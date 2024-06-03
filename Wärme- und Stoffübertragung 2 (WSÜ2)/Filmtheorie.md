In der Filmtheorie wird der Stoffübergang entlang eines Films beschrieben. Generelle Annahmen der Filmtheorie sin:
- Starre Grenzfläche
- Eindimensionale Strömung mit Grenzschicht ($\frac{\partial u}{\partial y}$ dominierend)
- Konzentrationsgefälle von $\xi_0$ auf $\xi_\delta$ nur innerhalb der Grenzschicht $\delta_\xi$
- Stofftransport in x- und z-Richtung vernachlässigbar
- Stationäre Verhältnisse, $\xi$ und $D_{AB}=const.$
- Haftbedingung an der Phasengrenze ist erfüllt

![[Pasted image 20240603120628.png]]
# Transportgleichung
Vereinfachung der Transportgleichung:
- Stationär
- keine Konvektion, da Konzentrationsgrenzschicht << Geschwindigkeitsgrenzschicht
- kein Diffusiver Transport in x und z Richtung

$$
\frac{\partial}{\partial y}\left( \rho\frac{\partial\xi}{\partial y} \right)=0
$$
Lösen der DGL:
Randbedingungen:
$$
\xi(y=0)=\xi_{A,0}\text{ und }\xi(y=\delta_\xi)=\xi_{A,\delta_\xi}
$$
Zweimaliges Integrieren führt zu Massenanteil $\xi_A(A)$:
$$
\begin{align}
\frac{\xi_{A,0}-\xi_A(y)}{\xi_{A,0}-\xi_{A,\delta_\xi}}&=\frac{y}{\delta_\xi}
\newline\newline
\xi_A(y)&=\xi_{A,0}-\frac{y}{\delta_\xi}\cdot (\xi_{A,0}-\xi_{A,\delta_\xi})
\end{align}
$$
Somit kann der Stofftransport bestimmt werden zu:
$$
j_A''=-\rho D \left. \frac{\partial\xi_A}{\partial y} \right|_{y=0}=\rho D\frac{\xi_{A,0}-\xi_{A,\delta_\xi}}{\delta_\xi}
$$
Mit $j_A''=g\Delta\xi_A$ folgt somit für den Stoffübergangskoeffizienten: $g=\rho\frac{D}{\delta_\xi}$
# Zweifilmtheorie
Im Gegensatz zur bisherigen Anwendung der Filmtheorie muss die Filmtheorie auf zwei fluide Phasen erweitert werden.
- Potentialdifferenz führt zu einem Stoffübergang von A über die Phasengrenze
- In beiden Phasen bildet sich eine Konzentrationsgenzschicht aus, wobei gilt: Konzentrationsgrenzschicht << Strömungsgrenzschicht
- Innerhalb der $\xi$-Grenzschicht erfolgt der Stofftransport von A ausschließlich diffusiv