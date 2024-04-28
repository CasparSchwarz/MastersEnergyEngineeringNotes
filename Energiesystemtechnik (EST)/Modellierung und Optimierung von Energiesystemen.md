## Definition Modell
Ein Modell erlaubt die Durchführung von Experimenten / Messungen, die am realen System nicht durchgeführt werden können und ist häufig billiger / schneller / sicherer als ein Experiment.
![[Pasted image 20231019092511.png]]

Typen von Modellen:
- Mentale Modelle (Intuition, Gefühl)
- Physikalische Modelle
- Modelle aus Analogien
- Mathematische Modelle (Stehen im Fokus)

Je nach betrachteten Zeitraum und räumlicher Ausdehnung muss das Modell weiter Vereinfacht werden. Dabei steigt die Vereinfachung mit steigendem Zeitraum und räumlicher Ausdehnung.

## Mathematische Modelle
Es gibt verschieden Möglichkeiten ein mathematisches Modell aufzubauen. Dabei ist die Komplexität unterschiedlich, je nach gewähltem Modell.
![[Pasted image 20231019092805.png]]

Ziele in der Modellierung von Energiesystemen sind:
- Analyse von bestehenden Systemen
- Optimierung von bestehenden Systemen
- Planung von neuen Systemen
Ein Energiesystem umfasst hierbei die lokale Energieerzeugung, Transport bzw. Verteilung und die Umwandlung von End- in Nutzenergie. Ebenso sind Kopplungsstellen an angrenzende bzw. übergeordnete Versorgunsstrukturen zu berücksichtigen.

## Optimierung
In der Optimierung wird ein Ziel in Form einer Zielfunktion definiert. Diese Zielfunktion gilt es zu maximieren oder zu minimieren, wobei die Zielfunktion von Entscheidungsvariablen abhängt, welche wiederum durch Nebenbedingungen beschränkt sind.
![[Pasted image 20231019093246.png]]
Die Optimierung geschieht in Energiesystemen auf **3 Ebenen**:
- Struktur
- Dimensionierung
- Betrieb

| Gleichungen | Kontinuierlich | Diskret |
| ---- | ---- | ---- |
| linear | linear program (LP) | mixed-integer linear program (MILP) |
| nichtlinear | nonlinear program (NLP) | mixed-integer nonlinear program (MINLP) |
### Lineare Optimierung
Mathematisch formuliert:
$\min\limits_x z = c^Tx = c_1x_1+c_2x_2+...+c_nx_n$
$s.t. Ax\leq b$

### Nicht-Lineare Optimierung
Bei nicht-linearen Optimierungsproblemen muss numerisch das Optimum gefunden werden. Dafür wird das Newton-Verfahren angewendet. Problem: **Durch die Konvergenz des Newton-Verfahrens ist das Finden des globalen Optimums nicht garantiert**.

Lösung: Lagrange-Methode
1. Einen Lagrange-Multiplikator $\lambda$ für jede Nebenbedingung einführen
2. $\lambda$ mal die Nebenbedingung in die Zielfunktion -> Lagrangefunktion
3. Partielle Ableitungen der Lagrangefunktion nach Variablen und allen $\lambda$ bilden
4. Gleichungssystem: Partielle Ableitungen = 0

Mathematisch formuliert:
$L(x, \lambda) = f(x) - \lambda h(x)$
$\frac{\partial L}{\partial x}=\frac{\partial f(x)}{\partial x} - \lambda\frac{\partial h(x)}{\partial x} = 0$
$\frac{\partial L}{\lambda} = -h(x) = 0$

### Mixed-integer linear program (MILP)
**Branch and Bound**: Jeder Lösungsweg wird ausprobiert, bis an einer Stelle die Randbedingungen nicht mehr erfüllt sind oder das Ende des Lösungswegs erreicht wird.
**Problem**: Die Komplexität steigt Exponential $\mathcal{O}(2^n)$
**Lösungsansatz**: Jede gefundene Lösung wird Obere / Untere Schranke des Optimierungsproblems -> Weitere Nebenbedingung mit jeder gefundenen Lösung

MILP kann genutzt werden um nichtlineare Probleme zu lösen: Dazu wird das nichtlineare Problem stückweise linearisiert.

Mathematisch formuliert:
$\min\limits_{x, y}=c^Tx+a^Ty$
$s.t \ Ax+By \leq b,$
$y \in \mathbb{Z},\ x \in\mathbb{R}^n,\ a\in\mathbb{R}^t,\ c\in\mathbb{R}^n,$
$A\in\mathbb{R}^{m\times n},\ B\in\mathbb{R}^{m\times t},\ b\in \mathbb{R}^m$

### Mixed-Integer nonlinear program (MINLP)
**Branch and Bound**: Siehe oben. Kann angewendet werden wenn die relaxierten Unterprobleme global lösbar sind. Das ist nur der Fall, wenn die relaxierten Unterprobleme linear oder konvex sind.

Mathematisch formuliert:
$\min\limits_{x, y}z=f(x,y)$
$s.t\ h(x,y)=0,$
$\quad \ \ g(x,y) \leq 0,$
$x\in\mathbb{R}^n,\ y\in\mathbb{Z}^n$

## Optimierung von Wärmeübertragernetzwerken
Ziel: Mnimierung der Gesamtkosten = Betrieskosten + Kapitalkosten

Zur Optimierung von [Wärmeübertragernetzwerken](Energieeinsatz#Wärmeintegration) kann das Euler-Theorem verwendet werden. Jedoch sagt das Euler-Theorem nur etwas über die Anzahl der Wärmeübertrager aus und nichts über die Position der Wärmeübertrager.

### Sequenzieller Ansatz
**Minimierung der Anzahl an Stromkopplungen**
- Stromkopplung ist die Verschaltung von einem heißen und einem kalten Strom

$min\Sigma_h\Sigma_k\epsilon_{h,k}$
