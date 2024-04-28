# Realer Kontakt
Die reale Kontaktfläche zweier Körper ist kleiner als die nominelle Kontaktfläche, da reale Flächen nicht vollständig glatt sind. Somit liegen nicht die gesamten Flächen zweier Körper aufeinander.
![[Pasted image 20240424125015.png]]
Der aus den realen Flächen resultierende Kontaktwiderstand ist im Allgemeinen abhängig von:
- Werkstoffpaarung
- Kontaktdruck
- Oberflächenbeschaffenheit
- und zu Teilen von der Temperatur

# Mathematische Grundlage
Für den Kontaktwiderstand $W_k$ gilt:
$$
\dot{Q}_K=\frac {T_{A,K}-T_{B,K}}{W_K}
$$
$W_K$ kann in drei Regime unterteilt werden:
1. $W_K=0$
	- Idealer Kontakt, kein Widerstand -> Stetiger Temperaturverlauf
2. $W_K=\infty$ 
	- Adiabater Kontakt
	- -> Es kann keine Wärme fließen
	- -> Sprung im Temperaturverlauf
3. $0<W_K<\infty$
	- realer Kontakt
	- Makroskopisch: Temperatursprung an der Kontaktstelle
	- Mikroskopisch: Verdichtung der Wärmestromlinien in den Kontaktspitzen -> Positionsabhängig sehr hohe Temperaturgradienten
	- Formelmäßige Beschreibung analog zu Konvektion:
	- $\dot{Q}_K=\alpha_K\cdot\Delta T\cdot A_{nom}$

# Wärmetransportmechanismen 
$\alpha_K$ ist die Summe der Wärmeübergangskoeffizienten der verschiedenen auftretenden Wärmetransportmechanismen:
$$
\alpha_K=\sum\alpha_i
$$
Zu den Auftretenden Wärmetransportmechanismen gehören:
1. Wärmeleitung in
	- Kontaktspitzen
	- Gastaschen
2. Konvektion in den Gastaschen
3. Strahlungsaustausch in den Gastaschen

![[Pasted image 20240424125951.png]]

$$
\begin{align}
\dot{Q}_K&=\alpha_K\cdot\Delta T_K\cdot A_{nom}
\newline
mit: \ \alpha_K&= \alpha_{L,F}+\alpha_{L,G}+\alpha_S
\end{align}
$$

## Konvektion in den Gastaschen
In den Gastaschen ist ausschließlich natürliche Konvektion möglich. Das vorhandensein von natürlicher Konvektion ist abhängig von der Rayleigh Zahl:
$$
Ra=Gr\cdot Pr = \frac{g\rho c_p\beta}{\nu\lambda}\Delta T l^3
$$

-> Natürliche Konvektion tritt auf, wenn $Ra>2000$

## Strahlungsaustausch in den Gastaschen
Um den Strahlungsaustausch zu beschreiben, wird dieser als Strahlungsaustausch zweier paraleller ebener Platten modelliert:
$$
\begin{align}
\dot{Q}_S&=\frac{A_{nom}-A_{real}}{\frac{1}{\epsilon_A}+{\frac{1}{\epsilon_B}-1}}\sigma(T^4_{K,B}-T^4_{K,A})
\newline
\alpha_S&=\frac{A_{nom}-A_{real}}{A_{nom}}\frac{\sigma}{\frac{1}{\epsilon_A}+{\frac{1}{\epsilon_B}-1}}\frac{T^4_{K,B}-T^4_{K,A}}{T_{K,B}-T_{K,A}}
\end{align}
$$
# Knudseneffekt
Die Knudsen-Zahl ist maßgeblich für die Wärmeübertragung in Gastaschen und beschreibt das Verhältnis von $\delta$ und $\Lambda$:
$$
\begin{align}
Kn&=\frac \Lambda \delta \newline
mit \ \Lambda&: Freie\ Weglänge
\newline

\delta&:\ Abstand
\end{align}
$$
Die Wärmeleitfähigkeit einer Gasschicht kann in 4 Knudsen-Zahl-Bereiche eingeteilt werden:
1. $Kn << 1$ Kontinuum
	- Spalt deutlich größer als freier Weglänge -> normale Wärmeleitung
2. $0,01 \leq Kn \leq 0,1$ Temperatursprung
	- Kein vollständiger Energietransport zwischen Gasmolekülen und Feststoffoberfläche -> Temperatursprung an der Oberfläche
3. $0,1\leq Kn\leq 10$ Übergangsbereich
	- Wärmeleitung durch intermolekulare Stöße und Wärmeübergang durch Stöße an der Feststoffoberfläche in der gleichen Größenordnung
4. $10<Kn$ Freie Molekularströmung
	- Stöße zwischen Gasmolekülen sehr selten -> Wärmetransport ausschließlich zwischen Gasmolekülen und Feststoffoberfläche

Im Bereich des Temperatursprungs kann der Wärmeübergangskoeffizient der Gasschicht über ein Ignorieren des Temperatursprungs modelliert werden:
$$
\alpha_{L,G}=\frac{\lambda_G}{\delta_G}
$$
