Turbulente Flammen sind durch eine turbulente Mischung charakterisiert. Die Turbulenz verstärkt die molekulare Vermischung und beschleunigt somit die Verbrennung.

Hier ist links der Prozess der Verbrennung mit der turbulenten Vermischung zu sehen und rechts die daraus folgende Verbrennungscharakteristik.
![[Pasted image 20231220085659.png]]

Aus Beobachtung bekannt: laminare Strömung wird turbulent
- Durch-/umströmten Körper vergrößern
- Strömungsgeschwindigkeit erhöhen
- Weniger zähes Fluid
Die Turbulenz kann über die Reynoldszahl bestimmt werden:
$Re=\frac{ud}{\nu}$

Zur konkreten Beschreibung werden Methoden der Statistik und Stochastik verwendet (siehe [[Statistische Beschreibung turbulenter Verbrennung]])
# Mathematische Beschreibung
Turbulente Strömungen sind instationär, Wirbelbehaftet und stochastisch. Turbulente Strömungen können in über die mittlere Geschwindigkeit und den Schwankungsanteil beschrieben werden. Diese Aufspaltung wird Reynolds-Zerlegung genannt.

## Reynolds-Zerlegung
Aufspaltung der Geschwindigkeit in Mittelwert und Schwankungsanteil
$u_i=\bar{u}_i+u_i'$

![[Pasted image 20231220092516.png]]

## Mittelwertbildung
Im Mittel **instationär** -> Ensemble-Mittelwert
$\bar{u}_i(x,y,z,t)=\lim_{N\to\infty}(\frac{1}{N}\sum_{k=1}^{N}u_i^k(x,y,z,t)),i=1,2,3$

Im Mittel **stationär** -> Einfaches zeitliches Mittel
$\bar{u}_i(x,y,z)=\lim_{\Delta t\to\infty}(\frac{1}{\Delta t}\int_{t}^{t+\Delta t}u_i(x,y,z,t)dt),i=1,2,3$

Da der Mittelwert der Schwankung null ist, kann der RMS-Wert (Root mean square) zur Mittelwertbildung verwendet werden:
$\bar{u_i'}=0$
$\sqrt{\overline{u_i'^2}}=\sqrt{\overline{u_1'^2}+\overline{u_2'^2}+\overline{u_3'^2}}\neq 0$

**Favre-Mittelung**:
$u_i=\tilde{u}_i+u_i''$
Definition so, dass Zusatzterm verschwindet: $\overline{\rho u_i''}=0$
-> Dichtegewichtete mittlere Geschwindigkeit
-> Erheblich vereinfachte Gleichungen mit Favre-Mittelwert

### Mittelung der Erhaltungsgleichung
- Ausgangspunkt: Navier-Stokes-Gleichungen für inkompressibel Fluide
Konti: $\frac{\partial u_j}{\partial x_j}=0$
Impuls: $\frac{u_j}{\partial t}+u_i\frac{\partial u_j}{\partial x_i}=-\frac{1}{\rho}\frac{\partial p}{\partial x_j}+\nu\frac{\partial^2u_j}{\partial x_i^2}$
-> **Vier Gleichungen** für **vier Unbekannte**: $u_1,u_2, u_3, p$
-> Einsetzen der Reynolds-Zerlegung in die Navier-Stokes-Gleichungen und dann Mittelung der ganzen Gleichung

**Gemittelte Kontinuitätsgleichung**
$\frac{\partial\overline{u_j}}{\partial x_j}=0$ und $\frac{\partial u_j'}{\partial x_j}=0$
-> Linearität der Kontinuitätsgleichung: keine Produkte von Schwankungsgrößen ($\overline{\bar{u}_iu_j'}=0$)

**Gemittelte Impulsgleichung**
$\overline{u_i\frac{\partial u_j}{\partial x_i}}=\frac{\partial}{\partial x_i}(\bar{u}_i\bar{u}_j)+\frac{\partial}{\partial x_i}\overline{(u_i'u_j')}=\bar{u}_i\frac{\partial\bar{u}_j}{\partial x_i}+\frac{\partial}{\partial x_i}\overline{(u_i'u_j')}$
-> Term, der das Produkt von Komponenten der Schankungsgeschwindigkeiten enthält: Ausdruck der Nichtlinearität des konvektiven Terms

Angewendet auf die gesamte Impulsgleichung:
$\frac{\partial \bar{u}_j}{\partial t}+\bar{u}_i\frac{\partial\bar{u}_j}{\partial x_i}=-\frac{1}{\rho}\frac{\partial\bar{p}}{\partial x_j}+\frac{\partial}{\partial x_i}(\nu\frac{\partial \bar{u}_j}{\partial x_i}-\overline{u_i'u_j'})$

**Reynoldsscher Spannungstensor**
Auf der rechten Seite der gemittelten Impulsgleichung wird dem viskosen Diffusionsterm ein Zusatzterm zugeschlagen. Dieser wird Reynoldsscher Spannungstensor genannt:
$\tau_{ij,turb}=-\rho\overline{u_i'u_j'}$

### Transportgleichung der Turbulenzenergie
Gleichung für die turbulente kinetische Energie (TKE):
$\bar{k}=\frac{1}{2}\overline{u_j'^2}$
Mit der Dissipation:
$\bar\varepsilon = \frac{\nu}{2}\overline{(\frac{\partial u_j'}{\partial x_i}+\frac{\partial u_i'}{\partial x_j})^2}$ 

Transportgleichung für TKE:
L+K=-P-DS+DF
- L: Lokale Änderung
- K: Konvektive Änderung
- P: Produktion
- DS: Dissipation
- DF: Diffusiver Transport

Vereinfachte Gleichungen:
- Statistisch homogene Turbulent: L=-P-DS
	- $\frac{\partial \bar{k}}{\partial t}=-\overline{u_i'u_j'}\frac{\partial\bar{u_j}}{\partial x_i}-\bar\epsilon$
- Statistisch isotrope Turbulenz: L=-DS
	- $\frac{\partial\bar{k}}{\partial t}=-\bar{\epsilon}$
 
# Unterschiedliche Strömungsfelder
### Turbulente Scherströmung
- Für technische Systeme der relevante Strömungsfall
	- Freistrahlströmungen
	- Tragflügelumströmungen
	- Strömungen in geschlossenen Brennräumen
- Durch die Komplexität dieser turbulenten Strömungen entzieht sie isch weitgehen einer theoretischen Analyse
![[Pasted image 20231220101715.png]]

### Statistisch homogene Turbulenz
- Alle gemittelten statistischen Fluktuationsgrößen sind invariant gegen eine räumliche Translation
	- Räumliches Analgogon zur statistischen Stationarität
	- Für gemittelte Fluktiationsgrößen $\overline{u_i'u_j'}$ gilt:
$\overline{u_i'(x_k)u_j'(x_k)}=\overline{u_i'(x_k+\Delta x_k)u_j'(x_k+\Delta x_k)}$
- Zugelassen sind konstante Gradienten der mittleren Geschwindigkeit

### Statistisch isotrope Turbulenz
- Alle statistischen Größen sind richtungsunabhängig: Invarianz bezüglich Rotation udn Spiegelung des Koordinatensystems:
$\overline{u_1'^2}=\overline{u_2'^2}=\overline{u_3'^2}$
- Alle mittleren Geschwindigkeiten sind Null
- Isotropie bedingt Homogenität
- Relevanz dieses Strömungsfalls:
	- Wichtiger Grenzfall: durch Vereinfachung theoretische Aussagen über Turbulenz möglich
	- Kleinskalige turbulente Bewegungen werden typischerweise als isotrop angenommen (Kolmogorovsche Annahme)
# Längenskalen turbulenter Strömungen
Turbulente Wirbel unterscheiden sich in ihrer Größe wobei
- $l_t$ die größten Wirbel
- $\eta$ die kleinsten Wirbel
beschreibt. Die größten Wirbel werden bestimmt durch geometrische Längen (z.B. Düsendurchmesser). Die kleinsten Wirbel entstehen durch den Zerfall großer Wirbel.
-> Energiekaskade ($l_t\to\eta$)
![[Pasted image 20231221085338.png]]
- Große Wirbel beinhalten größten Teil turbulenter kinetischer Enerige
	- Entziehen dem Strömungsfeld permanent Energie
	- Zerfall großer Wirbel -> Bildung kleinerer Strukturen
- Kontinuierlicher Energiefluss von großen zu kleinen Strukturen -> **Energiekaskade**
	- Energietransfer: Folge der nicht-linearen konvektiven Terme in Impulsgleichungen
	- Kontinuierlicher und stetiger Prozess: zwischen $l_t$ und kleinsten Abmaßen -> Wirbel aller Größen
- Kleinste Strukturen: Kolmogorov-Skalen
![[Pasted image 20231221085620.png]]

## Kolmogorovsche Hypothesen
1. Bei hinreichend großer Reynolds-Zahl haben Statistiken kleiner Wirbel eine universelel Form und sind eindeutig bestimmt durch die Parameter
	- Dissipationsrate $\bar\varepsilon$ mit $[\bar\varepsilon]=\frac{m^2}{s^3}$
	- Kinematische Viskosität $\mu$ mit $[\mu]=\frac{m^2}{s}$
	- $[k]=\frac{m^2}{s^2}$

1. Bei hinreichend großer Reynolds-Zahl haben Statistiken von Wirbeln der Größe r, mit $\eta << r << l_t$, einer universelle Form und sind abhängig von
	- Dissipationsrate $\bar\varepsilon$
	- Aber unabhängig von der kinematischen Viskosität $\nu$
# Turbulente Verbrennung
## Bilanzgleichungen
**Annahmen**
- Spezifische Wärmekapazität $c_{p,\alpha}=c_p=konst.$
- Druck $p=konst.$, Wärmeübertragung durch Strahlung wird vernachlässigt
- Lewis-Zahl $Le_\alpha=Le=Sc/Pr=1$

Temperaturgleichung: $\rho\frac{\partial T}{\partial t}+\rho u_i\frac{\partial T}{\partial x_i}=\frac{\partial}{\partial x_i}(\rho D\frac{\partial T}{\partial x_i})+\omega_T$
- Quellterm bedingt durch chemische Reaktion: $\omega_T=-\frac{1}{c_p}\sum_{\alpha=1}^Nh_\alpha\dot{m}_\alpha'''$

Die Temperaturgleichung ähnelt in dieser Form der Gleichung für den Massenbruch der Komponente $\alpha$
$\rho\frac{\partial Y_\alpha}{\partial t}+\rho u_i\frac{\partial Y_\alpha}{\partial x_i}=\frac{\partial}{\partial x_i}(\rho D\frac{\partial Y_\alpha}{\partial x_i})+\dot{m}_\alpha'''$

- Weitere Annahme: Ein-Schritt-Reaktion -> **Kopplungsbeziehung** zwischen $T$ und $Y_\alpha$

Somit kann ein **reagierender Skalar** definiert werden, welcher die Massenbrüche aller Komponenten und die Temperatur umfasst:
$\psi_\alpha=(Y_1, Y_2, ... Y_N, T)^T$ mit $\alpha=1,...N+1$
$\rho\frac{\partial \psi_\alpha}{\partial t}+\rho u_i\frac{\partial \psi_\alpha}{\partial x_i}=\frac{\partial}{\partial x_i}(\rho D_\alpha\frac{\partial \psi_\alpha}{\partial x_i})+\rho S_\alpha$
- $D_\alpha$ : Massendiffusivität, thermische Diffusivität
- $S_\alpha$ : Massen-/Temperaturquellterm

Für das reagierende Skalar wird eine Favre-Zerlegung durchgeführt und anschließend gemittelt:
$\bar\rho\frac{\partial\tilde\psi_\alpha}{\partial t}+\bar\rho \tilde{u}_j\frac{\partial\tilde\psi_\alpha}{\partial x_j}=\frac{\partial}{\partial x_j}\overline{(\rho D_\alpha\frac{\partial\psi_\alpha}{\partial x_j})}-\frac{\partial}{\partial x_j}(\bar\rho\widetilde{u_j''\psi_\alpha''})+\bar\rho\tilde{S}_\alpha$
... = Molekularer Transport - Turbulenter Transport + Gemittelter Quellterm
Bei großer Reynolds-Zahl kann der molekulare Transport vernachlässigt werden, wodurch nur noch der Quellterm geschlossen werden muss (siehe [[Modellierung turbulenter Flammen]]).

## Turbulente Vormischflammen
Aus laminaren Vormischflammen:
- Vorwärmzone heizt Gemisch kontinuierlich auf
- Diffusion von Reaktanden in die Reaktionszone
- Cross-Over Temperatur (Temperatur ab der die Reaktion stattfindet)
- Charakteristische Größen
	- Brenngeschwindigkeit $s_L$
	- Flammendicke $l_F$
### Anwendung
Vorgemischte Verbrennung wird industriell eingesetzt, wenn eine intensive Verbrennung auf kleinstem Raum stattfinden soll oder kann. Beispielsweise:
- Ottomotor
- Stationäre Gasturbinen
- Haushaltsbrenner bei Gasherden und -boilern

## Skalen turbulenter vorgemischter Verbrennung
Integrale turbulente Maße
$l_t=c_1\frac{\bar{k}^{3/2}}{\bar\varepsilon}$, $u'=\sqrt{\frac{2}{3}\bar{k}}$, $\tau=\frac{l_t}{u'}\sim\frac{\bar{k}}{\bar\varepsilon}$
Kleinste turbulente Maße/Kolmogorov-Skalen
$\eta=(\frac{\nu^3}{\bar\varepsilon})^{1/4}$, $u_\eta=(\nu\bar\varepsilon)^{1/4}$, $t_\eta=(\frac{\nu}{\bar\varepsilon})^{1/2}$
Flammendicke und Flammenzeit
$l_F=\frac{D}{s_L}=\frac{\lambda_b}{\rho_uc_ps_L}$, $t_f=\frac{l_F}{s_L}=\frac{D}{s_L^2}$
Turbulente Reynoldszahl
$Re_t=\frac{l_t}{l_F}\frac{u'}{s_L}$
Turbulente Damkähler-Zahl
$Da_t=\frac{\tau}{t_F}=\frac{l_t}{l_F}\frac{s_L}{u'}$
Karlovitz-Zahl (Interaktion kleinskaliger Turbulenz mit der Flamme)
$Ka=\frac{t_F}{t_\eta}=\frac{l_f^2}{\eta^2}=\sqrt{\frac{l_F}{l_t}(\frac{u'}{s_L})^3}$ und $Ka_\delta=\frac{I_\delta^2}{\eta^2}=\delta^2 Ka$

## Regimediagramm
Das Regimediagramm beschreibt die verschiedenen Flammenarten bei bestimmten Rahmenbedingungen.
![[Pasted image 20231221131513.png]]

### Gefaltete Flammen
- Ka < 1 -> $\eta > l_F$
- Interaktion einer sehr dünnen Flamme mit einer turbulenten Strömung
- Annahme: Unendlcih dünne Flamme

### Gelöschte Reaktionszonen
- $Ka_\delta > 1 \rightarrow \eta < I_\delta$
- Kleinste turbulente Wirbel dringen in die Reaktionszone ein
- Turbulenter Transport -> Radikale werden aus Reaktionszone herausgetragen
	- Örtliches Verlöschen in innerer Reaktionszone
	- Verlöschen der Flammenfront insgesamt möglich

### Dünne Reaktionszonen
- $Ka>1$ und $Ka_\delta < 1\rightarrow I_\delta <\eta<I_F$
- Mit $I_\delta\approx 0,1I_F\rightarrow Ka\approx 100Ka_\delta$
- Turbulente Mischung in Vorwärmzone
- Annahme: Unendlich dünne Reaktionszone (im Vergleich zu turbulenten Skalen)

## Turbulente Brenngeschwindigkeit
- Zentrale Aufgabe in der turbulenten vorgemischten Verbrennung: Quantifizierung der turbulenten Brenngeschwindigkeit $s_T$
- $s_T$: Geschwindigkeit, mit der sich eine turbulente Flammenfront in das unverbrannte Gemisch bewegt
- Unterscheidung zweier Grenzfälle durch Damköhler
	1. Großskalige Turbulenz <-> Gefaltete Flammen
	2. Kleinskalige Turbulenz <-> Dünne Reaktionszonen

Unterscheidung zwischen:
- Momentane Flammenfront
	- Flammenfläche $A_T$
	- Bewegt sich lokal mit der laminaren Brenngeschwindigkeit $s_L$ ins Unverbrannte
- Mittlere Flammenfront
	- Mittlere Flammenfläche $A$
	- Bewegt sich mit turbulenter Bewnngeschwindigkeit $s_T$
	- Entgegengesetzt gleich groß der mittleren Anströmung
![[Pasted image 20231221133038.png]]
Mit Konti: $\rho_us_LA_T=\bar\rho_us_TA$
-> $\frac{s_T}{s_L}=\frac{A_T}{A}=1+\frac{u'}{s_L}$
-> Faltung der laminaren Flamme ($A_T\uparrow$)-> Erhöhung von $s_T$
Turbulenz -> Flammenfläche $\uparrow$

## Turbulente Diffusionsflammen
Der einzige Unterschied in der Beschreibung von laminaren und turbulenten Flammen ist die Viskosität. In laminaren Flammen wird die molekulare Viskosität und in turbulenten Flammen die turbulente Scheinviskosität genommen.

Ein Phänomen bei turbulenten Flammen, im Vergleich zu laminaren Flammen ist, dass turbulente Flammen in ihrer Länge konstant sind und laminare Flammen mit steigender Reynolds-Zahl länger werden.
![[Pasted image 20231221134123.png]]


