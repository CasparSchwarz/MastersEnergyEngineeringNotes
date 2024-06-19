Zur Sicherheit von Batteriepacks werden diese mit Warnhinweisen versehen und Kennzeichnungen angegeben:
- Seriennummer
- Nennspannung
- Nennkapazität
- Maximale Spannung bei Standardbedingungen
- Maximaler Strom bei Standardbedingungen

# Standardtests an Batteriepacks
Elektrische Prüfungen:
- Isolationstest (Isolationswiderstand, Durchschlagfestigkeit)
- Funktionstests ( Zyklentests, Überlade- & Tiefenladetests, Tests unter Ein-Fehler Bedingung)
- Aufbau (Kriechstrecken, Einzelteile, Feuerfestigkeit, Dichtigkeit)

Mechanische Prüfungen:
- Kurzschluss
- Stoffaustritt
- Brand
- Bersten
- Explosion
- Rütteltest

UN Transporttests (Tests, die erfüllt werden müssen, damit eine Batterie transportiert werden darf)
# Sicherheit auf Zellebene
Je nach Zelltyp sind unterschiedliche Sicherheitsmechanismen integriert. Moderne Zylindrische Zelle haben dabei ein hohes Maß an intrinsischer Sicherheit (durch die Aufnahme von hohen Drücken). Pouch-Bag Zellen und prismatische Zellen haben quasi keine Sicherheitsfeatures.

Um auf Zellebene im sicheren Bereich zu bleiben, darf die Kathode nicht zu stark entladen werden (bis maximal 60 % Entladung), da das Kathodenmaterial sonst instabil wird. Beim Entladen kann es nur durch Unterschreiten der Entladeschlussspannung zu Korrosionseffekten oder zur Entstehung von Kurzschlüssen in der Batterie kommen. (siehe [[Lithium-Ionen Batterien#Batteriesicherheit]])

![[Pasted image 20240619124018.png]]

Der **thermal Runaway** tritt auf durch
- einen internen Kurzschluss
- Externen Kurzschluss
- Überladung
- Tiefentladung
- Überlast
- Wärmeeintrag von außen

wodurch die Erwärmung der Batterie in einen selbst-verstärkenden Kreislauf gerät, in dem die Temperatur der Batterie immer weiter bis hin zur Explosion steigt.

# Sicherheitsmechanismen innerhalb der Zelle
- aktiv
	- Thermomanagement
	- Spannungsüberwachung
	- Lademanagement
- passiv
	- Überdruckventil
	- Keramischer Separator
	- Strombgrenzung

Schmelzsicherung
- Stromabhängiges Abschalten bei Überlast
- Stromabhängiges Abschalten bei externem oder internem Kurzschluss

Thermosicherung
- Temperaturabhängiges Abschalten des Stromes
- Abschaltung erfolgt weitestgehend Stromunabhängig
- Einsatz in Batteriepacks von Laptops

PTC-Widerstand (Positive Temperature Coefficient)
- Schreibenförmiger Temperaturabhängiger Widerstand
- Begrenzung des Stromes
- Erhöht den Innenwiderstand der Zelle
- Reversible Sicherung, schützt vor externen Kurzschlüssen

Überdruckventil
- Verdampfender Elektrolyt entweicht in hohles VOlumen um den positiven Kontakt
- Schweißverbindung zwischen konkavem Blech und positivem Kontakt reißt ab
- Überdruck wird abgegeben, aber Zelle wird irreversibel zerstört