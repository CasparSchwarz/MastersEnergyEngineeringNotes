In der Strahlung von Gasen finden
- Emission (wirkt versärkend)
- Absorption (wirk abschwächend)
- Streuung (beides möglich)
- Transmission
statt.

# Physikalische Grundlagen
Die Energie eines Photons wird wie folgt beschrieben:
$$
E_{Quant}=f\cdot h
$$
Bei Betrachtung eines Volumenelements kommt in Abhängigkeit der Strahlungszahl $\eta=\frac 1\lambda$  nur noch ein Teil der einfallenden Intensität am Ende des Kontrollvolumens an.
![[Pasted image 20240501173026.png]]
## Quantenphysik
Atome und Moleküle können Strahlung im technisch relevanten Bereich des sichtbaren Lichts und der Infrarotstrahlung durch zwei Mechanismen aufnehmen oder abgeben:
1. Änderung des Energiezustands der Elektronen
2. Änderung des Vibrationszustands des Moleküls/Atoms
-> Der ablaufende Mechanismus hängt von der Energie und damit der Wellenzahl $\eta_Q$ des Lichtquants ab:
$$
E_Q=g\cdot c_0\cdot \eta_Q
$$
## Bohr'sches Atommodell
Das Atommodell nach Bohr beruht auf folgenden Annahmen:
- System besteht aus Atomkern und Elektronen
- Elektronen befinden sich auf festen Umlaufbahnen
- Beim Übergang zwischen den Schalen muss Energie aufgenommen oder abgegeben werden
-> Elektromagnetische Strahlung kann emittiert oder absorbiert werden
-> Strahlung, die im sichtbaren oder ultravioletten Bereich liegt, ist ausreichend energiereich um Elektronen-Übergänge hervorzurufen

Die Energie des Übergangs von einem Elektron in eine andere Schale kann berechnet werden:
$$
\Delta E=Z^2Rh\left(\frac{1}{n²_2}-\frac{1}{n^2_1}\right)
$$
## Molekülstrahlung
Moleküle können Strhalung aufnehmen oder abgaben indem sie ihren **Oszilationszustand** oder **Rotationszustand** und damit ihr Dipolmoment ändern:
![[Pasted image 20240502090045.png]]
Ein Molekül hat dann ein **Dipolmoment**, wenn der Schwerpunkt der positiven Ladungen (Atomkerne) und der negativen Ladungen (Elektronen) nicht zusammenfällt. Unpolare Moleküle ($O_2,N_2$) haben keins.

### Oszillationszustand
Wenn sich zwei Atomkerne eines Moleküls aus ihrem Gleichgewichtszustand aneinander annähern, wirkt die Coulombkraft abstoßend. Wenn sie sich voneinander weg bewegen, wirken die Bindungskräfte anziehend.
-> Für kleine Auslenkungen sind die Kräfte proportional zur Auslenkung und das System kann analog zu einem Feder-Masse-System als **harmonischer Oszillator** mit der Eigenfrequenz $\nu$ betrachtet werden.

Dabei ist der Oszillationszustand gequantelt und die angenommenen Energieniveaus äquidistant angeordnet:
$$
Schrödinger-Gleichung:\ E_{Osz,n}=h\cdot\nu \left(n+\frac12\right)
$$
![[Pasted image 20240502090601.png]]

Bei realen Molekülen gilt die Annahme äquidistanter Energieniveaus nur bei kleinen Abständen vom Gleichgewichtszustand.

## Rotationszustand
Während bei den Oszillationsübergängen jedes $\Delta n$ möglich ist, sind bei der Rotation nur bestimmte Übergänge möglich.
Regel:
- 2-Atomige Moleküle: $\Delta l=\pm1$
- 3-Atomige Moleküle: $\Delta l=\pm1$ oder $\Delta l = 0$

$$
\begin{align}
E_{Rot,l}&=\frac{h^2}{8\pi^2J}(l+1)\cdot l
\newline\newline
\Delta E_{Rot}&=E_{Rot}(l)-E_{Rot}(l-1)
\end{align}
$$

Das Absorptionsband wird dementsprechend in 3 Bänder unterteilt:
- P-Zweig: $\Delta l=-1$
- Q-Zweig: $\Delta l=1$
- R-Zweig: $\Delta l=0$


## Absorption
Die Absorption wird durch den Absorptionskoeffizienten beschrieben:
$$
\alpha=\frac{I_\eta}{I_0}
$$
## Emission
Emission stellt das Gegenstück zur Absorption dar. Durch die selben Mechanismen wie in der Absorption wird ein Strahlungsqant erzeugt. Dabei gilt gemäß dem **Kirschhoff'schen Gesetz**:
$$
\begin{align}
\alpha_\eta&=\epsilon_\eta
\newline
\epsilon_\eta&=\frac{I_\eta}{I_{schwarz}}
\end{align}
$$
## Streuung
Durch die Streuung wird die Verteilung auf die Raumrichtung bestimmt und die einfallende Strahlung vom ursprünglichen Weg abgelenkt.
$$
\frac{dI_{\eta,S}}{dS}=-\sigma_{S,\eta}I_\eta
$$
Zu beachten ist, dass die gestreute Strahlungsmenge $dI_{eta,S}$ nicht konstant über alle Raumwinkel $\theta$ und $\varphi$ ist. Den Anteil, der in eine bestimmte Richtung abgestrahlt wird beschreibt die Phasenfunktion $\Phi(\theta,\varphi)$
$$
\Phi(\theta,\varphi)=\frac{dI_{\eta,S}(\theta,\varphi)}{\frac{1}{4\pi}dI_{\eta,S}}
$$
![[Pasted image 20240501173912.png]]
Es gibt verschiedene Arten von Strahlung, die in Abhängigkeit der Partikelgröße $D$ und Wellenlänge $\lambda$ zueinander angewendet werden:
- Wenn $D<<\lambda$ -> Theorie der Rayleigh-Streuung
- Wenn $D\approx\lambda$ -> Theorie der Mie-Streuung
- Wenn $D>>\lambda$ -> Geometrische Optik

# Abschwächung
Die Gesamtabschwächung kann durch die Koeffizienten $a_\eta$ und $\sigma_\eta$ beschrieben werden:
$$
\begin{align}
\frac{I_\eta}{dS}&=\frac{I_{\eta,Absorption}}{dS}+\frac{I_{\eta,Streuung}}{dS}
\newline
\frac{I_\eta}{dS}&=-K_\eta\cdot I_\eta
\newline
Mit\ K_\eta&=a_\eta+\sigma_\eta
\newline
\newline
\rightarrow I_\eta(S)&=I_{\eta,0}\cdot e^{-K_\eta\cdot S}
\end{align}
$$
# Verstärkung
Verstärkt wird die Strahlung entweder durch Streuung oder Emission:
$$
\begin{align}
I_{\eta,Emission}&=\frac{1}{4\pi}\int\int\int a_\eta I_{\eta,schwarz}\ dS\ d\varphi\ d\theta
\newline \newline
\frac{dI_{\eta,eingestreut}}{dS}&=\frac{\sigma_{S,\eta}}{\eta}\int^{2\pi}_{\varphi=0}\int^\pi_{\theta=0}I_\eta(\varphi,\theta)\phi(\varphi,\theta)sin(\theta)\ d\theta\ d\varphi
\newline\newline
\frac{dI_{\eta}}{dS}&=\frac{dI_{\eta,Emission}}{dS}-\frac{dI_{\eta,Absorption}}{dS}-\frac{dI_{\eta,Gestreut}}{dS}+\frac{dI_{\eta,eingestreut}}{dS}
\end{align}
$$
