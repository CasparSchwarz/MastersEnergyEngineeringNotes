WKA benötigen Wind um elektrische Energie zu erzeugen. Dabei wird die Energie des Windes in mechanische Energie umgewandelt. Demnach ist eine genaue Standortanalyse und eine Auslegung der Anlage notwendig, damit Laufzeiten von mehr als 20 Jahren der WKA erreicht werden können. Bei der Standortanalyse sind dabei Gelände (Rauigkeit, Hindernisse) und der Wind (Geschwindigkeit, Turbulenzen) wichtig. Bei der Auslegung der Anlage sind Rotorleistung, der mechanische Wirkungsgrad und Störungen zu beachten.

**Theoretische elektrische Leistung**: $P_{el} = c_p \frac{\rho}{2} A_{Rotor}{V_w}³$

## Ursaches des Winds
- Sonne: 2% der Sonneneinstrahlung werden in Windenergie umgewandlet (3,4*10^12 kW)
- inhomogene Erdoberfläche
- Dichte- und Temperaturgradienten: **Druckgradientenkraft**
- Corioliskraft

### Druckgradientenkraft
Es wird ein kleines Raumvolumen betrachtet:
$m=A\cdot\Delta x\cdot\rho$
$F_p=F_1-F_2=-\Delta p \cdot A$
$F_p=-\frac{m}{\rho}\cdot\frac{\Delta p}{\Delta x}$

### Corioliskraft
Die Coriolistkraft entsteht durch die Drehung der Erde und die unterschiedlichen Geschwindigkeiten auf den Breitengraden. Somit behält ein bewegtes Volumen die Geschwindigkeit in Tangentialrichtung nach dem initialen Impuls. In einem mitbewegten Koordinatensystem (Beachter auf der Erdoberfläche) scheint das Volumen in tangentialer Richtung beschleunigt zu werden. Diese Beschleunigung ist die Coriolisbeschleunigung und resultiert in der Corioliskraft.

Die Corioliskraft berechnet sich wie folgt:
$\vec{F}_c=2\cdot m(\vec{v}\times\vec{\omega})$
Auf der Erde gilt
$\overrightarrow{\omega}=(0, \omega cos(\varphi), \omega sin(\varphi))^T$
Und somit:
$F_c = \sqrt{F_x^2+F_y^2}=2m\omega sin(\varphi)\sqrt{v_{ns}^2+v_{ow}^2}$
$ns: Nord-Süd$
$ow: Ost-West$
$F_c=2\cdot m\cdot v\cdot\omega sin(\varphi)$

## Geostrophischer Wind
Geostrophischer Wind ist das Resultat aus dem Kräftegleichgewicht von Druckgradientenkraft und Coriolistkraft. Dabei Steigt die Coriolistkraft mit dem Breitengrad. In realen Systemen wird die Corioliskraft zusätzlich mit der Reibungskraft überlagert, sodass die dem Druckgradienten entgegnende Kraft aus Reibung und Corioliskraft besteht.

## Lokale Windverhältnisse
Durch die Reibbedingung am Boden entsteht eine bodennahe Grenzschicht. Dabei nimmt die Turbulenz mit der Höhe ab.

Universelle Wandgesetz für turbulente Strömungen:
$\frac{\bar{u}}{u_x}=\frac{1}{\kappa}ln(\frac{zu_*}{\mu})+C$
Wobei
$u_*=\sqrt{\frac{\tau_w}{\rho}}$

Logartihmisches Windprofil
$v(z)=v_{ref}\frac{ln(\frac{z}{z_0})}{ln(\frac{z_{ref}}{z_0})}$

Turbulenz & Böen
$v(z)=\bar{v}+v'(t)$
