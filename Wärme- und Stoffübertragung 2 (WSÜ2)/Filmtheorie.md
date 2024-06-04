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
Im Gegensatz zur bisherigen Anwendung der Filmtheorie muss die Filmtheorie auf zwei fluide Phasen erweitert werden. Die Zweifilmtheorie kann nur verwendet werden, wenn beide Phasen nicht miteinander mischabr sind.
- Potentialdifferenz führt zu einem Stoffübergang von A über die Phasengrenze (gemeint ist das **chemische Potential**)
- In beiden Phasen bildet sich eine Konzentrationsgenzschicht aus, wobei gilt: Konzentrationsgrenzschicht << Strömungsgrenzschicht
- Innerhalb der $\xi$-Grenzschicht erfolgt der Stofftransport von A ausschließlich diffusiv

## Flüssig zu flüssig
Aufgrund der Massenerhaltung: $j_1''=j_2''$
![[Pasted image 20240604132336.png]]
Der diffusive Stoffübergang wird wie folgt berechnet:
$$
j''=j_1''=g_1(\xi_{\infty,1}-\xi_{g,1})=j_2''=g_2(\xi_{\infty,2}-\xi_{g,2})
$$
Das chemische Potential entscheidet über das Verhältnis von $\xi_{g,1}$ zu $\xi_{g,2}$. Das Verhältnis lässt sich bei Diffusion durch eine Phasengrenze zweier flüssiger Phasen über das **Nernst'sche Gesetz** bestimmen:
$$
K_N=\frac{\xi_{g,1}}{\xi_{g,2}}
$$
Daraus folgt für der Stoffdurchgang:
$$
\begin{align}
j''&=\frac{\xi_{\infty,1}-K_N\xi_{\infty,2}}{\frac{1}{g_1}+\frac{K_N}{g_2}}
\newline\newline
\frac{1}{k_{\xi,1}}&=\frac{1}{g_1}+\frac{K_N}{g_2}
\end{align}
$$
## Flüssig zu gasförmig
Beim Stoffübergang zwischen eine flüssigen und gasförmigen Phase sind keine Massenanteile gegeben, sondern Konzentrationen in der Flüssigkeit und Partialdrücke in der Gasphase. Das Phasengleichgewicht zwischen Flüssig- und Gasphase wird durch den Herny-Koeffizienten $K_{HC}$ beschrieben (siehe [[Phasengleichgewichte#Henry-Koeffizient]]):
$$
p_A=K_{HC,A}C_A
$$
Für kleine Konzentrationen kann der $K_{HC}$ über den bekannten Herny-Koeffizienten $H_{fl}$ korreliert werden:
$$
K_{HC,A}=H_{A,fl}\frac{M_{fl}}{\rho_{fl}}
$$
Da die Absorption von Gas in Flüssigkeiten exotherm ist, wird mehr Gas bei niedrigen Temperaturen in der Flüssigkeit gelöst:
$$
\begin{align}
\frac{d\ ln(K_{HC,A})}{dT}&=-\frac{\Delta h_{Abs,A}}{RT^2}
\newline\newline
Mit\ \Delta h_{Abs,A}&\text{: Absorptionsenthalpie des Stoffes A}
\end{align}
$$
Somit folgt für den Stoffmengenstrom:
$$
\dot n_A''=\frac{K_{HC,A}C_{A,\infty}-p_{A,\infty}}{R\frac{T}{\beta_G}+\frac{K_{HC,A}}{\beta_{Fl}}}
$$
Dabei stellen $\beta_i$ die Stoffübergangskoeffizienten analog zu $g_i$ dar.
# Rieselfilm
