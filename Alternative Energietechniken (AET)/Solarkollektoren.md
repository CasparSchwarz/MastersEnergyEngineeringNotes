Unter Solarkollektoren werden Solarmodule verstanden, die solare Strahlung in Wärme umwandeln.
# Physikalische Grundlagen
Die solare Strahlung setzt sich aus direkter Strahlung und diffuser Strahlung zusammen. Die Summe aus beiden bildet die Globalstrahlung:
$$
G=G_{dir}+G_{dif}
$$

Die Position der Sonne wird mit zwei Winkeln beschrieben:
- $\gamma_S$: Sonnenhöhe
- $\alpha_S$: Sonnenazimut

Gleichzeitig wird die Ausrichtung des Kollektors über zwei weitere Winkel beschrieben:
- $\beta$: Neigung der Fläche
- $\alpha$: Azimut der Fläche

Der **Air-Mass-Faktor** AM gibt die Weglänge der Sonnenstrahlen durch die Atmosphäre in Abhängigkeit des Sonnenhöhenwinkels. Mit dem AM erhöht sich die Absorptionsrate, da mehr Luft gestreut und absorbiert werden kann.
$$
AM\approx \frac{1}{sin(\gamma+5°)}
$$

In der Atmosphäre kommt es zu verschiedenen Streuungs- und Absorptionseffekten, welche die einfallende Sonnenstrahlung abschwächen:
- **Rayleigh-Streuung**: Streuung an Molekülen, die kleiner als die Licht-Wellenlänge sind. Durch die Wellenlängenabhängigkeit wird blaues Licht stärker gestreut als rotes
- **Mie-Streuung**: Streuung an Molekülen, welche größer als die Licht-Wellenlänge sind
- **Gasabsorption**: Einzelne Gase absorbieren unterschiedliche Wellenlängenbänder und erzeugen eindeutige Linien im Spektrum verantwortlich

Die Interaktion von Strahlung mit Materie wird über verschiedene Faktoren beschrieben:
- $\rho$: Reflexionsgrad
- $\alpha$: Absorptionsgrad
- $\tau$: Transmissionsgrad
- $\varepsilon$: Emissionsgrad

Eine Oberfläche emittiert Strahlung proportional der 4. Potenz ihrerer absoluten Temperatur:
$$
\dot q''=\varepsilon\cdot\sigma\cdot T^4
$$
Unterschiedliche Oberflächen haben unterschiedliche Absorptions- und Emissionsgrade. Um einen geeigneten Absorber zu konstruieren wird ein Kupferblech entweder mit Lacken oder speziellen Materialien beschichtet.
![[Pasted image 20240614090310.png]]
Dabei zeigt Schwarzchrom einen interessanten Effekt, da der Emissionsgrad deutlich niedriger als der Absorptionsgrad ist. Dies wird durch die hohe Rauigkeit der Oberfläche erzielt, wodurch ein Großteil der emittierten Strahlung wieder vom Material absorbiert wird.
# Kollektorarten
Bei der Auslegung eines Solarkollektors muss beachtet werden, dass der Kollektorkreislauf die hohen Drücke bei Auftreten von Sieden aufnehmen kann. Dafür wird ein Ausdehngefäß zum Druckausgleich verwendet.
## Flachkollektor
Ein Flachkollektor besteht aus einer transparenten Abdeckung, einem Absorber und einem Flüssigkeitskanal.
![[Pasted image 20240614090910.png]]
## Vakuumröhrenkollektor
In Vakuumröhrenkollektoren sitzt der Kollektor in einer evakuierten Röhre, sodass minimale Konvektion auftritt und Wärmeverluste auf Strahlung beschränkt werden. 

Das Problem bei Vakuumröhrenkollektoren ist, dass diese für die gesamte Lebenszeit dicht sein müssen. Durch den realen Betrieb kommt es zu Ausdehnung und Zusammenziehen des Materials auf Grund von Temperaturunterschieden. Zudem sind die Dichtungen permanenter Sonnenstrahlung ausgesetzt. Dadurch kommt nach einiger Zeit Luft in die Vakuumröhre, sodass die Wärmeverluste steigen.
# Kennzahlen von Solarkollektoren
Wirkungsgrad:
$$
\eta=\frac{\dot q_N''}{G}=\frac{G\cdot\tau\alpha-k_{eff}\cdot\Delta T}{G}=\eta_0-\frac{k_{eff}\cdot\Delta T}{G}
$$
Optischer Wirkungsgrad:
$$
\eta_0=\tau\cdot\alpha
$$
Nutzbare Einstrahlung:
$$
G_N=G\cdot\tau\cdot\alpha
$$
Nutzwärmeleistung:
$$
\dot q_N''=G_N-\dot q_V''
$$
Effektiver Wärmeverlust:
$$
k_{eff}=c_1+c_2(t_m-t_a)
$$
Kennliniengleichung:
$$
\eta=\eta_0-\frac{c_1\cdot\Delta T}{G}-\frac{c_2\cdot\Delta T^2}{G}
$$
# Alternative Konzepte
PV/T-Hybridkollektor:
- Kombination aus Solarthermie und PV
- Vorteil: Kühlung der PV-Module erhöht den Wirkungsgrad -> Geeignet für Niedertemperatursysteme

Photobioreaktor:
- Kombination aus Biomasse- und Wasserstofferzeugung

