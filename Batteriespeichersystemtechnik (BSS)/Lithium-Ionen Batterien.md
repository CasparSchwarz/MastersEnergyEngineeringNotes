Lithium ist ein attraktives Elektrodenmaterial, da es die höchste Spannung und spezifische Kapazität erzielen kann. Dementsprechend wird zur Zeit sehr viel in Lithium-Ionen Batterien investiert. Ebenso ist der Markt für Lithium-Ionen Batterien sehr groß (Fahrzeuge, Tragbare Geräte, Gartengeräte). Der größte weltweite Hersteller von Li-Ion Batterien ist zur Zeit CATL (ca. 36 % Marktanteil).

# Klassifizierung
Li-Io Batterien werden nach Anodenmaterial und Elektrolyt unterschieden:
- Lithium-Basiert
	- Lithium-Ion
		- Anode: Graphit
		- Kathode
			- NMC (Nickel, Mangan, Cobalt)
			- LCA (Lithium, Cobalt, Aluminium)
			- LMO (Lithium, Mangan, Sauerstoff)
			- LFP (Lithium, Eisen, Phosphor)
			- LFMP (Lithium, Eisen, Mangan, Phosphor)
	- Lithium-Ion
		- Kathode: Verschiedene
		- Anode
			- Si (Kohlenstoff-Silizium Mischung)
			- LTO (Lithium, Titan)

# Funktionsweise
Lithium-Ionen sind Lithium Atome, denen ein Elektron fehlt und somit positiv geladen sind. Die Lithium-Atome geben dabei an der Anode Elektronen ab und die Ionen wandern durch das Elektrolyt zu der Kathode.

Die Anode besteht dabei im Regelfall aus Graphit, wobei auf ein Lithium-Atom 6 Grpahit Atome kommen. Somit existiert in einer Lithium-Ionen Batterie niemals metallisches Lithium, da die einzelnen Atome nicht mit einander zu einem Metall verbunden sind.

Während des Ladens wird das Lithium aus dem Kathodenmaterial herausgelöst. Dabei kann nur maximal 70 % des Lithiums herausgelöst werden, da das Kathodenmaterial sonst instabil wird.
$$
\begin{align}
Laden&:\ LiNi_xMn_yCo_zO_2\rightarrow Li_{1-w}Ni_xMn_yCo_zO_2+w\ Li^++w\ e^-
\newline\newline
Entladen&:\ LiNi_xMn_yCo_zO_2\leftarrow Li_{1-w}Ni_xMn_yCo_zO_2+w\ Li^++w\ e^-
\newline\newline
Mit&:\ (0\leq w\leq 0,7\ /\ x+y+z=1)
\end{align}
$$
![[SmartSelect_20240506_093354_Drive.jpg]]
# Verwendete Materialien
## Elektrolyten
Als Elektrolyt können flüssige oder feste Elektrolyte verwendet werden. Zu den flüssigen zählen unter anderem basische und sauer Lösungen. Diese haben eine hohe Leitfähigkeit, erzeugen jedoch während des Ladevorgangs Wasserstoff, was ein erhöhtes Sicherheitsrisiko zur Folge hat.

Sicherer sind Polymmerelektrolyte, die aus einer Membran bestehen. Diese haben jedoch eine deutlich niedrigere Leitfähigkeit als flüssige Elektrolyte und müssen dementsprechend sehr sehr dünn sein (<< 50 µm).
## Anoden & Kathoden

| Kathodenmaterial                | Vorteile                                        | Nachteile                                        |
| ------------------------------- | ----------------------------------------------- | ------------------------------------------------ |
| $LiCoO_2$                       | Gute Lebensdauer                                | Hohes Sicherheitsrisiko, geringe Vollzykleenzahl |
| $LiNiO_2$                       | Gute Performance                                | Höchstes Sicherheitsrisiko                       |
| $LiMn_2O_4$                     | Sicherheit beesser als Co & Ni                  | Schlechtere Lebensdauer                          |
| $LiCo_{1/3}Ni_{1/3}Mn_{1/3}O_2$ | Populär und große Spezialisierungsmöglichkeiten |                                                  |
| $LiCo_xNi_yMn_2Al_wO_2$         | Große Variabilität in Mischmaterialien          |                                                  |
| $LiFePO_4$                      | Günstiges und sicheres Ausgangsmaterial         |                                                  |

| Anodenmaterial           | Spannung | Eigenschaften                                                                           |
| ------------------------ | -------- | --------------------------------------------------------------------------------------- |
| Hard Carbon $LiC_6$      | 3,7 V    | Geringe Vollzyklenzahl                                                                  |
| Graphit $LiC_6$          | 3,7 V    | Teuer, hohe Vollzyklenzahl                                                              |
| Titanat $Li_4Ti_5O_{12}$ | 2,2 V    | sicher (kaum Volumenänderung), geringere Energiedichte, hohe Leistung, hohe Lebensdauer |
| Silizium $Li_{22}Si_6$   | 3,7 V    | hohe Energiedichte, in der Forschung                                                    |

## Alterung
### Solid Electrolyte Interface
An der Fläche zwischen Graphit und Elektrolyt reagieren beide Stoffe miteinander und es entsteht eine Passivschicht (Solid Electrolyte Interface). In dieser Passivschicht werden Ionen gefangen und deren Durchtritt erschwert. Umso mehr Ionen gefangen werden, desto geringer wird die Kapazität und umso größer die Schicht desto schlechter die Leistungsfähigkeit.

Bei vollständiger Ladung und Entladung der Batterie, verändert das Graphit das Volumen so stark, dass die Passivschicht reißt und somit einen neuen Kontakt zwischen Graphit und Elektrolyt herstellt. Dadurch wird das Wachstum der Passivschicht erhöht.

Best use:
- Flache Ladezyklen (Nur wenige 10 % laden)
- Tiefer Ladezustand (geringeres Potenzial) besser als hohes Potenzial
- Immer Aufladen wenn die Chance besteht -> Ladzyklen flach halten
- Zeit bei maximalem Ladezustand gering halten (Bei Auto direkt nach Volladen losfahren)

### Li-Plating
Bei Lithium-Plating flockt metallisches Lithium an der Anode aus, wenn das Potenzial der Anode unterhalb des Potenzials von metallischem Lithium (0 V) liegt. Hauptsächlich geschieht dies bei:
- niedrigen Temperaturen und
- hohen Stromstärken

## Solid-State Elektrolyte
Festkörperbatterien benutzen als Elektrolyt etwa Kunststoffe (Polymere) oder Keramiken. Der Hauptunterschied zu Li-Io-Batterien mit flüssigem Elektrolyt ist, dass **kein Graphit** als Anode verwendet wird sondern **metallisches Lithium**.

**Probleme**:
- Sicherheit: Metallisches Lithium ist sehr reaktiv
- Lebensdauer
	- Zyklisierung von metallischem Lithium ist nicht 100 % reversibel
	- ca. 4-facher Überschuss an Lithium notwendig
	- Dendritenbildung
	- Zyklenzahlen bei flüssigem Elektrolyt weniger als 100 Zyklen
- Sehr schlechte spezifische Leitfähigkeit (Elektrolyt muss sehr dünn sein)
- Bisher nur für 50 °C - 60 °C

# Anwendungsbereiche
## Lithium-Metall
- Flüssig: Nur für Knopfzellen
- Polymer / Festkörper: erlangt mehr Aufmerksamkeit

Nachteil:
- Formierung von Dendriten beim Laden
- Hochreaktiv -> gefährlich

## Litium-Ionen
- Flüssig: Einsatz in EV & HEV (Höchster Marktanteil)
- Polymer: Betrieb bei höheren Temperaturen und geringerer Leistung
	- Hohe Temperaturen
	- Schlechte Leitfähigkeit

# Gehäusetypen
![[SmartSelect_20240513_092921_Drive.jpg]]
Zylindrische Zelle
- 18 mm - 45 mm Durchmesser
- 65 mm - 80 mm Länge
- Begrenzt in der dichtesten Packung
- Luftraum wirkt Wärmeisolierend (höhere Sicherheit)
- Zylindrische Form nimmt Drücke deutlich besser auf als andere Zellenformen

Pouch-bag Zelle
- Lassen sich dichter Packen als zylindrische Zellen
- Nur Folie, kein festes Gehäuse
- Sehr gute Kühlungseigenschaften (große Overfläche)

Prismatische Zelle
- Festes Gehäuse
- Hohe volumetrische Energiedichte
- Mussen mit Druck beaufschlagt werden, damit sich die Zelle nicht so stark verformt
- Brauchen Schichten zwischen den Zellen zur Wärmeisolation

# Hochleistungs- und Hochenergiebatterien
![[SmartSelect_20240513_094143_Drive.jpg]]
Bei hohen Leistungen werden mehr Schichten verwendet, wodurch die Menge an Passivmaterialien zunimmt. Somit kann weniger Energie in Aktivmaterialien gespeichert werden.

**Beachte**: Bei hohen Entladeströmen erwärmt sich die Batterie -> Erhöhte Kapazität aufgrund der Temperaturänderung
**Aber**: Bei niedrigen Temperaturen und hohen Strömen fällt die Spannung anfangs sehr stark ab -> System denkt, dass die Batterie leer ist, da die Spannung so stark abgefallen ist
# Batteriesicherheit
Die Batteriespannung muss immer im Bereich des normalen Betriebs zwischen ca. 2,5 V und 4,5 V betrieben werden:
![[Pasted image 20240527084712.png]]

Erhöhung der passiven Sicherheit:
- Verbesserte Überdruckventile bzw Sollbruchstelen
- Verwendung von keramischen Separatoren
- LiFePO4 als inhärent sicheres Material

Aktive Sicherheit:
- Spannugnsüberwachung jeder einzelnen Zelle
- Genaues Lade- und Entlademanagement
- Temperaturüberwachung und Kühlkonzepte

## Thermal runaway
Durch Überladung kann es zu einem thermal runaway kommen. Dabei initiiert der Temperaturanstieg durch Überladung oder eine externe Wärmequelle eine **exotherme Reaktion**, welche sich selbst immer weiter beschleunigt. Dadurch Zerfällt die Aktivmasse und es kann zum Brand kommen.
# Lade- und Entladekurven
Eine typische Lade- und Entladekurve sieht wie folgt aus:
![[Pasted image 20240527090617.png]]
## Lithium Plating
Bei tiefen Temperaturen, hohen Strömen und bei Überladung.
Beispiel:
- Kleine Diffusionskoeffizienten
- Hohe Konzentrationen in äußeren Partikel Schalen
- Tiefes lokales Potential
- Lithium Plating

![[Pasted image 20240527091407.png]]
## Batteriemanagement
Bei neuen Batterien haben alle Zellen einen einheitlichen SOC. Mit der Zeit können die Zellen jedoch ungleich altern, sodass einzelne Zellen in einen thermal runaway geraten können, obwohl andere Zelle noch nicht ihren maximalen Ladungszustand erreicht haben. Dementsprechend wird ein Ladungsausgleich benötigt, um alle Zellen auf einen einheitlichen SOC zu bringen.
# Rohmaterialbedarf und Verfügbarkeit
Der Preis einer Batteriezelle setzt sich wie folgt zusammen:
![[Pasted image 20240527092354.png]]

|           | Batteriezelle<br>100 Ah/ 3,8 V | Batteriepack<br>100 kWh |
| --------- | ------------------------------ | ----------------------- |
| Nickel    | 325 g                          | 85,5 kg                 |
| Mangan    | 37 g                           | 9,7 kg                  |
| Kobalt    | 41 g                           | 11,1 kg                 |
| Lithium   | 35 g                           | 9,2 kg                  |
| Aluminium | 144 g                          | 37,9 kg                 |
| Kupfer    | 281 g                          | 73,9 kg                 |
# Alterungsprozesse
Die Alterung von Batterien wird vom Ladezustand und den äußeren Bedingungen bestimmt. Dabei muss immer zwischen Nutzbarkeit und Langlebigkeit abgewägt werden:
- Bei niedrigem SOC kann die Lebensdauer deutlich erhöht werden (Faktor 2 bis 3)
- Bei niedrigem SOC ist die Nutzbarkeit gering
- Bei hohem SOC sinkt die Lebensdauer deutlich (wenn bspw. Laptop immer vollgeladen)
- Bei hohem SOC wird die höchste Nutzbarkeit bereitgestellt

- Lösungsmittel Co-Interkalation / Abblättern von Graphit / Cracking
	- -> Kapazitätsverlust
	- Beschleunigt durch Überladen
- Elektrolyt Zersetzung
	- -> Kapazitätverlust, Leistungsverlust
	- Beschleunigt durch hohe Temperatur und hoher Ladezustand
- SEI Wachstum
	- -> Erhöhung der Impedanz und Leistungsverlust
	- Beschleunigt durch: hohe Stromraten, hohen Zyklentiefen
- Verringerung der aktiven Oberfläche
	- -> Erhöhung der Impedanz und Leistungsverlust
	- Beschleunigt durhc hohe Temperatur und hoher Ladezustand
- Abscheidung von metallischem Lithium
	- -> Kapazitätsverlust, Leistungsverlust
	- Beschleunigt durch niedrige Temperaut, hohe Stromraten, schlechtes Zelldesign
- Kontaktverlsut der Aktivmassenpartikel wegen Volumenänderung
	- -> Kapazitätsverlust
	- Beschleunigt durch hohe Stromraten, hohe Zyklentiefe
- Korrosion des Ableiters
	- -> Leistungsverlust und Erhöhung der Impedanz
	- Beschleunigt durch niedriger SOC, Tiefentladung

## Alterung an der Anode
- Abblättern von Graphit, Cracking
- Zersetzung des Elektrolyten
- SEI Wachstum
- SEI Kovnertierung/ Stabilisierung/ Wachstum
- SEI Auflösung / Ablagerung
- Positive / Negative Wechselwirkung
- Ablagerung von metallischem Lithium (Plating)
- Dendritenbildung
- Bildung neuer Oberfläche zur SEI-Bildung -> beschleunigte Alterung

## Alterung an der Kathode
- Mikro-Cracking
- Gasung
- Elektrolytzersetzung
- Ausbildung einer Oberflächenschicht
- Ablagerung neuer Phasen
- Kontaktverlust zu leitenden Partikeln
- Korrosion des Ableiters
- Oxidation der leitenden Partikel
- Zersetzung des Binders

# Lebensdauertests
Es gibt zwei grundsätzliche Arten von Alterungstests:
- Kalendarische Alterung (vor allem Standzeiten)
- Zyklentests (Betrieb des Speichers)

Für die Lebensdauerbeschreibung ist die Wöhlerkurve von großer Bedeutung. Sie gibt die Anzahl an Zyklen an, die bei einer Entladetiefe erreicht werden können. Die rote Kurve ist dabei das Produkt aus Zyklen und Entladetiefe und zeigt somit die effektiv entnommene Energie an.
![[Pasted image 20240527100830.png]]

In den Tests ist zu beachten, dass es sehr schwierig ist, alle Zellen einer Batterie in allen Betriebspunkten zu testen. Das führt dazu, dass statistische insignifikante Ergebnisse durch unzureichende Stichprobengrößen erzeugt werden.

Temperatur hat einen signifikanten Einfluss auf die Alterung von Batterien. Ebenso auch der SOC und der DOD. Jedoch ist die geringe Zyklentiefe von geringem Einfluss auf die Alterung.

Bei der Entladung hat die Entladestromstärke keinen Einfluss auf die Alterung der Batterie.

Im realen Betrieb können über 4.000 äquivalente Vollzyklen erreicht werden. Bei kleinen Zyklentiefen deutlich mehr als 5.000