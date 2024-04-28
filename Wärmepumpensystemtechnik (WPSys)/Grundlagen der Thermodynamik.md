## Hauptsätze der Thermodynamik
- Erster Hauptsatz: $\sum\limits_i^nQ_i+\sum\limits_i^nP_i=0$
- Zweiter Hauptsatz: $\sum\limits_i^n\dot{S}+\sum\limits_i^n\frac{\dot{Q}_i}{T_i}+\sum\limits_i^n\dot{S}_{irr}=0$
- Leistungszahl: $COP=\frac{\dot{Q}_{ab}}{P_{el}}=\frac{\dot{Q}_{ab}}{\dot{Q}_{ab}-\dot{Q}_{zu}}$ 
- Carnot-Leistungszahl: $COP_{Carnot}=\frac{T}{T-T_u}$
- Gütegrad: $\eta_{Carnot}=\frac{COP}{COP_{Carnot}}$
- Isentroper Verdichterwirkungsgrad: $\eta_{is,V}=\frac{vdp}{vdp+Tds}$
- Volumetrische Heizenergie: $VHC=\frac{\dot{Q}_{ab}}{\dot{V}_{Verdichter, ein}}$
## Kältemittel
In Wärmepumpen werden Kältemittel verwendet. Es wird unterschieden zwischen nassen und trockenen Kältemitteln.
- Nasse Kältemittel: positive Steigung der Sattdampfkurve
- trockene Kältemittel: negative Steigung der Sattdampfkurve
Die Begriffe nass und kalt beziehen sich auf die Möglichkeit, dass ein gerade vollständig verdampftes Kältemittel bei Kompression auskondensiert. Kondensiert das Kältemittel bei Kompression ist das Kältemittel nass, sonst trocken.
Beispiel eines nassen Kältemittels:
![[Pasted image 20231027101131.png]]
In einem Verdichter darf es nicht zu einem Tropfenschlag durch Kondensation kommen. Dementsprechend wird das Kältemittel aus Sicherheitsgründen überhitzt. Die Überhitzung kann über ein variables Expansionsventil gesteuert werden. Ist die Überhitzung zu gering, wird auf einen niedrigeren Druck expandiert. Ist die Überhitzung zu hoch, wird auf einen höheren Druck expandiert.

Um das Expansionsventil zu schützen, wird im Kondensator das Kältemittel unterkühlt. Ebenso wird damit die nutzbare Wärmemenge erhöht.

### Klassifikation von Kältemitteln
Nach **ASHRAE 34**
- Giftigkeit
	- **A** Geringe Giftigkeit
	- **B** Größere Giftigkeit
- Flammbarkeit
	- **1** Keine Flammenausbreitung
	- **2** Geringe Brennbarkeit
	- **2L** Geringe Brennbarkeit bei geringer Flammenausbreitungsgeschwindigkeit
	- **3** Größere Brennbarkeit

### Namenskonvention
#### Organische Reinstoffe
**Rwxyzbb**
- **R**: Refrigerant
- **w** Anzahl Doppelbindungen
- **x**: x=c-1
- **y**: y=h+1
- **z**: z=f
- **bb**: Angehängte Buchstaben
- **cl**: Anzahl der restlichen Bindungen
-> Summenformel: $C_cH_hF_fCl_{Cl}$

#### Gemische
- R 400er (zeotrop)
- R 500er (azeotrop)
- zeotrop: Temperaturgleit; Gemischpartner Sieden bei unterschiedlichen Temperaturen / Drücken
- azeotrop: Kein Temperaturgleit; Gemischpartner Seiden bei der gleichen Temperatur; aka Schnittpunkt von Siede- und Taukurve

#### Anorganische Reinstoffe
R 7xx mit xx: ganzzahlig gerundete Molmasse