Supercaps sind elektrochemische Doppelschichtkondensatoren. Sie besitzen eine sehr geringe Energiedichte, haben jedoch eine sehr hohe Leistungsdichte.

Supercaps bestehen aus Kohlenstoff mit sehr hoher Oberfläche (2000 m^2/g). Zudem wird ein geringer Abstand zwischen Ionen und Kohlenstoff realisiert. Supercaps sind aus zwei Elektronen, die durch einen Separator getrennt sind, aufgebaut. Dabei wird das Kohlenstoffpulver mit einer Paste auf die Elektroden aufgetragen.

Die Kapazität des Kondensators ist Abhängig von der Oberfläche und des Elektrodenabstands:
$$
C=\varepsilon_0\varepsilon_r\frac Ad
$$
Die Energiemenge ist von der Kapazität und der Spannung abhängig:
$$
E=\frac 12 CU^2
$$
Ebenso wie die Ladungsmenge:
$$
Q=CU
$$

Energie wird dabei durch Verschiebung und Anlagerung der Ionen an das Aktivmaterial gespeichert. Somit findet keine Reaktion statt, sodass die Lebensdauer deutlich Oberhalb der von Batterien ist.

Es werden organische Elektrolyten verwendet. Diese bestehen aus einem Lösungsmittel (Acetonitrile, Propylene-Karbonat) und Leitsalzen (0,5 M bis 2 M). Typische Leitfähigkeiten solcher Elektrolyten liegen im Bereich von 10 bis 60 mS/cm.

Bei der Entsorgung von Supercaps muss darauf geachtet werden, dass die Elektrolyten gesundheitsschädlich sind. Zudem kann fast nur das Elektrodenmaterial rezykliert werden, der Rest wird thermisch verwertet.

**Vergleich LiIon zu Supercap**

|                    | Lithium-Ionen Batterie | Supercap        |
| ------------------ | ---------------------- | --------------- |
| positive Elektrode | Li Metalloxid          | Kohlenstoff     |
| negative Elektrode | Graphit                | Kohlenstoff     |
| Elektrolyt         | organisch              | organisch       |
| Speicherprinzip    | chemisch               | elektrostatisch |
| Zellspannung       | 3,6 - 4,2 V            | 2,5 - 2,8 V     |
| Energiedichte      | > 100 Wh/kg            | 5 Wh/kg         |
| Leistungsdichte    | 1000 W/kg              | > 5000 W/kg     |
# Eigenschaften & Bauformen
Supercaps haben eine hohe Leistungsfähgikeit, können jedoch nur wenig Energie speichern. Die Zyklenlebensdauer liegt bei 10^5 bis 10^6. Auf der anderen Seite ist die temperaturbedingte Alterung sehr stark bei Supercaps (Halbierng der Lebensdauer mit 7 K Temperaturanstieg).

Typischerweise werden Supercaps mit konstanter Leistung entladen. Dabei wird der Kondensator zwischen Nennspannung und halber Nennspannung betrieben. Das bedeutet, dass bei konstannter Leistung die Stromstärke im Betrieb verdoppelt wird, und somit die Wärmeverluste vervierfacht.

Um Supercaps anwenden zu können, werden die Zellen zu Modulen zusammengebaut. Die Kapazität des Moduls sinkt linear mit der Zahl der Zellen. Die Spannung steigt jedoch linear mit der Anzahl der Zellen und die Energie quadratisch mit der Spannung.
# Alterung
Die Lebensdauer eines Supercaps ist stark abhängig von der Betriebsspannung und der Umgebungstemperatur. Dabei verkürzen hohe Spannungen und Temperaturen die Lebensdauer. Es ist zu beachten, dass hohe Spannungen jedoch in einigen Fällen genutzt werden können, solange es nicht im Dauerbetrieb geschieht.

Der wesentliche Alterungsprozess ist die **Zersetzung des Elektrolyten**. Die chemischen Prozesse zur Zersetzung des Elektrolyten laufen doppelt so schnell ab bei
- Temperaturerhöhung um 10 K
- Spannungserhöhung um 100 mV

Temperaturerhöhungen können durch Spannungsabsenkung kompensiert werden. Das geht jedoch mit einem Energieverlust einher, sodass die Kapazität des Kondensators erhöht werden muss.

Bei beschleunigten Alterungstest können andere Alterungseffekte auftreten, als es im Anwendungsfall der Fall ist. Bspw. ein Aufblähen des Zellgehäuses aufgrund der Zersetzung des Elektrolyten.
## Selbstentladung
- Spannungsabfall hängt stark von der Vorgeschichte ab
	- Ladedauer, Lade/Entlade-Vorgeschichte, Temperatur, Anfangsspannung
- Spannungsabnahme besteht aus mehreren Phasen:
	- Exponentiell: Zeitkonstanten von Stunden und Tagen
	- Lineare Abnahme nach mehreren Monaten
- Ladungsgehalt hängt hauptsächlich von der Spannung ab
- -> Erklärung für den schnellen Selbstentlademechanismus: Ionen-Umverteilung
- Immer noch sind viele Fragen offen:
	- Wie funktioniert der Ladungsverlust? -> Langsamer Mechanismus?
	- Richtige Annahme, dass C=const?
	- Warum verhalten sich die beiden untersuchten Zelltypen so unterschiedlich?

# Modellierung
Zur Modellierung von Kondensatoren wird ein elektrisches Ersatzschaltbild verwendet:
![[Pasted image 20240708163219.png]]
Wobei:
- $R_S$: Serienwiderstand, Innenwiderstand
- $R_P$: Parallelwiderstand, Selbstentladung
- $L$: Induktivität (meist vernachlässigbar)
- $C$: Kapazität

Wird das Aktivmaterial betrachtet, besteht dieses aus vielen kleinen Poren, die durch das Graphit entstehen:
![[Pasted image 20240708170123.png]]
Es wird unterschieden zwischen
- Makroporen (d > 500 Anstrom)
- Mesoporen (20 < d < 500 A)
- Mikroporen (d < 20 A)

An jeder Pore liegen positive und negative Ladungsträger an, sodass jede Pore als eigener Kondensator modelliert werden kann.
![[Pasted image 20240708170316.png]]
![[Pasted image 20240708170612.png]]
Während des Ladens ändert sich die Verteilung der Ionen in den Poren. Sind die Ionen gleichmäßig verteilt, ist ein Zustand geringster Energie und somit geringster Ladung erreicht.

Ein solches System zu modellieren ist quasi unmöglich, da weder Informationen über die Geometrie bestehen, noch Rechenkapazität zur Verfügung steht um solche Modelle durchzurechnen. Dementsprechend werden die Makro, Meso und Mikroporen zusammengefasst betrachtet:
![[Pasted image 20240708171342.png]]
Dabei werden die Poren der Größe nach absteigend aufgeladen:
1. Macro
2. Meso
3. Micro

Da die Widerstände der großen Poren kleiner ist als die der kleinen.
# Ladungsausgleichsysteme
Warum ist ein Ladungsausgleich in Kondensatoren notwendig?
- Unterschiedliche Selbstentladung
- Unterschiedliche Kapazitäten
- Schutz vor Übersüannung
- Erhöhung der Lebensdauer

Es gibt 3 Typen von Ausgleichsystemen:
- Passive Ausgleichsysteme
- Gesteuerte Passive Auslgeichsysteme
- Aktive Ausgleichsysteme

## Passive Ladungsausgleichsysteme
In diesem System wird der Kondensator langsam entladen, bis alle Zellen komplett entladen sind. **AUF KEINEN FALL FÜR LI-ION BATTERIEN**

Hierbei sorgen Zählerdioden dafür, dass ab einer Bestimmten Spannung nur Strom über die Dioden fließt und nicht mehr durch den Kondensator.

- Topologien
	- Parallel-Widerstände
	- Z-Dioden
- Vorteile
	- Preisgüstig
	- Einfache Herstellung
- Nachteile
	- Langsam
	- Schlechter Wirkungsgrad
	- Relativ große Verluste
	- Temperaturabhängigkeit der Schwellspannung der Z-Dioden

## Aktive Ladungsausgleichsysteme
- Topologien
	- Hoch-Tiefsetzsteller
	- Multiplexer und Kondensator
	- Galvanisch getrennten Spannungsquellen
- Vorteile
	- Umleitung der Energie
	- Hoher Wirkungsgrad
- Nachteile
	- Komplizierte Steuerung
	- Zusätzliche Bauteile nötig
	- Relativ teuer

## Gesteuerte Passive Ausgleichsysteme
- Stand der Technik
- Bestandteile
	- Kompoarator
	- Schalter
	- Bypass-Widerstand
- Vortiele
	- Einfach
	- Kostengünstig
- Nachteile
	- Langsamer Ausgleich
	- Keine Temperaturkorrektur
	- Schlechter Wirkungsgrad