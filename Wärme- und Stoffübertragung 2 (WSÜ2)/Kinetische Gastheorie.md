In der kinetischen Gastheorie wird die Durchmischung zweier Gase beschrieben. Im Allgemeinen wird in der kinetischen Gastheorie das Verhalten idealer Gase ausschließlich über die Betrachtung der kinetischen Energie der Moleküle beschrieben.
# Grundlagen
## Ideale Gase
Annahmen:
- Energie eines Gases besteht ausschließlich aus der kinetischen Energie der Moleküle
- Moleküle mit Masse $m$ und Durchmesser $D$ in kontinuierlicher und zufälliger Bewegung
- Moleküle sehr klein im Verhältnis zur mittleren Weglänge
- Elastische Stöße sind die einzige zwischenmolekulare Wechselwirkung

Geschwindigkeit der Gasmoleküle:
$$
\begin{align}
\bar w&=\left(\frac{8k_BN_AT}{\pi M}\right)^{0.5}
\newline\newline
Mit:\bar w&=\sqrt{w_x^2+w_y^2+w_z^2}
\end{align}
$$
Da der Geschwindigkeitsbereich der Moleküle sehr groß ist und es durch Zusammenstöße zu einer ständigen Umverteilung kommt, wird ein Gas durch die Maxwell'sche Geschwindigkeitsverteilung beschrieben:
$$
p(w)=4\pi\left(\frac{M}{2\pi RT}\right)^{\frac 3 2}w^2e^{-\frac{Mw^2}{2RT}}
$$
## Reale Gase
Lennard-Jones Potential $\phi$:
$$
\phi(r)=4\epsilon\left[ \left( \frac \sigma r \right)^{12}-\left(\frac \sigma r \right)^6 \right]
$$
Das Potential zeigt:
- Abstoßung der Moleküle bei geringem Abstand
	- Reale Gase sind bei hohen Drücken schwerer zu komprimieren als ideale Gase
	- Realgasfaktor $Z>1$
- Anziehung der Moleküle untereinander bei größerem Abstand
	- Resultat: Kräfte, die eine Kompression bei mäßigem Druck begünstigen
	- Realgasfaktor $Z<1$
# Diffusion in Gasen
## Gedankenexperiment:
In einem abgeschlossenen Raum befinden sich die Moleküle A (links) und B (rechts). Diese sind zunächst getrennt voneinander, doch der Konzentrationsunterschied bewirkt Diffusionssträme der beiden Stoffe.

**Voraussetzungen**:
- Moleküle besitzen ähnliche Eigenschaften
- Moleküle bewegen sich mit der durchschnittlichen Geschwindigkeit $\bar w$

## Herleitung
Die Wahrscheinlichkeit, dass Moleküle A durch die Kontrollebene an der Stelle $x_0-l$ hindurchtreten ist höher, als dass sie durch die Kontrollebene an der Stelle $x_0+l$ treten, da die Anzahl an A-Molekülen links größer ist als rechts. Somit gilt für die Diffusion von A in x-Richtung:
$$
\begin{align}
j_A''&=\eta\cdot c_{ges}\frac{M_A}{N_A}\bar w\left[ \left.\frac{c_a}{c_{ges}}\right|_{x_0-l} - \left.\frac{c_a}{c_{ges}}\right|_{x_0+l} \right]
\newline\newline
Taylorentwicklung\ (linearisiert):
\left.j_A''\right|_{x=x_0}&=\eta\cdot n_{ges}\cdot\bar w\cdot\left[ -2l \left.\frac{d\frac{n_A}{n_{ges}}}{dx}\right|_{x_0} \right]
\newline\newline
Aus\ Vergleich\ mit\ Fick'schem\ Gesetz:D&=2\eta\cdot\bar w\cdot l

\end{align}
$$
## Berechnung von Diffusionskoeffizienten
Der Diffusionskoeffizient für binäre Systeme:
$$
D=2\eta\cdot\bar w\cdot l
$$Nach der kinetischen Gastheorie gilt:
$$
l = \frac{\bar w}{z}=\frac {Geschwindigkeit}{Stoßhäufigkeit}=\frac{k_BT}{\sqrt{2}\pi d_k^2 p}
$$
Daraus folgt somit:
$$
D=\frac{\left( \frac{k_b}{d^2} \right)^{1.5}}{d^2}\left( \frac{N_A}{M} \right)^{0.5}\frac{T^{1.5}}{p}
$$Da diese Formel weiterhin auf der kinetischen Gastheorie basiert und dementsprechend stark vereinfacht ist, gibt es die **Chapman-Enskog** Formel:
$$
D_{AB}=1,8583\cdot10^{-7}\frac{T^{1,5}}{p\Omega_D^{AB}(T)}\sqrt{\frac{1}{M_A}+\frac{1}{M_B}}
$$
Für Mehrstoffgemische muss ein anderer Ansatz gewählt werden. Dabei wird nur eine Komponente betrachtet und der Rest des Mehrstoffgemischs als einziges homogenes Gemisch. Dafür wird die Formel nach Stefan-Maxwell verwendet:
$$
\frac{\partial\psi_\alpha}{\partial z}=\sum^n_{\beta=1}\frac{c_\alpha c_\beta}{c^2D_{\alpha\beta}}\left( \frac{j_\alpha''}{\rho_\alpha} - \frac{j_\beta''}{\rho_\beta} \right)
$$
Für eine schwach konzentrierte Komponente $\alpha$ gilt:
$$
D_{\alpha m}=\left( \sum^n_{\beta=1;\beta\neq\alpha}\frac{\psi_\beta}{D_{\alpha\beta}} \right)^{-1}
$$
# Diffusion in Flüssigkeiten
Nach Einstein:
$$
D=\frac{k_BT}{6\pi\eta r}
$$
