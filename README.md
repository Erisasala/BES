# Datenbanken
Ein Datenbanksystem ist ein System zur elektronischen Datenverwaltung. Es
unterstützt die computergestützte Datenverarbeitung von Informationen die durch
eine Datenbankapplikation erzeugt und verarbeitet werden. Außerdem strukturiert es
und speichert diese Informationen in eine Datenbank ab.
Eine Datenbank dient der strukturierten Speicherung und Verwaltung von
Informationen, die einen Teilausschnitt aus der realen Welt abbilden und persistieren.
Durch eine Datenbank (DB) wird eine einheitliche und anwendungsneutrale Sicht auf
die Daten ermöglicht.

## Aufbau eines Datenbanksystems
Der Aufbau eines Datenbanksystems besteht aus einer **Datenbank (DB)**, welche die
**Datenbasis** darstellt, und aus einem **Datenbankmanagementsystem (DBMS)**.
Die **Verwaltungssoftware** organisiert intern die strukturierte Speicherung der Daten
und kontrolliert alle lesenden und schreibenden Zugriffe auf die Datenbank.
Ein **Datenbankmanagementsystem** abstrahiert die Details von Hard- und
Software-Komponenten eines Systems. Dadurch können Datenbanken
anwendungsunabhängig definiert, konstruiert und manipuliert (verändert) werden. Ein
Datenbankmanagementsystem (DBMS) bietet schnelle und effiziente Zugriffsverfahren,
um Daten verarbeiten zu können.
## Die zentralen Aufgaben eines Datenbanksystems
Die zentralen Aufgaben eines Datenbanksystems sind die Entgegennahme großer strukturierter
Datenmengen, deren Speicherung und Verwaltung sowie die Abfrage von Daten.
Um die komplexen und vielseitigen Anforderungen an eine konsistente und einheitliche Datenhaltung
zu erfüllen, müssen Datenbanksysteme eine Reihe von Merkmalen aufweisen. Die Anforderungen an
ein Datenbanksystem sind:
* **Datenunabhängigkeit:** Anwendungsprogramm und Datenhaltung sollten unabhängig
voneinander sein.
* **Effizienter Speicherzugriff:** Verwendung von Speichertechniken, um die
Datenverarbeitung effizient zu gestalten (z. B. Indizes).
* **Paralleler Datenzugriff:** Mehrere Benutzer müssen gleichzeitig auf die Daten zugreifen
können. Hierfür benötigt es Protokolle für Transaktionskontrollen.
* **Datenkonsistenz:** Eine Veränderung der Daten muss vollständig sein und zuvor definierte
Regeln einhalten.
* **Gemeinsame Datenbasis:** Die Daten werden zentral abgelegt und verwaltet.
* **Datenintegrität:** Daten müssen vollständig und den Regeln entsprechend korrekt sein,
ansonsten ist die Speicherung zu verhindern (z. B. Verweis auf einen nicht vorhandenen
Fremdschlüssel).
* **Datensicherheit:** Der Zugriff darf nur durch autorisierte Benutzer gestattet werden.
* **Wiederherstellungsverfahren:** Im Fehlerfall muss ein Backup- oder Recovery-Verfahren
zur Wiederherstellung einer konsistenten Datenbank vorhanden sein.
* **Abfragesprache:** Ein Datenbanksystem (DBS) muss eine Möglichkeit für die
Datenmanipulation (Abfrage, Aktualisierung, Berichtsgenerierung, Veränderung)
bereitstellen (bei relationalen DBS ist dies meist eine Form von SQL).
* **Keine / kontrollierte Redundanz:** Um Inkonsistenz und Integritätsverletzungen zu
vermeiden, sollte die redundante (mehrfache) Speicherung von identischen Daten
verhindert werden. In Ausnahmefällen kann Redundanz zur Performance-Optimierung
verwendet werden, dies sollte jedoch überwacht warden.

# MySQL versus MariaDB
Entwickler beider Datenbankmanagementsysteme ist *Michael "Monty" Widenius*. **MySQL** wurde 1994 entwickelt, **MariaDB** gibt es seit 2009. Beide begannen als Open Source Projekte. Die Kommerzialisierung von **MySQL** fand schrittweise statt. 2008 wurde **MySQL** an Sun Microsystems verkauft, jene Entwicklerfirma, wo auch Widenius und sein Team arbeiteten. 2010 kaufte Sun Microsystems dann Oracle und begann beide Systeme gewinnbringend zu vermarkten. Im Open Source Bereich geschah nur mehr wenig. Widenius und sein Team gründeten eine eigene Firma und begannen an dem frei zugänglichen **MySQL-Fork MariaDB** zu arbeiten. Maria ist der Name der zweiten Tochter des Entwicklers Widenius. Die neue Firma wurde (im Gegensatz zum Geschäftsmodell von Oracle) strikt unterteilt in einen kommerziellen Zweig, der *MariaDB-Corporation*, und einen Open Source (Community) Bereich – der MariaDB-Foundation
Die Ziele der MariaDB Foundation:
*	die **MySQL**-Talente unter einem Dach zusammenhalten
*	den Fortbestand der Community-Entwicklung fördern
*	sicherstellen, dass immer eine freie Version von **MySQL** existiert
**MariaDB** hat einen starken Fokus auf die offene Entwicklung. Im Vordergrund stehen zwei Grundsätze:
*	Der Quellcode von sich in der Entwicklung befindenden Programmteilen steht über öffentliche Respositorys zur Verfügung.
*	Alle Entwicklungsschritte werden öffentlich dokumentiert.
Die Datenbank-Managementsysteme **MySQL** und **MariaDB** basieren auf demselben Software-Kern. Bis **MySQL Version 7** waren beide Systeme kompatibel, d.h. Drop-In Replacement und sogar Upgrades sollten in beide Richtungen funktionieren. **MySQL 8** ist nicht mehr abwärtskompatibel, weder zu seinem eigenen System, noch zu **MariaDB**.

|    MERKMALE                                     |    MySQL                                                                                                 |    MariaDB                                                                                               |
|-------------------------------------------------|----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
|    Lizenz                                       |    Duales Lizenzsystem (Proprietär und GPL 2)                                                            |    GPL 2                                                                                                 |
|    Betriebssysteme                              |    Oracle Linux                                                                                          |    Arch Linux                                                                                            |
|                                                 |    Red Hat                                                                                               |    Red Hat/CentOS                                                                                        |
|                                                 |    CentOS                                                                                                |    Manjaro                                                                                               |
|                                                 |    Debian                                                                                                |    Debian                                                                                                |
|                                                 |    Ubuntu                                                                                                |    Ubuntu                                                                                                |
|                                                 |    Oracle Solaris                                                                                        |    openSUSE                                                                                              |
|                                                 |    SUSE Enterprise Linux                                                                                 |    SUSE Enterprise Linux                                                                                 |
|                                                 |    Microsoft Windows                                                                                     |    Microsoft Windows                                                                                     |
|                                                 |    Microsoft Windows Server                                                                              |    Microsoft Windows Server                                                                              |
|                                                 |    Apple macOS                                                                                           |    Apple macOS                                                                                           |
|                                                 |    FreeBSD                                                                                               |    Fedora                                                                                                |
|                                                 |    Solaris                                                                                               |    Mint                                                                                                  |
|    Programmiersprache                           |    C and C++                                                                                             |    C, C++, Bash und Perl                                                                                 |
|    Primäres Datenbankmodell                     |    Relationales Datenbankmodell                                                                          |    Relationales Datenbankmodell                                                                          |
|    Sekundäre Datenbankmodelle                   |    Dokumentenorientiertes Datenbankmodell                                                                |    Dokumentenorientiertes Datenbankmodell                                                                |
|                                                 |    Key-Value-Datenbank                                                                                   |    Key-Value-Datenbank                                                                                   |
|                                                 |                                                                                                          |    Graphenorientierte Datenbank                                                                          |
|    SQL-Schnittstelle                            |    Ja                                                                                                    |    Ja                                                                                                    |
|    NoSQL-Schnittstellen                         |    Ja                                                                                                    |    Ja                                                                                                    |
|    Protokoll                                    |    MySQL-Protokoll                                                                                       |    MySQL-Protokoll                                                                                       |
|    Replikation                                  |    Replikation mit GTID (Global Transaction Identifier)                                                  |    Replikation mit GTID (Global Transaction Identifier)                                                  |
|                                                 |    Master-Master-Replikation                                                                             |    Master-Master-Replikation                                                                             |
|                                                 |    Master-Slave-Replikation                                                                              |    Master-Slave-Replikation                                                                              |
|    In-Memory Unterstützung                      |    Ja                                                                                                    |    Ja                                                                                                    |
|    Routing                                      |    MySQL Router (GPLv2)                                                                                  |    MariaDB MaxScale (BSL)                                                                                |
|    Partitionierung (Sharding)                   |    Horizontale Partitionierung, Sharding mit MySQL Cluster oder   MySQL Fabric                           |    Horizontale Partitionierung, Sharding mit MySQL Cluster oder   MySQL Fabric                           |
|    SQL Management                               |    MySQL Workbench (Microsoft Windows, macOS und Linux)                                                  |    SQLyog von Webyog (Microsoft Windows, Linux)                                                          |
|    Monitoring                                   |    MySQL Enterprise Monitor (proprietär)                                                                 |    Monyog von Webyog (Microsoft Windows und Linux) (proprietär)                                          |
|    Verschlüsselung                              |    Verschlüsselung inaktiver Daten                                                                       |    Verschlüsselung inaktiver Daten                                                                       |
|                                                 |    - InnoDB-Tabellenräume                                                                                |    - InnoDB-Tabellenräume                                                                                |
|                                                 |                                                                                                          |    - InnoDB-Tabellen                                                                                     |
|                                                 |                                                                                                          |    - InnoDB-Log-Dateien                                                                                  |
|                                                 |                                                                                                          |    - Aria-Tabellen                                                                                       |
|                                                 |                                                                                                          |    - Temporäre Dateien                                                                                   |
|                                                 |                                                                                                          |    - Binlogs                                                                                             |
|    Rollenbasierte Zugriffskontrolle             |    Nein                                                                                                  |    Ja                                                                                                    |
|    Authentifizierung                            |    Authentifizierung via SHA-256                                                                         |    Authentifizierung via ed25519-Plugin                                                                  |
|    Datenmaskierung                              |    Via ProxySQL                                                                                          |    Via MariaDB MaxScale (BSL)                                                                            |
|    Firewall                                     |    Via MySQL Enterprise Firewall (proprietär)                                                            |    Via MariaDB MaxScale (BSL)                                                                            |
|    Auditing                                     |    Via MySQL Enterprise Audit Plugin (proprietär)                                                        |    Via MariaDB Audit Plugin                                                                              |
|    Analyse                                      |    Nein                                                                                                  |    Via MariaDB ColumnStore                                                                               |
|    Routing & Load-Balancing                     |    Via MySQL Router                                                                                      |    Via MariaDB MaxScale (BSL)                                                                            |
|    Backup                                       |    Via MySQL Enterprise Backup (proprietär)                                                              |    Via MariaDB Backup (ein Fork von Percona XtraBackup)                                                  |
|    Common Table Expression (CTE)                |    Ja                                                                                                    |    Ja                                                                                                    |
|    Fensterfunktion                              |    Ja                                                                                                    |    Ja                                                                                                    |
|    Temporale Tabellen mit Versionsverwaltung    |    Nein                                                                                                  |    Ja                                                                                                    |
|    Query Rewriting                              |    Ja                                                                                                    |    Nein                                                                                                  |
|    Datentypen                                   |    String (CHAR, VARCHAR, TINYTEXT, TEXT, MEDIUMTEXT, LONGTEXT,   ENUM, SET, BINARY, VARBINARY, JSON)    |    String (CHAR, VARCHAR, TINYTEXT, TEXT, MEDIUMTEXT, LONGTEXT,   ENUM, SET, BINARY, VARBINARY, JSON)    |
|                                                 |    Numerisch (BIT, TINYINT, SMALLINT, MEDIUMINT, INT, BIGINT,   DECIMAL, FLOAT, DOUBLE, BOOLEAN)         |    Numerisch (BIT, TINYINT, SMALLINT, MEDIUMINT, INT, BIGINT,   DECIMAL, FLOAT, DOUBLE, BOOLEAN)         |
|                                                 |    Datum/Zeit (DATE, DATETIME, TIMESTAMP, TIME, YEAR)                                                    |    Datum/Zeit (DATE, DATETIME, TIMESTAMP, TIME, YEAR)                                                    |
|                                                 |    Large Object Datatypes (TINYBLOB, BLOB, MEDIUMBLOB, LONGBLOB)                                         |    Large Object Datatypes (TINYBLOB, BLOB, MEDIUMBLOB, LONGBLOB)                                         |
|                                                 |    GEOMETRY                                                                                              |    GEOMETRY                                                                                              |
|                                                 |    POINT                                                                                                 |    POINT                                                                                                 |
|                                                 |    LINESTRING                                                                                            |    LINESTRING                                                                                            |
|                                                 |    POLYGON                                                                                               |    POLYGON                                                                                               |
|    Räumliche Datentypen                         |    MULTIPOINT                                                                                            |    MULTIPOINT                                                                                            |
|                                                 |    MULTILINESTRING                                                                                       |    MULTILINESTRING                                                                                       |
|                                                 |    MULTIPOLYGON                                                                                          |    MULTIPOLYGON                                                                                          |
|                                                 |    GEOMETRYCOLLECTION                                                                                    |    GEOMETRYCOLLECTION                                                                                    |
|                                                 |    InnoDB                                                                                                |    InnoDB/XtraDB                                                                                         |
|                                                 |    MyISAM                                                                                                |    MyISAM                                                                                                |
|                                                 |    MEMORY                                                                                                |    MEMORY                                                                                                |
|                                                 |    CSV                                                                                                   |    CSV                                                                                                   |
|    Datenbank-Engines                            |    Archive                                                                                               |    Archive                                                                                               |
|                                                 |    BLACKHOLE                                                                                             |    BLACKHOLE                                                                                             |
|                                                 |    Merge                                                                                                 |    Merge                                                                                                 |
|                                                 |    Federated                                                                                             |    FederatedX                                                                                            |
|        Offizielle Konnektoren                   |    ODBC                                                                                                  |    ColumnStore                                                                                           |
|                                                 |    C++                                                                                                   |    Aria                                                                                                  |
|                                                 |    C                                                                                                     |    Cassandra                                                                                             |
|                                                 |    ADO.NET                                                                                               |    CONNECT                                                                                               |
|                                                 |    JDBC                                                                                                  |    Mroonga                                                                                               |
|                                                 |    PHP                                                                                                   |    MyRocks                                                                                               |
|                                                 |    Python                                                                                                |    OQGRAPH                                                                                               |
|                                                 |    Perl                                                                                                  |    Sequence                                                                                              |
|                                                 |    Ruby                                                                                                  |    SphinxSE                                                                                              |
|                                                 |    Node.js                                                                                               |    Spider                                                                                                |
|                                                 |                                                                                                          |    TokuDB                                                                                                |
|                                                 |                                                                                                          |    ODBC                                                                                                  |
|                                                 |                                                                                                          |    C++                                                                                                   |
|                                                 |                                                                                                          |    C                                                                                                     |
|                                                 |                                                                                                          |    ADO.NET                                                                                               |
|                                                 |                                                                                                          |    JDBC                                                                                                  |
|                                                 |                                                                                                          |    PHP                                                                                                   |
|                                                 |                                                                                                          |    Python                                                                                                |
|                                                 |                                                                                                          |    Perl                                                                                                  |
|                                                 |                                                                                                          |    Ruby                                                                                                  |
|                                                 |                                                                                                          |    Excel                                                                                                 |
|                                                 |                                                                                                          |    JavaScript                                                                                            |
|                                                 |                                                                                                          |    Swift                                                                                                 |
|                                                 |                                                                                                          |    R                                                                                                     |

Wie man auch anhand der Tabelle sehen kann, ist **MariaDB** schon längst nicht mehr nur als Fork von **MySQL** anzusehen. Es hat **MySQL** in manchen Bereichen technologisch bereits überholt („War of Features“).
Besonders hervorzuheben an **MariaDB**, sind folgende Konzepte:
* Bietet dem Anwender eine optimalen Speicherengine für alle Anwendungsfälle - große Palette an Datenbankengines im Vergleich zu **MySQL**.

*	Sicherheit der der gespeicherten Daten. Seit Version 10.1 - Möglichkeit zur Verschlüsselung von Daten auf Storage-Ebene. Ganze Table-Spaces oder einzelne Tabellen, sowie verschiedenste Log-Dateien können verschlüsselt werden.

3.	Role-based Access Control – Zugriffsrechte werden nicht klassisch (wie bei **MySQL**) auf der Basis einzelner Benutzer vergeben, sondern anhand definierter Rollen, die ein Mitarbeiter im Unternehmen ausfüllt. Das erleichtert die Verwaltung - User muss nicht angelegt, sondern nur zugewiesen werden.

4.	Das mächtigste Tool von MariaDB ist MaxScale (Benannt nach Widenius’ Sohn). Er ist ein Datenbank-Router, der zum Load-Balancing von Clustern (System Galera), für Master-Slave-Replikationen und zukünftig auch als Firewall eingesetzt wird. MaxScale ist für den Anwender unsichtbar, er stellt eine normale Datenbankinstanz dar. Gegenüber dem Datenbank-Cluster, bildet MaxScale eine übergeordnete Schicht, die die Kommunikation zwischen Anwendung und Datenbanken steuert. Änderungen an den Datenbank-Clustern wirken sich nicht auf die Anwendungsschicht aus.

5.	Selbstoptimierung der MariaDB Datenbank –Generierung von Statistiken, unabhängig von der Speicherengine – diese fließen in Query-Optimizer ein. Anpassung an Unternehmensanforderungen.

**MariaDB** ist heute Standard in allen großen Linux Distributionen.

## PostgreSQL

PostgreSQL , oft kurz Postgres genannt, ist ein freies, objektrelationales Datenbankmanagementsystem (ORDBMS). Seine Entwicklung begann in den 1980er Jahren, seit 1997 wird die Software
von einer Open-Source-Community weiterentwickelt.
Eine Objektrelationale Datenbank (kurz ORDB), auch objektrelationales
Datenbankmanagementsystem (kurz ORDBMS) genannt, stellt das Bindeglied zwischen
klassischen relationalen Datenbanken und Objektdatenbanken dar. Sie kommen überall dort zum
Einsatz, wo Mengen von Objekten in Beziehung zu anderen Daten oder Objekten gebracht werden
müssen.
PostgreSQL nennt sich selbst "The world's most advanced open source database". PostgreSQL ist für
Linux, aber auch für alle anderen, gängigen Betriebssysteme wie MacOS, Windows und BSD
verfügbar.
PostgreSQL setzt den SQL-Standard 2008 sehr umfassend um. Neben den gängigen Datentypen kann
die Datenbank auch nativ mit XML umgehen und ab Version 9.2 auch mit Daten im JSON-Format:.
PostgreSQL ist weitgehend konform mit dem SQL-Standard SQL:2011, d. h. der Großteil der
Funktionen ist verfügbar und verhält sich wie definiert.
PostgreSQL ist vollständig ACID-konform *(inklusive der Data Definition Language), und unterstützt
erweiterbare Datentypen, Operatoren, Funktionen und Aggregate.
**ACID-konform** (atomacy, consistency, isolation, durability)
Das **ACID-Prinzip** beschreibt **sinnvolle Regeln zum effektiven und effizienten Umgang mit
Datenbanktransaktionen. Eine Datenbanktransaktion ist eine Sequenz von Operationen**, die
einzigartig und durchführbar sein muss.
* Atomicity oder Atomarität: Ausführung aller oder keiner Informationsteile einer Transaktion
* Consistency oder Konsistenz: Transaktionen erzeugen einen gültigen Zustand oder fallen in
den alten Zustand zurück
* Isolation oder Abgrenzung: Transaktionen verschiedener Anwender oder Prozesse bleiben
voneinander isoliert
* Durability oder Dauerhaftigkeit: Nach einer erfolgreichen Transaktion bleiben die Daten
dauerhaft gespeichert
Obwohl sich die Entwicklergemeinde sehr eng an den SQL-Standard hält, gibt es dennoch eine Reihe
von PostgreSQL-spezifischen Funktionalitäten, wobei in der Dokumentation bei jeder Eigenschaft ein
Hinweis erfolgt, ob dies dem SQL-Standard entspricht, oder ob es sich um eine spezifische
Erweiterung handelt. Darüber hinaus verfügt PostgreSQL über ein umfangreiches Angebot an
Erweiterungen durch Dritthersteller, wie z. B. PostGIS zur Verwaltung von Geodaten.
PostgreSQL ist in den meisten Linux-Distributionen enthalten. Apple liefert von der Version Mac OS X
Lion (10.7) an PostgreSQL als Standarddatenbank aus.

## Oracle 
Oracle wurde im Jahr 1977 von Larry Ellison gegründet und ist zurzeit das populärste relationale Datenbankmanagemantsystem
Programmiersprache:
* Assemblersprache
*	C
*	C++
*	Java
Unterstützte Betriebssysteme:
*	Linux
*	Windows
*	Solaris
*	HP-UX
*	AIX
Verschiedene Editionen:
*	Enterprise -> enthält alle Features (am teuersten)
*	Standard -> enthält standard Features
*	Express -> gratis (sehr stark eingeschränkt)
*	Lite -> für mobile Geräte
Für Studienzwecke ist Oracle frei erhältlich
War die erste Datenbank welche für Grid-Computing ausgelegt wurde (Kosten- und Ressourcensparend)
Implementierung der ACID-Eigenschaften (atmoicity, consistency, isolation, duarbility)
*	atmoicity -> kann eine Transaktion nicht vollständig durchgeführt werden, wird ein Rollback ausgeführt, d.h. auch erfolgreiche Teile der Tansaktion werden zurückgesetzt (Alles oder Nichts Prinzip)
*	consistency -> Integritätsbedingungen werden vor dem Abschluss der Transaktion überprüft
*	isolation -> parallel laufende Transaktionen beeinflussen einander nicht
*	duarbility -> gewährleistet dass Daten nach einer Transaktion dauerhaft in der Datenbank gespeichert sind

Java kann innerhalb der Datenbank ausgeführt werden
Gespeicherte Prozeduren erfolgen in PL/SQL oder Java
Unterstützung von regulären Ausdrücken

Abweichungen des ANSI-SQL-Standards:
*	Datentyp „date“ enthält zusätzlich die Uhrzeit
*	Datentyp „boolean“ ist nicht vorhanden
*	Leerzeichen und NULL werden nicht  unterschieden
Lizenzeirung:
*	abhängig von der Anzahl der Prozessorkerne
*	abhängig von der Anzahl der möglichen Benutzer
Die Lizenzeirung ist sehr teuer und daher ein großer Nachteil von Oracle
Neuere Versionen beinhalten die Features der älteren Versionen, d.h. alte Datenbanken sind auch mit der aktuellsten Version kompatibel

## BigTable
BigTable  unterstützt das MapReduce-Verfahren und stellte die Grundlage von vielen Google-Produkten, wie etwa Google Maps, Google Bücher, YouTube oder Google Earth, dar. Besonderer Wert wurde auf Skalierbarkeit und Geschwindigkeit gelegt. Die Datenbank basiert deshalb auch auf einer nichtrelationalen Struktur.
Charakteristisch für in BigTable gespeicherte Daten ist, dass sehr häufig Datensätze hinzugefügt werden, vorhandene Datensätze aber sehr selten geändert werden. Eine BigTable besteht grundlegend aus sehr vielen Zeilen. Innerhalb einer Zeile können beliebig viele Spalten definiert werden.
Eine Bigtable ist eine spärlich verteilte, beständige, mehrdimensional sortierte Mappe. Die Mappe wird durch eine Zeile Schlüssel, Spaltenschlüssel und ein Zeitstempel indiziert. Jeder Wert in der Mappe ist ein nicht interpretiertes Array von Bytes.
Konsistente Latenzzeit unter 10 ms


## Integration
Cloud Bigtable kann in das Apache-Ökosystem und andere Google Cloud-Produkte integriert werden. Im GCP-Ökosystem kann BigQuery Daten abfragen, die in einer Cloud Bigtable-Datenbank gespeichert sind. Mit Cloud Dataflow können Sie Daten verarbeiten, die in Cloud Bigtable gespeichert sind, oder die Ausgabe Ihrer Cloud Dataflow-Pipeline speichern. Die Cloud Bigtable-Unterstützung für die HBase-API ermöglicht eine Schnittstelle mit einer Reihe von Funktionen wie Apache Beam für die Datenverarbeitung, JanusGraph für die grafische Analyse und OpenTSDBTM für die Zeitreihenanalyse.
## Vorteile von BigTable sind: 	

*	Konsistente Latenzzeit unter 10 ms
*	Die Replikation sorgt für höhere Verfügbarkeit, höhere Haltbarkeit und Ausfallsicherheit bei Zonenausfällen
*	Ideal für Ad Tech, Fintech und IoT
*	Einfache Integration mit Open-Source-Big-Data-Tools
*	Schnell und performant
*	Nahtlose Skalierung und Replikation
*	Einfach und integriert


# Quelle
[http://www.datenbanken-verstehen.de/lexikon/datenbanksystem/]

[https://cloud.google.com/bigtable/]

[https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf]

[https://de.wikipedia.org/wiki/Google_BigTable]

[http://datenbanken-verstehen.de/]

[https://en.wikipedia.org/wiki/Oracle_Database]

[https://docs.oracle.com/cd/B19306_01/server.102/b14220/intro.htm]

[https://www.techopedia.com/definition/8711/oracle-database]

[https://www.ionos.de/digitalguide/hosting/hosting-technik/mariadb-vs-mysql/ ]

[https://www.informatik-aktuell.de/betrieb/datenbanken/mariadb-und-mysql-vergleich-der-features.html]
