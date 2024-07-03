Ein Prallstrahl entsteht, wenn ein Flüssigkeitsstrahl auf eine Ebene trifft. Prallstrahlen werden dabei über ein Rohr und eine Düse hergestellt und für verschiedene Einsatzzwecke angewendet:
- Kühlen
- Schneiden
- Trocknen
- Reinigen

Die Auswahl eines geeigneten Prallstrahls ist dabei abhängig von der erreichten Nusseltzahl. Diese hängt bei Prallstrahlen von der Reynoldszahl und der Prandtlzahl ab.

Es gibt einphasige und zweiphasige Prallstrahlen. Bei einphasigen Prallstrahlen wird der Freistrahl mit zunehmnder Länge dicker. Bei zweiphasigen Prallstrahlen 
# Zonen eines Prallstrahls
Ein Prallstrahl wird in 6 Zonen unterteilt:
- Freistrahl
- Stauzone
- Blasius Grenzschichtbereich
- Watson Ähnlichkeitsgebiet
- Sprungbereich
- Stromabwärts

![[Pasted image 20240703143749.png]]
# Wärmeübertragung bei Prallstrahlen
Um den Wärmeübergang eines Prallstrahls zu bestimmen muss zunächst das Geschwindigkeitsfeld des Prallstrahls beschrieben werden.
## Geschwindigkeitsfeld bei Prallstrahlen
Das Geschwindigkeitsfeld bei Prallstrahlen ist für die unterschiedlichen Bereiche des Prallstrahls zu definieren (siehe oben).
![[SmartSelect_20240703_160854_Drive.jpg]]
### Freistrahl
Im Freistrahl ist bei Düsenaustritt ein parabolisches Geschwindigkeitsprofil vorhanden, welches durch den Einfluss der Gravitation in ein homogenes Geschwindigkeitsprofil übergeht. Durch die Erdbeschleunigung steigt die Geschwindigkeit des Mediums im Freistrahl, wodurch sich der Querschnitt des Freistrahls verringert. Im Freistrahl dominieren viskose Kräfte und Trägheitskräfte.

Beim Übergang zur Stauzone sind Zähigkeitskräfte (viskose Kräfte) und Kräfte aufgrund von Druckgradienten gleich groß.
### Stauzone
Die Stauzone liegt am Ende des Freistrahls direkt über der Bodenplatte. Aufgrund des hohen Drucks in der Stauzone wird die axiale Freistrahlströmung in radiale Richtung abgelenkt. Im Regelfall ist die Breite der Stauzone in der Größenordnung des Düsendurchmessers.

In der Stauzone dominieren Kräfte durch Druckgradienten.
### Grenzschichtbereich
An die Stauzone schließt der Blasius Grenzschichtbereich an. In diesem wächst die Grenzschichtdicke $\delta_v$ bis zur Strömungshöhe an. Bei Düsendurchmesser $D$ liegt der Blasius Grenzschichtbereich im Bereich:
$$
\mathcal{O}(D/2)=r_S\leq r < r_v=0,1773\cdot D\cdot Re_D^{1/3}
$$
### Watsons Ähnlichkeitsgebiet
Das Watson Ähnlichkeitsgebiet beginnt dort, wo die Grenzschichtdicke die Strömungshöhe erreicht hat und Endet beim hydraulischen Sprung, oder bei Umgehen eines Hindernisses.
$$
r_v\leq r_j=1,046\cdot \left[ \frac{\sigma\dot V^2}{8\pi^2\nu^2g\rho} \left( -1+\sqrt{1+\frac 2\pi \frac{\dot V\nu g \rho^2}{\sigma^2}} \right) \right]^{1/4}
$$
Mit $\sigma$ als Oberflächenspannung

Die Bedingung für den hydraulischen Sprung ist der Übergang von einer überkritischen in eine unterkritische Strömung. Dabei ist die Strömungsgeschwindigkeit gleich der Wellenausbreitungsgeschwindigkeit.
### Sprungbereich
Die Stärke des Sprunges hängt vor allem von der Hindernishöhe ab. Je nachdem wie stark der Sprung ist, entstehen unterschiedliche Strukturen im Sprungbereich.
## Bestimmung des Wärmeübergangs
In WSÜII ist vor allem der Wärmeübergang in den Bereichen der Stauzone, im Grenzschichtbereich und im Watson Ähnlichkeitsgebiet von Bedeutung. Die größte Nusseltzahl wird dabei in der Stauzone erreicht, wobei diese rapide im Grenzschichtbereich und Watson Ähnlichkeitsbereich abnimmt.
![[SmartSelect_20240703_162342_Drive.jpg]]
Der höchste Wärmeübertrag wird aufgrund des Einflusses der Fläche im Ähnlichkeitsbereich erreicht.
### Stauzone
Unter der Annahme einer **laminaren Grenzschicht**:
$$
\begin{align}
Nu_D&=\frac{\alpha D}{\lambda}=G(Pr)Re_D^{1/2}\sqrt{B} \\\\
Mit:\ B&=2\frac{D}{u_f}\frac{du_e}{dr}\\\\
G(Pr)&=\frac{\sqrt{2Pr/\pi}}{1+0,805\sqrt{2Pr/\pi}}\text{ Für Pr}\leq0,15 \\\\
G(Pr)&=0,539Pr^{2/5}\text{ Für }0,15<Pr<3,0 \\\\
G(Pr)&=0,60105Pr^{1/3}-0,050848\text{ Für }Pr\geq 3
\end{align}
$$

### Das Temperaturfeld in Prallstrahlen
Wenn die Prandtlzahl kleiner-gleich 1: Temperaturgrenzschichtdicke < Geschwindigkeitsgrenzschichtdicke

Wenn die Prandtlzahl größer 1: Temperaturgrenzschichtdicke > Geschwindigkeitsgrenzschichtdicke

Zur Beschreibung des Temperaturfeldes werden folgende Annahmen getroffen:
- Inkompressibel
- 2D
- Reibungsbehaftet
- Stationär

