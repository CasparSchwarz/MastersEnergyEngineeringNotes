# Beschreibung verfahrenstechnischer Prozesse
In welchem Verhältnis müssen die Edukte zugeführt werden?
- Reaktionsgleichungen
- Stöchiometrie

Muss Energie zu- oder abgeführt werden?
- Energiebilanzen
- Reaktionsenthalpie

Welche Reaktionen laufen ab?
- Reaktionsmechanismus
- Homogegne und heterogene Reaktionen

Weelcher Mechanismus ist geschwindigkeitsbestimment?
- Reaktionskinetik
- Stoffübergang / Diffusion

Welche Produktzusammensetzung entsteht?
- Chemisches Gleichgewicht (siehe [[CE2]])

## Erster Hauptsatz der Thermodynamik
Der 1. HS beschreibt die Energieerhaltung. In stationär durchströmten Reaktionsräumen ist er wie folgt:
$$
\begin{align}
\dot Q+P&=\sum^N_{i=1}\dot n_{a,i}\cdot H_{m,i}(T_a,p_a)-\sum^N_{i=1}\dot n_{e,i}\cdot H_{m,i}(T_e,p_e)
\newline\newline
Mit:\ \dot n_{a,i}&=\dot n_{e,i}+\nu_i\cdot\dot z
\newline\newline
\nu_i&:\ stöchiometrischer\ Koeffizient
\newline
\dot z&:\ Umsatzrate\ der\ Reaktion\ in\ 1/s\newline
N&:\ Gesamtanzahl\ aller\ Reaktanden\newline
H_{m,i}&:\ molare\ Enthalpie\ eines\ Reaktanden\ in\ kJ/mol
\end{align}
$$
## Reaktionsenthalpie
Die Reaktionsenthalpie beschreibt die bei einer Reaktion umgesetzte Energie. Dabei haben exotherme Reaktionen eine Reaktionsenthalpie kleiner als 0 und endotherme Reaktionen eine Reaktionsenthalpie größer als 0:
- exotherm: $\Delta H_R^0<0$
- endotherm: $\Delta H_R^0>0$

Die sogenannte **Standardreaktionsenthalpie** beschreibt die Reaktionsenthalpie bei Standardbedingungen.

Die Standardbildungsenthalpie $H_{B,i}^0$ eines Stoffes bezeichnet die Standardreaktionsenthalpie der Bildungsreaktion des jeweiligen Stoffes. Dabei werden die Standarbildungsenthalpien der Elemente in ihrer stabilsten Form auf den Wert Null festgelegt.
## Chemisches Gleichgewicht
Jede freiwillig ablaufende chemische Reaktion strebt einem Gleichgewicht zu, in dem keine weitere Änderung der Zusammensetzung des Reaktionsgemischs mehr auftritt (siehe [[Reaktionskinetik]])

Die Geschwindigkeit, mit der eine Reaktion stattfindet, wird wie folgt bestimmt:
$$
\begin{align}
\nu_{Hin}&=k_{Hin}\cdot x_A^a\cdot x_B^b\newline
\nu_{Rück}&=k_{Rpck}\cdot x_C^c\cdot x_D^d
\end{align}
$$
Das chemische Gleichgewicht wird über die Gleichgewichtskonstande Beschrieben, wobei sich $K_C$ auf die Stoffmengenanteile und $K_p$ auf die Partialdrücke bezieht.

Das chemische Gleichgewicht befindet sich immer dort, wo die Änderung der Gibbs'schen freien Enthalpie 0 ist:
$$
\begin{align}
\left(\frac{\partial G}{\partial Z}\right)_{T,p}&=\sum^N_{i=0}\nu_i\mu_i=0 
\newline\newline
Mit:\ \mu_i&=\mu_i^0+R\cdot T\cdot ln\left(\frac{p_i}{p^0}\right)
\newline\newline
\rightarrow\sum^N_{i=1}\nu_i\mu_i^0+RT\cdot ln(K_p)&=0
\newline\newline
K_p&=exp\left(-\frac{\sum\nu_i\mu_i^0}{RT}\right)
\end{align}
$$

Das **Prinzip von Le Chatelier** (Prinzip des kleinsten Zwanges):
Ein System im Gleichgewichtszustand "versucht", von außen einwirkende "Zwänge" durch eine Anpassung der Zustandsgrößen zu kompensieren und den "Zwang" zu verkleinern. "Zwänge" sind Temperatur, Druck, Stoffkonzentrationen.
## Reaktionsgeschwindigkeit
Die Reaktionsgeschwindigkeit r ist definiert als die durch die Reaktion bedingte Änderung der Molzahl einer Komponente i mit der Zeit, bezogen auf den stöchiometrischen Koeffizienten $\nu_i$ (siehe [[Reaktionskinetik]]):
$$
r = \frac{1}{\nu_i}\frac{dn_i}{dt}
$$
Die Funktion $f_1$ wird als Geschwindigkeits-Faktor bezeichnet:
$$
f_1:=k=k_0\cdot exp\left(-\frac{E_A}{RT}\right)
$$
Die Funkion $f_2$ erfasst die Abhängigkeit er Reaktionsgeschwindigkeit von den Konzentrationen der Reaktanden und wird durch einen Potenzansatz beschrieben:
$$
\begin{align}
(-\nu_1)A_1+(-\nu_2)A_2&\rightarrow\nu_3A_3+\nu_4A_4
\newline\newline
f_2&=c_{A_1}^{n_1}\cdot c_{A_2}^{n_2}
\end{align}
$$
