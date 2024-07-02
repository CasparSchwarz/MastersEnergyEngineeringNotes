Photovoltaik nutzt direkte und diffuse Sonnenstrahlung um elektrischen Strom zu produzieren. Somit eignet sich PV auch für bedeckte Tage, an denen nur diffuses Licht zur Verfügung steht.
# Physikalische Grundlagen
PV basiert auf dem photoelektrischem Effekt. Dabei reicht die Energie eines Photons aus, um Elektronen aus der Gitterstruktur eines Materials rauszuschlagen.
$$
E=hf=h\frac c \lambda
$$
Bei dem photoelektrischen Effekt werden Elektronen aus dem Valenzband in das Leitungsband gehoben. Die Elektronen im Leitungsband werden anschließend abgeführt und dem Valenzband wieder zugeführt, sodass ein Stromfluss entsteht. Bei Halbleitern liegt die Energiemenge zum Herauslösen eines Elektrons liegt zwischen 0,1 eV und 3 eV.

Um Halbleiter nutzen zu können, müssen diese dotiert werden:
- p-dotiert: Freie Löcher, Silizium dotiert mit Elementen mit 3 Valenzelektronen
- n-dotiert: Freie Elektronen, Silizium dotiert mit Elementen mit 5 Valenzelektronen

![[Pasted image 20240702174718.png]]

Wird mehr Energie durch die Sonne geliefert, als für das Anheben notwendig, so kommt es zu Verlusten und die überschüssige Energie wird in Wärme umgewandelt.
![[Pasted image 20240702174950.png]]
Somit gibt es einen maximalen Wirkungsgrad für herkömmliche Solarzellen, welcher bei ca. 33 % liegt (Shockley-Queisser-Grenze). Dieser Wirkungsgrad kann erhöht werden durch Kaskadenanordnung der Zellen (Multijunction-Solarzellen).
![[Pasted image 20240702175238.png]]
# Kennlinien und Verschaltung von PV
Aufbau eines kristallinen PV-Moduls:
![[Pasted image 20240702175311.png]]
![[Pasted image 20240702175330.png]]

Über das elektrische Ersatzschaltbild einer realen Solarzelle können die Einzelnen Ströme beschrieben werden:
![[Pasted image 20240702175557.png]]
- Photostrom $I_{ph}$ beschreibt die durch optische Anregung generierten Ladungsträger
- Diffusionsstrom $I_d$ und Rekombinationsstrom $I_r$ vermindern den Photostrom um die Elektronen, die nicht an die Oberfläche gelangen
- Reihenwiederstnad $R_S$ umfasst Widerstand des Halbleitermaterials, der Metallkontaktierung und Kontaktwiderstände
- Parallelwiderstand $R_P$ beschreibt Leckströme am p-n-Übergang

Die Strom-Spannungs-Kennlinie beschreibt den Stromabfall bei zunehmnder Spannung. Der Maximum Power Point (MPP) ist dabei der Punkt maximaler Leistung. Der Füllfaktor beschreibt dabei das Verhältnis von MPP zu dem Produkt aus Leerlaufspannung und Kurzschlussstrom:
$$
F=\frac{MPP}{I_kU_0}
$$

In einer **Reihenschaltung** addiert sich die Spannung der Zellen, in einer **Parallelschaltung** addiert sich der Strom der Zellen.
# Komponenten
Um eine PV-Anlage zu installieren sind folgende Komponenten notwendig:
- PV-Module
- Wechselrichter (Wandlung Gleichspannung zu Wechselspannung, verlustbehaftet)
- PV-Zähler
- Zwei-Energierichtungszähler
- Monitoring-System

Bei Bränden behindern hohe Spannungen und Ströme die Löscharbeiten, da selbst nach Unterbrechung der Verbindung eine Spannung an den PV-Modulen erzeugt wird.

PV kann entweder fest ausgerichtet oder nachgeführt ausgeführt werden.
# Halbleitermaterialien und alternative Techniken
## Silizium
Bei Silizium eignen sich folgende Arten von Silizium:
- monokristallin
- polykristallin
- amorph

Dabei haben monokristalline Zellen den höchsten Wirkungsgrad (ca. 17 %), sind aber auch in der Herstellung aufwendig und am teuersten.

Polykristalline Zellen bestehen aus mehreren Kristallen die unterschiedliche Orientierungen aufweisen. Wirkungsgrad ca. 15 %.

Amorphe Zellen bestehen aus einer dünnen nichtkristallinen Siliziumschicht. Diese haben einen niedrigen Wirkungsgrad und degradieren mit der Zeit, sind aber sehr kostengünstig.
## Cadmium-tellurid
- Bei diffuser, schwacher Bestrahlung bessere Wirkungsgrade als Silicium
- Geringe Empfindlichkeit ggü. Temperaturschwankungen
- Nur geringer Marktanteil
- CdTe ist gesundheitsschädlich
## Galliumarsenid
- Arsen ist giftig
- Teurer und seltener als Quarzsand (Silicium)
- Aufwendige Kristallzüchtung
- Komplexe Entsorgung
- Auf Spezialgebiete beschränkt wie Satelliten
## Perowskit (CaTiO3)
- Geringe Herstellungskosten
- Hoher Wirkungsgrad (> 22 %)
- Geringe Haltbarkeit und hohe Degradation
- Empfindlich ggü Feuchtigkeit
## Kupfer-Indium-Gallium-Dielenid (CIGS)
- Sehr dünne Schichten (1 - 2 µm) -> Biegsam
- Indium is selten
- Wirkungsgrad bis zu 22,6 %
## Multijunction Zellen
Bei diesen Zellen absorbieren unterschiedliche Schichten unterschiedliche Wellenlänge und lassen die jeweils anderen Wellenlänge hindurch. Damit werden Satelliten oder Concentrator PV-Module gebaut und Wirkungsgrade von 46 % erreicht.
## Konzentrator PV
Hierbei wird Sonnenlicht auf einen Kollektor konzentriert, wodurch Wirkungsgrade von über 40 % erreicht werden. Dabei ist eine Kühlung der Zelle unbedingt notwendig, damit diese nicht unter der thermischen Belastung zerstört wird.
## Organische Zellen
Organische Zellen bestehen aus Kohlenwasserstoffen und haben die Eigenschaft, durchsichtig zu sein. Zudem sind diese Zellen sehr dünn, sodass diese ebenfalls flexibel und leicht sind -> Dadurch quasi unzerbrechlich. Zudem ist der ökologische Fußabdruck klein.
# Nachahltigkeit
Die energetische Amortisationszeit wird wie folgt berechnet:
$$
\tau=\frac{KEA}{\bar P_{el}}
$$
Sie gibt an, ab welcher Zeit die Energie zur Produktion, Betrieb und Rückbau der PV-Zelle wieder erzeugt wurde.

Typische Werte:
- Norderuopa: ca. 2,5 Jahre
- Südeuropa: ca. 1,5 Jahre

Da die Lebensdauern typischerweise im Bereich von 20 bis 30 Jahren liegen, erzeugt eine PV-Anlage ca. 10 Mal mehr Energie als zu ihrer Herstellung benötigt wurde. Auf den Lebenszyklus betrachtet kommt man somit auf einen CO2 Footprint von ca. 32 g/kWh.