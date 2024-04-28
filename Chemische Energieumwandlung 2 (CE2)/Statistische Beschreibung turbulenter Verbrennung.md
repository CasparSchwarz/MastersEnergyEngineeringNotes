Eine analytische Betrachtung von turbulenten Flammen ist nicht möglich. Um turbulente Flammen zu beschreiben und zu modellieren muss auf stochastische Zusammenhänge und Statistik zurückgegriffen werden.
# Zustandsraum
Ein Zustandsraum beschreibt die Gesamtheit aller möglichen Ereignisse. In dem Zustandsraum werden die Wahrscheinlichkeiten von Ereignisse definiert.
- Zufallsvariable $U$
- Zustandsraumvariable $V$
Im Zustandsraum können bestimmte Ereignisse eintreten. Dabei beschreibt ein Ereignis einen bestimmte Bereich im Zustandsraum.
Beispiel:
- Ereignis A: $A=\{U<V_a\}$
- Ereignis B: $B=\{V_a\leq U<V_b\}$

Die Wahrscheinlichkeit des Eintretens eines Ereignisses ist demnach:
$p=P(A)=P\{U<V_a\}$
wobei für p=0 das Eintreten ausgeschlossen und für p=1 das Eintreten sicher ist.

# Verteilungsfunktion (CDF)
- Wahrscheinlichkeit lässt sich ausdrücken durch Verteilungsfunktion
- Wichtige Eigenschaften einer Verteilungsfunktion
	1. $F(-\infty)=0$
	2. $F(+\infty)=1$
	3. $F$ ist monoton steigned

# Gemeinsame Verteilungsfunktion (jCDF)
- Gemeinsame CDF der Zufallsvariablen U_1, U_2, ...
- Wichtigste Eigenschaften einer jCDF
	- Monoton Steigend
	- $F_{1,2}(-\infty, V_2)=P\{U_1<-\infty, U_2<V_2\}=0$
	- $F_{1,2}(+\infty, V_2)=P\{U_1<+\infty, U_2<V_2\}=F_2(V_2)$ -> Marginale CDF

# Wahrscheinlichkeitsdichtefunktion (PDF)
- Ableitung der Verteilungsfunktion (CDF)
$f(V)=\frac{dF(V)}{dV}$
- Wichtige Eigenschaften einer PDF
	1. CDF monoton steigend -> PDF $f(V)\geq0$
	2. Fläche ist eins $\int^\infty_{-\infty}f(V)dV=1$
	3. $f(-\infty)=f(+\infty)=0$

## Momente einer PDF
- PDF von U bekannt -> n-tes Moment
$\overline{U^n}=\int^\infty_{-\infty}V^nf(V)dV$ und $\overline{Q(U)^n}=\int^\infty_{-\infty}Q(V)^nf(V)dV$

**Zentrierte Momente**
$\mu_n=\overline{(U-\bar{U})^n}=\int^\infty_{-\infty}(V-\bar{U})^nf(V)dV$

# Gemeinsame Wahrscheinlichkeitsdichtefunktion (jPDF)
- Gemeinsame PDF
$f_{1,2}(V_1,V_2)=\frac{\partial^2F_{1,2}(V_1,V_2)}{\partial V_1\partial V_2}$
- Wichtige Eigenschaften einer jPDF
	- Nicht-negativ
	- Fläche ist eins $\int\int f_{1,2}(V_1,V_2)dV_2dV_1|^\infty_{-\infty}=1$
	- Marginale PDF $f_2(V_2)=\int^\infty_{-\infty}f_{1,2}(V_1, V_2)dV_1$
