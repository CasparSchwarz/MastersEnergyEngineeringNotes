# Modellierung oder Schließung der Transportgleichung
- Zwei Schritte
	1. Einführung des Gradiententransportansatzes -> Wirbelviskosität
	2. Modellierung der Wirbelviskosität

Somit mit turbulenten Spannungstensor und Gradiententransportansatz:
$-\overline{u_i'u_j'}=\nu_t(\frac{\partial \bar{u}_i}{\partial x_j}+\frac{\partial\bar{u}_j}{\partial x_i})$ mit $\nu_t$ als Wirbelviskosität (scheinbare Zähigkeit)

Die Wirbelviskosität wird verursacht durch turbulente Wirbel. Die Dimensionsanalyse ergibt: $\nu_t \sim l_tu'$

## Modellierung der Wirbelviskosität
Nach **Prandtl-Kolmogorov**
$\nu_t=C_{\mu}l_{pk}\sqrt{k}$
$C_{\mu}$ ist eine Modellkonstante und nimmt häufig den Wert 0,09 an
$l_{pk}$ ist die Charakteristische Länge -> empirisch zu bestimmen

-> Gleichung für die turbulente kinetische Energie:
$\frac{\partial\bar{k}}{\partial t}+\bar{u}_i\frac{\partial\bar{k}}{\partial x_i}=P_k-\bar\varepsilon+\frac{\partial}{\partial x_i}(\frac{\nu_t}{P_{r_k}}\frac{\partial\bar{k}}{\partial x_i})$ mit $P_k=-\overline{u_i'u_j'}\frac{\partial\bar{u}_j}{\partial x_i}$ und $\bar\varepsilon = C_D\frac{k^{3/2}}{l_{pk}}$

**k-$\varepsilon$-Modell**
$\nu_t=C_{\mu}\frac{k^2}{\varepsilon}$
Zur Schließung: Lösuen je einer Gleichung für
- TKE $\frac{\partial\bar{k}}{\partial t}+\bar{u}_i\frac{\partial\bar{k}}{\partial x_i}=P_k-\bar\varepsilon+\frac{\partial}{\partial x_i}(\frac{\nu_t}{P_{r_k}}\frac{\partial\bar{k}}{\partial x_i})$
- Dissipation: $\frac{\partial\bar{\varepsilon}}{\partial t}+\bar{u}_i\frac{\partial\bar{\varepsilon}}{\partial x_i}=(c_{\varepsilon 1}P_k-c_{\varepsilon 2}\bar{\varepsilon})+\frac{\partial}{\partial x_i}(\frac{\nu_t}{P_{r_k}}\frac{\partial\bar{\varepsilon}}{\partial x_i})$

# Modellierung turbulenter Diffusionsflammen
Zur Modellierung turbulenter Diffusionsflammen werden [statistische Methoden](Statistische%20Beschreibung%20turbulenter%20Verbrennung.md) benötigt.

Für den Grenzfall **unendlich schneller Chemie** kann die lokale Zusammensetzung allein durch die Beschreibung der Mischung ermittelt werden (siehe [[CE2#Bilanzgleichung für den Mischungsbruch]]). Aus dem Mischungsbruch kann die Zusammensetzung und die Temperaturverteilung ermittelt werden:
$\tilde{T}=\int^{+\infty}_{-\infty}T(Z)\tilde{f}(Z)dZ$ und $\tilde{Y}_i=\int^{+\infty}_{-\infty}Y_i(Z)\tilde{f}(Z)dZ$
-> Lokale Statistik von $Z$ sowie die Funktionen $Y_i(Z)$ und $T(Z)$ werden benötigt

# Modellierung turbulenter Vormischflammen
#Bray-Moss-Libby-Modell
Die Modellierung turbulenter Vormischflammen passiert anhand des **Bray-Moss-Libby-Modells**. Dabei wird die Fortschrittsvairable $c$ definiert:
$c=\frac{T-T_u}{T_b-T_u}$ oder $c=\frac{Y_P}{Y_{P,b}}$
Dabei ist $c=1$ im verbrannten und $c=0$ im unverbrannten. Zudem wird die Flammendicke als sehr dünn angenommen ($l_F <<\eta<<l_t$).

Wahrscheinlichkeitsdichtefunktion: $f(c)=\alpha\delta(c)+\beta\delta(1-c)$
- $\delta(c-c_o)= \{\infty \ für \ c=c_0,\ 0 \ sonst \}$
- $\int^\infty_{-\infty}\delta(c-c_0)dc=1$

- zur Schließung des BML-Modells: $\widetilde{u''c''}=\tilde{c}(1-\tilde{c})(\bar{u}_b-\bar{u}_u)$
- chemischer Quellterm: $\bar\omega_c=\rho_us_L^0I_0\Sigma$
	- $I_0$: Streckungsfaktor -> Lokale Brenngeschwindigkeitserhöhung durch Streckung
	- $\Sigma$: Flammenfläche pro Volumen (Flammenflächendichte)
