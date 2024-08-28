Eine Phase ist ein Gebiet in dem sich die inneren Zustandsgrößen kontinuierlich ändern. Ein Gleichgewicht beschreibt einen Zustand, in dem alle Nettoströme zwischen zwei Phasen verschwinden.

An der Phasengrenze kommt es immer zum Austausch von Molekülen. Im **thermodynamischen Gleichgewicht** ist die Anzahl der Moleküle, die die Phase wechseln, in beide Richtungen gleich.

Im Allgemeinen werden drei verschiedene Gleichgewichte betrachtet:
- Thermodynamisches Gleichgewicht
- Mechanisches Gleichgewicht
- Chemisches Gleichgewicht

# Physikalische Grundlagen
Bei Flüssigkeitsgemischen wird zwischen zeotropen und azeotropen Gemischen unterschieden, wobei sich ein azeotropes Gemisch in einem Punkt wie ein Reinstoff verhält.
## Chemisches Potential
Ein Potential bezeichnet die Fähigkeit eines konservativen Kraftfeldes Arbeit zu verrichten.

Das chemische Potential $\mu / kj/mol$ ist eine Zustandsgröße und kennzeichnet die Neigung eines Stoffs:
- sich mit anderen Substanzen umzusetzen
- sich in eine andere Zustandsform zu wandeln
- an einen anderen ort abzuwandern

Die Stärke dieser Neigung ist stoff- und zustandsabhängig, wobei eine Umwandlung, Umsetzung oder Abwanderung freiwillig ist, wenn $\mu_{Anfang}>\mu_{Ende}$.

Linearer Ansatz zur Bestimmung des chemischen Pontentials:
$$
\mu=\mu_0+\alpha\cdot\Delta T+\beta\cdot\Delta p+\sum\gamma_i\cdot\Delta_i
$$

## Herleitung des chemischen Potentials
$$
\begin{align}
\text{Aus dem 2. Hauptsatz: }&
\newline
(1)\ dU&=TdS-pdV+\sum_i\mu_idn_i
\newline\newline
\text{Problem: }&\text{eingeschränkte praktische Handhabbarkeit}
\newline
\text{Abhilfe: }&
\newline
(2)\ H &= U+pV \text{ Enthalpie}
\newline
(3)\ A&=U-Ts\text{ Helmholtzsche Energie}
\newline
(4)\ G&=H-Ts\text{ Gibbsche freie Enthalpie}
\newline\newline
(5)\ dH&=dU+pdV+Vdp
\newline
\rightarrow\ (6)\ dH&=Tds+Vdp+\sum\mu_idn_i
\newline
\rightarrow\ (7)\ dA&=-SdT-pdV+\sum\mu_idn_i
\newline
\rightarrow\ (7)\ dG&=-SdT+Vdp+\sum\mu_idn_i
\newline\newline
dG&=\left( \frac{\partial G}{\partial T} \right)_{p,n_i}dT+\left( \frac{\partial G}{\partial p} \right)_{T,n_i}dp+\left( \sum_i \left( \frac{\partial G}{\partial n_i} \right)_{T,p,n_j\neq i} \right)dn_i
\newline
\rightarrow \mu_i &= \left( \frac{\partial G}{\partial n_i} \right)
\end{align}
$$
## Fugazität
Um das chemische Potential zu bestimmen, benötigt es einer Hilfsfunktion.
$$
d\mu_i=dg_i=v_i\cdot dp
$$
Unter der Annahme eines idealen Gases findet sich folgender Ausdruck:
$$
\mu_i-\mu_i^0=R\cdot T\ ln\left( \frac{p}{p^0} \right)
$$
Die Fugazität $f_i$ nach Lewis ist ein Zustand in abhängig von Temperatur, Druck und Konzentration. Dabei steht $f_i$ für einen korrigierten Druck. Dabei ist die Abweichung von Fugazität zu idealem Druck umso größer, je höher der Druck ist.

Somit gilt für die Gleichgewichtsbedingun:
$$
\begin{align}
\mu_i^{\alpha,0}+R\cdot T\ ln \left( \frac{f_i^\alpha}{f_i^{\alpha,0}} \right) &= \mu_i^{\beta,0}+R\cdot T\ ln \left( \frac{f_i^\beta}{f_i^{\beta,0}} \right)
\newline\newline
\text{Bei gleichem Referenzzustand:}
\newline
f_i^\alpha&=f_i^\beta
\end{align}
$$
Um die Fugazität weiterverwenden zu können, müssen Hilfsfunktionen definiert werden:
- Fugazitätskoeffizient $\varphi_i$: Verhältnis Fugazität und Partialdruck für die Korrektur bei realem Verhalten
- Aktivität $\alpha_i$; Verhäktnis von Figazität und Standardfugazität
- Aktivitätskoeffizient $\gamma_i$: Verhältnis aus Aktivität und beliebigem Konzentrationsmaß $\psi_i$

Um die Fugazität zu beestimmen gibt es zwei Möglichkeiten:
- Verwendung einer Zustandsgleichung
- Verwendung einer Zustandsgleichung für die Gasphase bzw, eines Aktivitätskoeffizienten für die flüssige Phase
$$
\begin{align}
\text{Für Gase: }f_i^D&=\psi_i^D\cdot\varphi_i^D\cdot p
\newline\newline
\text{Für Flüssigkeiten: }f_i^{Fl}&=\gamma_i\cdot K_i^{Fl}\cdot f_i^0
\end{align}
$$
## Aktivität
Bei idealen Flüssigkeiten oder Gasen werden alle Atome oder Moleküle als starre Kugeln angesehen:
-> Es wirken keine anziehenden oder abstoßenden Kräfte
-> Atome/Moleküle können beliebig ersetzt werden

Die Aktivität beschreibt Wechselwirkungen zwischen den verschiedenen Molekülen.

# Berechnung von Gleichgewichten
Um Gleichgewichte zu berechnen, wird die Fugazität benötigt, für welche wiederum die Aktivität benötigt wird.

Im Allgemeinen gilt:
$$
\psi^{fl}_i\cdot\gamma^{fl}_i\cdot p_{i,sat}=\psi_i^D\cdot p
$$

Ein geeignetes Modell muss gewählt werden, je nachdem ob das realen Gas durch ideale Modelle beschrieben werden kann:
- ideale Gase
	- Keine Interaktion außer elastische Stöße
	- Moleküle sind Punktteilchen
	- meist bei niedrigen Drücken anwendbar
- ideale Flüssigkeiten
	- Keine innere Reibung
	- Inkompressibel
	- Keine Oberflächenspannung
## Raoult'sches Gesetz
Das Raoult'sche Gesetz betrachtet eine Standarrdfugazität und vernachlässigt die Aktivität. Somit ist das Gesetz unabhängig vom Lösungsmittel definiert, was einen Fehler im Vergleich mit realen System herbeiführt.

Somit ist das Raoult'sche Gesetz nur für **ideale Gase** zu verwenden. Ebenso ist das Raoultsche Gesetz zu verwenden, wenn der Partialdruck einer Flüssigkeit in der Gasphase bestimmt werden soll.
## Henry-Koeffizient
Um eine genauere Bestimmung des Gleichgewichts zu erreichen, wird der Henry-Koeffizient zur bestimmung der Standardfugazität verwendet. Der Henry-Koeffizient beschreibt somit die Löslichkeit über einen einfachen linearen Zusammenhang zwischen dem Partialdruck in der Gasphase und der Stoffmengenkonzentration in der Flüssigphase. $H_{ij}$ ist für Stoffpaarungen tabelliert und stark temperaturabhängig.

Das Herny'sche Gesetz wird verwendet, wenn die Konzentration einer Gasförmigen Komponente in einer Flüssigkeit bestimmt werden soll.