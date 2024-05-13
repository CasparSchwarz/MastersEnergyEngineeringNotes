In der kinetischen Gastheorie wird die Durchmischung zweier Gase beschrieben.

# Diffusion in Gasen
## Gedankenexperiment:
In einem abgeschlossenen Raum befinden sich die Moleküle A (links) und B (rechts). Diese sind zunächst getrennt voneinander, doch der Konzentrationsunterschied bewirkt Diffusionssträme der beiden Stoffe.

**Voraussetzungen**:
- Moleküle besitzen ähnliche Eigenschaften
- Moleküle bewegen sich mit der durchschnittlichen Geschwindigkeit $\bar w$

## Herleitung
Die Wahrscheinlichkeit, dass Moleküle A durch die Kontrollebene an der Stelle $x_0-l$ hindurchtreten ist höher, als dass sie durch die Kontrollebene an der Stelle $x_0+l$ treten, da die Anzahl an A-Molekülen links größer ist als rechts. Somit gilt für die Diffusion von A in x-Richtung:
$$
\begin{align}
j_A''&=\eta\cdot c_{ges}\frac{M_A}{N_A}\bar w\left[ \left.\frac{c_a}{c_{ges}}\right|_{x_0-l} - \left.\frac{c_a}{c_{ges}}\right|_{x_0+l} \right]
\newline\newline
Taylorentwicklung\ (linearisiert):
\left.j_A''\right|_{x=x_0}&=\eta\cdot n_{ges}\cdot\bar w\cdot\left[ -2l \left.\frac{d\frac{n_A}{n_{ges}}}{dx}\right|_{x_0} \right]
\newline\newline
Aus\ Vergleich\ mit\ Fick'schem\ Gesetz:D&=2\eta\cdot\bar w\cdot l

\end{align}
$$
