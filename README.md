# Software Praktikum - Java-Projekt

Dieses Repository dient zum einfachen Start in das Software Praktikum der [Fachschaft Geoinformatik](https://geofs.uni-muenster.de/) des Institut für Geoinformatik, Münster. Ziel des Praktikums ist die Entwicklung eines Navigationssystems in der Programmiersprache Java. Dabei dürfen (und sollen) externe Softwarebibliotheken (APIs) genutzt werden. Eine beispielhafte Auswahl ist am Ende dieses Dokuments gelistet. Desweiteren finden sich hier Einleitungen und Links zu Dokumentationen / Spezifikationen von agilen Arbeitsweisen in der Softwareentwicklung.

## Inhalt

* [Agiles Arbeiten](#agiles-arbeiten)
* [APIs](#apis)

## Agiles Arbeiten

Unter agiler Softwareentwicklung versteht man die transparente und flexible Arbeitsweise, welche sich von früheren Methoden unterscheidet. Viele Softwareprojekte scheitern daran, dass den am Projekt beteiligten Parteien nicht klar ist, was sie für Anforderungen an die Software hat bzw. was die andere Partei für Erwartungen und Denkweisen hat. So wurden, z.B. in einem Lastenheft, Anforderungen aufgelistet, welche dann abgearbeitet worden sind, ohne dass eine Kommunikation zwischen Kunden und Entwicklern stattgefunden hat. Änderungswünsche mussten daher im Nachhinein aufwändig umgesetzt werden und ließen nicht selten den Budgetrahmen explodieren.

Wichtig ist vor allem bei der Entwicklung einer Software, dass man nicht sofort drauf los programmiert sondern sich zunächst Gedanken über die Architektur macht. So sollten Klassen und Schnittstellen erst in einer abstrakten Weise definiert werden, bevor deren Implementierung stattfindet. Eine sehr hilfreiche Arbeitsweise ist dabei die [testgetriebene Entwicklung](https://de.wikipedia.org/wiki/Testgetriebene_Entwicklung). Dabei werden erst die Testfälle erstellt und gegen diese dann entwickelt. Der große Vorteil hierbei ist, dass die Projektziele bereits mit den Tests sichergestellt werden können und nicht in die falsche Richtung entwickelt wird und Fehler frühzeitig erkannt werden können.

Eine inzwischen sehr populär gewordene agile Arbeitsweise ist Scrum, welche im folgenden Abschnitt kurz zusammengefasst wird.

### [Scrum](https://de.wikipedia.org/wiki/Scrum)

Beim Scrum (aus dem Englischen für Gedränge) wird in die Softwareentwicklung in kleine Aufgaben eingeteilt, welche in ein Backlog wandern. Dieser Backlog beschreibt die Gesamtheit an Aufgaben, welche zur Erreichung des Projektziels abgearbeitet werden müssen. Dabei ist das Backlog kein festgeschriebener Block von Aufgaben, sondern kann erweitert, reduziert und geändert werden. Ziel ist das transparente Arbeiten mit dem Kunden bereits während der Entwicklung, um auf Änderungswünsche schnell reagieren zu können. Die einzelnen Aufgaben werden dann in Sprints abgearbeitet. Ein Sprint ist eine feste Zeiteinheit, in welcher eine ausgewählte Menge an Aufgaben bearbeitet wird. Das optimale Ziel ist hierbei, dass nach jedem Sprint eine neue Version der Software released werden könnte. Das Entwicklerteam besteht aus drei Mitgliedern mit drei Rollen. So gibt es den/die Produkt Owner, welche/r für die Software verantwortlich ist und dadurch sicherstellt, dass die Entwicklung in die gewünschte Richtung verläuft. Dann gibt es den Scrum Master, dessen Hauptaufgabe es ist, sicherzustellen, dass die Entwickler (die die 3. Rolle stellen) ohne Störungen ihre Arbeit machen können.

2001 wurden die folgenden Leitsätze als [Agiles Manifest](https://de.wikipedia.org/wiki/Agile_Softwareentwicklung#Werte) formuliert, die auch ganz besonders für Scrum gelten:

„Wir erschließen bessere Wege, Software zu entwickeln, indem wir es selbst tun und anderen dabei helfen. Durch diese Tätigkeit haben wir diese Werte zu schätzen gelernt:
* Individuen und Interaktionen stehen über Prozessen und Werkzeugen
* Funktionierende Software steht über einer umfassenden Dokumentation
* Zusammenarbeit mit dem Kunden steht über der Vertragsverhandlung
* Reagieren auf Veränderung steht über dem Befolgen eines Plans
Das heißt, obwohl wir die Werte auf der rechten Seite wichtig finden, schätzen wir die Werte auf der linken Seite höher ein.“

### [Kanban](https://de.wikipedia.org/wiki/Kanban_(Softwareentwicklung))

Kanban ist eine Methode zur Verwaltung der Aufgaben in einem Projekt. Dabei lässt sich die Methode wie folgt kurz zusammenfassen:

Es gibt drei Spalten, unter welchen die Aufgaben einsortiert werden. Die erste Spalte umfasst die Aufgaben, welche noch abgearbeitet werden müssen. In die nächste Spalte werden dann die Aufgaben geschoben, welche sich aktuell in Bearbeitung befinden. Ist eine Aufgabe dann abgeschlossen, so wird sie in die letzte Spalte verschoben. Durch dieses System ist es auch für Projektaußenstehende relativ einfach zu erkennen, in welchem Zustand sich ein Projekt gerade befindet und an welchen Aufgaben gerade gearbeitet wird.

Ein kostenloses Tool für diese Methodik, welches auf für dieses Praktikum empfohlen wird, ist [Trello](https://trello.com/de).

## APIs

Dieser Abschnitt listet eine kleine Auswahl an APIs, welche zur Routenberechnung und -visualisierung genutzt werden können. Alle hier gelisteten APIs sind kostenlos nutzbar und manche in Teilen auch Open Source. Eine Registrierung ist oftmals zur Nutzung erforderlich, um einen API-Key zu erhalten, mit welchem Abfragen an den jeweiligen Dienst gestellt werden können.

### [GrapHopper](https://www.graphhopper.com/)

* API zur Routenberechnung (u.a.)
* Registrierung erforderlich
* Teilweise Open Source Software

### [Google Directions API](https://developers.google.com/maps/documentation/directions/start)

* API zur Routenberechnung (u.a.)
* Registrierung erforderlich (Google Account)
* Proprietäre Software

### [MapQuest Directions API](https://developer.mapquest.com/documentation/)

* API zur Routenberechnung (u.a.)
* Registrierung erforderlich
* Proprietäre Software (aber auch OSM-Daten nutzbar)

### [GeoTools](http://geotools.org/)

* API zur Geodatenvisualisierung (u.a.)
* Keine Registrierung erforderlich
* Open Source Software

### [Unfolding Maps](http://unfoldingmaps.org/)

* API zur Geodatenvisualisierung (u.a.)
* Keine Registrierung erforderlich
* Open Source Software

### [Mapbox](https://docs.mapbox.com/)

* API zur Geodatenvisualiserung und Routenberechnung (u.a.)
* Registrierung erforderlich
* Proprietäre Software
