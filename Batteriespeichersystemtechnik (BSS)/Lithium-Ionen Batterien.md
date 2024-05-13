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