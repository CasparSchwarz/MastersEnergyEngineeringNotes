Windenergie beschreibt die Stromerzeugung aus Wind durch Winkraftanlagen. Dabei wird die kinetische Energie des Windes in elektrische Energie umgewandelt. Siehe [[Windenergie/Windenergie|Windenergie]]

# Windangebot
Das Windangebot ist stark fluktuierend:
- Im Winter größeres Angebot als im Sommer
- Gleicht Jahresschwankngen der PV teilweise aus
- Überlagert werden jahreszeitliche Schwankungen durch Fluktuationen auf Wochen-/Tagesebene

Die Windgeschwindigkeit wird durch eine Weibull-Verteilung beschrieben:
$$
\begin{align}
Dichtefunktion:\ f(v)&=\frac k a \left(\frac v a\right)^{k-1}\cdot e^{-\left(\frac v a\right)^k}
\newline\newline
Verteilungsfunktion:\ F(v)&=1-e^{-\left(\frac v a\right)^k}=\int f(v)\ dv
\newline\newline
Mit:\ a&:\ Skalierungsfaktor
\newline
k&:\ Formfaktor
\end{align}
$$
Ebenso ist die Windgeschwindigkeit stark höhenabhängig. Die Berechnung der Geschwindigkeit in anderen Höhen als der Referenzhöhe geschieht über den Potenzansatz nach Hellmann:
$$
\begin{align}
\bar v_H&=\bar v_{ref}\left(\frac{H}{H_{ref}}\right)^\alpha
\newline
Mit\ \alpha&:\ Geländeroberfläche
\end{align}
$$
# Typen von WKA
WKA werden nach ihrer Achsausrichtung Klassifiziert:
- Horizontale Achsausrichtung
	- Einflügler
	- Zweiflügler
	- Dreiflügler
- Vertikale Achsausrichtung
	- Darrieus-Rotor
	- Savonius-Rotor

Wobei dabei alle bis auf der Savonius-Rotor mit Auftrieb die Windenergie umwandeln. Der Savonius-Rotor nutzt das Widerstandsprinzip. Siehe [[Rotorkonzepte]]

## Ein- und Zweiflügler
**Vorteile**:
- günstige Herstellung
- geringes Rotorgewicht
- höhere Rotorfrequenz (geringeres Drehmoment, geringerer Materialaufwand für Getriebe und Generator)
- größere Anlagen möglich
- weniger Flügel

**Nachteile**:
- größere Randwirbelverluste
- hohe Geräuschemissionen (aufgrund der hohen Umfangsgeschwindigkeit)

## Dreiflügler
**Vorteil**:
- höherer theoretischer Wirkungsgrad
- geringerer Geräuschemissionen
- Schingungsdynamik einfacher beherrschbar
- erprobte Technik

**Nachteile**:
- höherer Material- und Fertigungskosten
- aufwendige Montage bei Off-Shore-Anlagen

## Darrieus-Rotor
**Vorteil**:
- keine Windrichtungsnachführung notwendig
- keine Blattverstellung notwendig
- Getriebe und Generator können am Boden installiert werden
- Blatt nach Prinzip der Kettenlinie geformt (nur Zugspannungen, keine Biegemomente)

**Nachteile**:
- höhere Anlaufgeschwindigkeit (4 - 5 m/s)
- kein automatischer Anlauf (Motor notwendig)
- geringere Wirkungsgrade (Leistungsbeiwerte bis 40 %)
- anfällig für Schwindungen

## Savonius-Rotor
**Vorteile**:
- weder Windrichtungsnachführung noch Blattverstellung notwendig
- Getriebe und Generator können am Boden installiert werden
- automatischer Anlauf (daher oft zum Antrieb von Darrieus-Rotoren verwendet)
- geringe Anlaufgeschwindigkeit (ab 2 m/s)

**Nachteile**:
- geringe Leistung
- hoher Materialbedarf

# Physikalische Grundlagen
Siehe [[Windphysik]]

Kinetische Energie der Luft:
$$
P_{Wind}=\frac 1 2 \dot m v^2=\frac 1 2 \rho A v^3
$$
Entnommene Leistung der Turbine:
$$
P_{Turb}=Av\frac \rho 2(v^2_1-v^2_2)
$$
Nach der Betz'schen Theorrei kann der Luft nicht die gesamte Energie entzogen werden (da sonst keine Strömung mehr besteht). Aufgrund der Betzschen Theorie können WKA wie folgt beschrieben werden:
![[SmartSelect_20240510_083608_Drive.jpg]]
$$
\begin{align}
Geschwindigkeit\ in\ Rotorebene\ v&=\frac{v_1-v_2}{2}
\newline\newline
Leistungsbeiwert\ c_P(x)&=\frac{P_{Turb}}{P_0}=\frac{1+x}{2}(1-x^2)
\newline\newline
Mit\ x&=\frac {v_2}{v_1}
\end{align}
$$
Dabei ist zu erkennen, dass $c_P$ maximal bei $x=\frac 1 3$ wird und einen Wert von $c_P=59,3 \%$ erreicht.

Die Schnelllaufzahl beschreibt das Verhältnis aus Umfangsgeschwindigkeit des Rotors zur Windgeschwindigkeit:
$$
\lambda=\frac u v
$$
# Betriebsverhalten
Damit eine WKA elektrische Leistung erzeugen kann, muss der Wind eine bestimmte Einschaltgeschwindigkeit überschreiten. Unterhalb der Einschaltgeschwindigkeit sind die Reibungsverluste für den Betrieb zu groß.

Zwischen der Einschaltgeschwindigkeit $v_e$ und der Nenngeschwindigkeit $v_N$ wird die jeweilt maximale Leistung entzogen. Ab Windgeschwindigkeiten über $v_N$ wird nur noch die Nennleistung bereitgestellt.

Wird die Ausschaltgeschwindigkeit $v_A$ erreicht, muss die WKA abgeschaltet werden, da sonst die Rotorgeschwindigkeiten und wirkenden Kräfte zu hoch für die WKA sind.

# Regelung
**Stallregelung**
- Begrenzung der entommenen Leistung durch Strömungsabrriss
- Passiv: Rotorprofil sorgt für Strömungsabriss ab bestimmer Windgeschwindigkeit
- Aktiv: Drehbare Rotorblätter werden in ihrem Anstellwinkel verändert sodass es zum Strömungsabriss kommt

**Pitchregelung**
- Bei Überschreiten der Nennleistung werden die Rotorblätter leicht aus dem Wind gedreht
- Begrenzung der Leistung auf Nennleistung
- Zum Abschalten werden die Rotorblätter in Fahnenposition gestellt

# Antriebsstrang
Siehe [[Antriebsstrang]]

Es existieren WKA mit und ohne Getriebe. In WKA mit Getriebe wird die Rotordrehzahl erst auf höhere Drehzahlen umgesetzt und anschließend dem Generator zugeführt. In WKA ohne Getriebe sitzt der Rotor auf der Generatorwelle.

Als Generator können Synchron- und Asynchrongeneratoren genutzt werden.
Synchrongenerator:
- Vorteil: Höchste Regelbarkeit durch entkopplung der Antriebsseite von der Netzseite
- Nachteil:
	- Hohe Verluste im Umrichter
	- Höhere Kosten für Umrichter und Synchrongenerator

Asynchrongenerator:
- Vorteile:
	- Umrichter für ca. ein Drittel der Nennleistung ausgelegt
	- Geringere Verluste
- Nachteil: Aufwand der Regelung

# Windparks
siehe [[Windparkplanung]]

- Zusammenschluss mehrer WKA zu einem Windpark erzeugt Synergie-Effekte:
	- Schaffung von Infrastruktur zum Bau
	- Gemeinsame elektrische Anbindung ans Stromnetz
	- Geringerer logistischer Aufwand bei der Errichtung
- Aerodynamische Abschattung vermindert Ertrag der einzelnen WKA

Offshore ggü. Onshore:
- Vorteile
	- Höherer Windgeschwindigkeit
	- Weniger Turbulenz
	- Höheres Platzangebot als an Land
	- Höhere Akzeptanz
	- Großes Ausbaupotenzial
- Nachteile
	- Große Entfernung zur Küste
	- Aufwändige Fundamente
	- Rauere Umweltbedingungen
	- Zugänglichkeit und Logistik
	- Finanzierbarkeit großer Windparks
	- Schutz von Flora und Fauna

Gegen Ende der Laufzeit einer WKA kann **Repowering** durchgeführt werden, wobei alte Anlagen durch modernere und effizientere Anlagen ersetzt werden. Somit können diese WKA noch weit über die Lebensdauer hinaus betrieben werden. Ebenso hat Repowering eine hohe Akzeptanz in der Bevölkerung, da weniger Anlagen installiert werden, die Leistung jedoch steigt.

# Umweltauswirkungen
Siehe [[Windparkplanung#Behördliche Auflagen]]
- Veränderung des Landschaftsbilds
- Schattenwurf
- Schallemissionen
- Flächenverbrauch
- Störungen von Funk und Fernsehen, Radar
- Vogel-/Fledermausschlag

