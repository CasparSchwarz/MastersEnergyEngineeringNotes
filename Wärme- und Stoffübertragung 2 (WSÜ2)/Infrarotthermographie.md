Infrarotthermographie ist ein nicht-invasives Verfahren zur Temperaturmessung und wird heutzutage in vielen Gebieten verwendet (z.B. Forschung, Gebäudesanierung, Prozessüberwachung).

# Grundlagen
Infrarotstrahlung ist nach DIN 5031 Teil 7 der Teil des elektromagnetischen Spektrums mit einer Wellenlänge zwischen 0,78 µm und 1 mm. Dabei wird der Bereich meist in
- nahes,
- kurzwelliges,
- mittelwelliges,
- langwelliges und
- fernes Infrarot unterteilt.

![[Pasted image 20240424171025.png]]

Bei der Messungen kommen drei Strahlungsbänder zum Einsatz, das
- kurz-
- mittel-
- lang-
wellige Band.

Die Wahl des jeweiligen Messbands hängt vom erwarteten Temperaturniveau ab.

Das Plancksche Verteilugnsgesetz beschreibt die spektrale Strahlungsstromdichte eines **schwarzen** Körpers:
$$
\dot{q}^{''}_{s\lambda}=\frac{c_1\lambda^{-5}}{exp[c_2/(\lambda T)]-1}
$$

# Strahlung realer Oberflächen
Reale Flächen sind im Allgemeinen nicht schwarz, dementsprechend müssen Emissions-, Transmissions-, und Reflektionsgrad müssen berücksichtigt werden. Diese sind im Allgemeinen abhängig von der Wellenlänge:
$$
\varepsilon(\lambda)=\frac{\dot q^{''}_{\lambda, Real}(T)}{\dot q_{\lambda,schwarz}(T)} \ mit\ 0\leq\varepsilon\leq1
$$
Ebenfalls sind Emissions-, Transmissions- und Reflektionsgrad von dem Blickwinkel abhängig:![[Pasted image 20240424173103.png]]

Bei der Infrarotthermographie wird die gesamte von einer Fläche ausgehende Strahlung (Oberflächenhelligkeit) detektiert:
$$
\dot{Q}_{Oberfläche}=\dot{Q}_\epsilon+\dot Q_\tau+\dot Q_\rho
$$
Im Regelfall enthält nur einer dieser Anteile die Information über die Temperatur der Fläche.

# Messverfahren
Die Strahlung wird durch einen Detektor gemessen, welcher diese in elektrische Signale umwandlet. Die elektrischen Signale können in einem Rechner weiterverarbeitet werden, sodass daraus ein Bild entsteht.

Die Detektoren können entweder
- thermische Deketoren oder
- Photodetektoren
sein.
Ein thermischer Detektor (Mikrobolometer) nutzt die Temperaturabhängigkeit eines elektrischen Widerstandes aus. Ein Photodetektor (Quantendetektor) nutzt den photoelektrischen Effekt aus.

Der Deketor sollte dementsprechend nach dem Einsatzzweck ausgewählt werden:
- stationär & geringe Genauigkeit -> Mikrolobolometer

Bei der Signalverarbeitung wird eine bestimmte Menge an Energie vom Detektor aufgenommen. Das erreichte Energieniveau wird in ein digitales Level (DL) umgewandelt.