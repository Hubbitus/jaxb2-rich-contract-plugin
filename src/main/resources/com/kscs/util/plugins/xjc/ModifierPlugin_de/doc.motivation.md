Generell ist es vorteilhaft, Anwendungslogik so zu implementieren, dass Objekte in der Regel nach der
Initialisierung in ihrem Zustand unver�nderlich sind. In traditionellen Programmiersprachen wie z.B.
Java bleibt dies jedoch oftmals ein akademischer Ansatz, da oft auf bestehendem Code und bestehenden Bibliotheken
aufgesetzt werden muss, die ein derartiges Programmiermodell nicht oder nur unzul�nglich unterst�tzen.

Das `modifier`-Plugin schafft eine M�glichkeit, einerseits (z.B. durch das `immutable`-Plugin) die allgemeine
Schnittstelle einer Klasse so zu definieren, dass dar�ber keine Zustands�nderungen am Objekt m�glich sind,
aber gleichzeitig f�r bestimmte Szenarien eine explizit abzurufende Referenz bereit zu stellen, �ber die das
Objekt dennoch einfach ver�ndert werden kann.

Der Einsatz dieses Plugins ist haupts�chlich f�r eine �bergangszeit w�hrend der Refaktorierung von existierendem
Code vorgesehen, sodass zur Compilezeit die Stellen im Code deutlich werden, die zustandsver�nderliche
Objekte voraussetzen. Ziel sollte es dann sein, dieses Plugin irgendwann im eigenen Projekt abschalten zu k�nnen.