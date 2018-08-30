## group-contract
### Bugs
Currently none known

### Aktivierung
#### -Xgroup-contract

#### Optionen

##### -declareSetters=`{y|n}` (y)
Auch die Setter-Methoden in den generierten Interfaces deklarieren. Wenn nein, werden nur Getter deklariert.


##### -declareBuilderInterface=`{y|n}` (y)
Wenn das "fluent builder plugin" (-Xfluent-builder) ebenfalls aktive ist, generiere auch Interfaces f�r die inneren Builder-Klassen.


##### -supportInterfaceNameSuffix=`<string>` (Lifecycle)
Methoden, die zu Typkonflikten f�hren k�nnen, wenn zwei oder mehr interfaces aus diesem Generat gleichzeitig(mit "&") als Grenzen generischer Typparameter verwendet werden, werden in ein eigenes Interface ausgelagert, dessen Name dann mit dem angegebenen Wortbestandteil endet.


##### -upstreamEpisodeFile=`<string>` (META-INF/jaxb-interfaces.episode)
Suche die angegebene "episode"-Datei (Resource-Pfad), um Informationen �ber interfaces zu erhalten, die in Modulen definiert wurden, von denen dieses hier abh�ngig ist (siehe "-episode"-Mechanismus in der XJC-Dokumentation).


##### -downstreamEpisodeFile=`<string>` (/META-INF/jaxb-interfaces.episode)
Generiere "episode"-Datei f�r abh�ngige Module an der angegebene Stelle (Resource-Pfad).

