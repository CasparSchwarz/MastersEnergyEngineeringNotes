![[Pasted image 20231117095740.png]]
Bei Diffusionsflammen werden Brennstoff und Oxidator getrennt dem Brennraum zugeführt. Dabei diffundiert der Oxidator in den verdampften Brennstoff, wodurch eine Randschicht entsteht, in der der Brennstoff reagiert. Damit es zur Reaktion kommt, müssen Brennstoff und Oxidator molekular gemischt sein. Der Mischgrad ist dabei geschwindigkeitsbestimmend, da die Mischung der langsamste Schritt der Reaktion ist.

Zur Modellierung von Diffusionsflammen werden
- Gegenstrombrenner,
- Schlitzbrenner und
- Jetbrenner
genutzt. Zudem ist der Mischungsbruch $Z$ ein wichtiger Parameter zur Beschreibung von Diffusionsfalmmen:
$Z=\frac{m_1}{m_1+m_2}=\frac{1}{1+\lambda l_{min}Y_{B,1}}$
mit:
- 1: Brennstoffstrom
- 2: Oxidatorstrom

## Kopplungsbeziehungen
Brennstoff und Oxidator im unverbrannten Zustand:
$\frac{Y_{O_2}-Y_{O_s,u}}{\nu^{'}_{O_2}M_{O_2}}=\frac{Y_B-Y_{B,u}}{\nu^{'}_BM_B}$

Normalisierung zwischen Oxidator und Brennstoff
$Z=\frac{\beta-\beta_2}{\beta_1-\beta_2}$
mit:
- $\beta = \nu Y_B-Y_O$
- $\nu = \frac{M_O\nu_O}{M_B\nu_B}$

Temperatur als Funktion von Z
$Z=\frac{h-h_2}{h_1-h_2}=\frac{T_u-T_2}{T_1-T_2}$
<=> $T_u(Z)=T_2+Z(T_1-T_2)$
mit:
- $Le=\frac{\lambda}{\rho c_p D}=1$
- $c_p = konst$

## Flammenflächenmodell
Annahmen:
- Verbrennung in einer Diffusionsflamme erfolgt in der singulären Fläche stöchiometrischer Mischung
- Brennstoff und Sauerstoff diffundieren von entgegengesetzten Seiten in die Flammenfläche hinein
- Sie verschwinden dort, während die Produktkomponenten und die Temperatur dort ein singuläres Maximum haben
Voraussetzungen:
- Unendlich große Verweilzeiten oder unendlich schnelle Chemie
- Vollständige Verbrennung
- Eine chemische Bruttoreaktion

Mageres Gemisch: $0<Z<Z_{st}$ : Sauerstoff vorhanden
Fettes Gemisch: $Z_{st}<Z<1$ : Brennstoff vorhanden

Verlauf der Massenbrüche:
![[Pasted image 20231117102122.png]]

## Burke-Schumann-Lösung
Annahme:
- $K_p \rightarrow \infty$
- $c_p=const.$
- Unendlich schnelle Reaktion
$T=T_u(Z)+\frac{Z}{Z_{st}}[T_{st}-T_u(Z_{st})]$ bei $0\leq Z \leq Z_{st}$
$T=T_u(Z)+\frac{1-Z}{1-Z_{st}}[T_{st}-T_u(Z_{st})]$ bei $Z_{st} \leq Z \leq 1$

## Flamelet-GLeichung
- Verbrennung in dünner Schicht in unmittelbarer Nähe der Fläche stöchiometrischer Mischung
- Einfluss endlich schneller chemischer Kinetik in der Nähe dieser Fläche am größten
-> Konturangepasstes Koordinatensystem
$x_1, x_2, x_3, t \rightarrow Z(x_1, x_2, x_3, t), Z_2,Z_3,\tau$
![[Pasted image 20231219161250.png]]
Instationäre Flamelet-Gleichung:
$\rho\frac{\partial T}{\partial\tau}-\rho D(\frac{\partial Z}{x_j})^2\frac{\partial^2 T}{\partial Z^2}=\dot{\omega}_T$
Instationärer Term - Mischung = Quellterm

Stationäre Flamelet-Gleichungen:
$-\frac{\rho\chi_{st}}{2}\frac{\partial^2T}{\partial Z^2}=\dot{\omega}_T$
$-\frac{\rho\chi_{st}}{2}\frac{\partial^2Y_{\alpha}}{\partial Z^2}=\dot{m}_{\alpha}''''$

Dabei beschreibt $\chi$ den Diffusionskoeffzienten im Mischungsbruchraum

### Eigenschaften der Flamelet-Gleichungen
- Zustandekommen aus einer Art Grenzschichtapproximation
- Eindimensional
- Mischungsbruch ist unabhängige Koordinate
- Wie beim Flammenflächenmodell universelle Darstellung der Temperatur und der Konzentrationen als Funktion des Mischungsbruchs
- Numerische Berechnung bei bekanntem $\chi_{st}$
- Grenzfall $\chi_{st}\rightarrow 0$: Gleichung für homogenen Reaktor

Wenn $\chi \uparrow\rightarrow T \downarrow$ da der Wäremabfluss mit dem Diffusionskoeffizienten steigt und dadurch die Temperatur sinkt. Sinkt die Temperatur zu stark kommt es zur Verlöschung der Flamme (T < cross over temperature).

## Laminare Freistahldiffusionsflamme
- Runde laminare Freistahldiffusionsflamme
	- Laminarer Brennstoffstrahl tritt aus einer runden Düse als Freistrahl aus
	- Das sich bildende Gemisch ist gezündet
![[Pasted image 20231219170002.png]]
Ausganspunkt zur Beschreibung laminarer Freistrahldiffusionsflammen bildet die Grundgleichung für stationäre rotationssymmetrische Grenzschichtströmungen ohne Auftrieb.

Konti: $\frac{\partial (\rho u_z r)}{\partial z} + \frac{\partial (\rho u_r r)}{\partial r} = 0$
Impulsgleichung in z-Richtung: $\rho u_z r\frac{\partial u_z}{\partial z} + \rho u_r r\frac{\partial u_z}{\partial r} = -r\frac{\partial p}{\partial z}+\frac{\partial}{\partial r}(\mu r\frac{\partial u_z}{\partial r})$
Mischungsbruch: $\rho u_z r\frac{\partial Z}{\partial z} + \rho u_r r\frac{\partial Z}{\partial r} = \frac{\partial}{\partial r}(\frac{\mu}{Sc} r\frac{\partial u_z}{\partial r})$

Schmidt-Zahl $Sc=\frac{\mu}{\rho D}$

Inkompressibler runder Freistrahl
- Ruhende Umgebung
- Kosntante Dichte
- Kein Auftrieb
-> Ähnlichkeitslösung
-> Ähnlichkeitskoordinate $\eta=\frac{r}{z}$

Mischungsbruch auf der Achse $Z_a(z)=Z(z, r=0)$
$Z_a(z)=\frac{1+2Sc}{32}\frac{\rho_0}{\rho_{\infty}}\frac{Re}{C}\frac{d}{\zeta}$
-> $L=\frac{1+2Sc}{32Z_{st}}\frac{\rho_0}{\rho_{\infty}C}\frac{u_0d^2}{\nu}-a$
