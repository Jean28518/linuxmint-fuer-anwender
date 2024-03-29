Programme installieren
======================


Anwendungsverwaltung
--------------------
Diese sollte die erste Anlaufstelle sein, wenn man Anwendungen installieren möchte. 
Die Beschreibung ist meist aufschlussreich und empfehlenswert.


Beispiel Microsoft Teams:
^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: images/teams-for-linux_anwendungsverwaltung.png

Wenn man sich den Beschreibungstext durchliest, erfahren wir, 
dass diese Ausführung nicht offiziell von Micorosoft unterstützt wird.
Das heißt, Dritte stellen das Programm zur Verfügung.
Sollten also während der Benutzung Fehler auftreten, 
könnte das auf diesen Sachverhalt zurückzuführen sein.

Generell spricht nichts gegen die Verwendung von solchen Ausführungen,
man sollte es aber im Hinterkopf behalten, dass das eine inoffizielle Ausführung ist.
Meistens kriegt man nichtmal mit, dass dies eine inoffizielle Ausführung ist.

Möchte man hingegen die offizielle Version installieren,
werden Details dazu im nächsten Abschnitt ``.deb Dateien aus dem Internet`` beschrieben.


Flatpaks:
^^^^^^^^^
Aus dem Screenshot im zuvorigen Abschnitt kann man unter Details das Wort ``Flatpak`` entnehmen.
Flatpak ist eine neue Technologie, auf Linux Programme zu installieren und auszuführen.

Flatpaks haben den Vorteil, dass sie auf jedem Linux laufen sollen und in der Regel top aktuelle Versionen eines Programms bieten.
Dazu laufen sie in ihrem eigenen kleinen "Linux", auch Sandkasten genannt.
Allerdings können so bei manchen Flatpaks Kompatibilitäts-Probleme im Zusammenspiel vorallem mit anderen Programmen auftreten,
da diese nicht in die kleinen "Sandkästen" herein oder aus ihren eigenen heraus kommen.

Dies bringt eine neue Sicherheitsschicht mit sich: Durch diese kann man kontrollieren, 
was ein Flatpak-Programm auf dem System machen darf.

.. tip:: 
    Manchmal findet man bei der Dateiauswahl nicht die gewünschte Dateien oder Ordner. Dies kann darauf hinweisen, 
    dass das Flatpak keine Berechtigungen hat, auf alle Dateien zuzugreifen.
    Durch die Anwendung ``Flatseal`` kann man unter anderem die Dateiberechtigungen für einzelne Flatpak-Anwendungen einstellen und ändern.

.. warning:: 
    Auch wenn Flatpak-Anwendungen eine neue Sicherheitsschicht haben, kann diese durch bösartige Anwendungen umgangen werden.
    Hat es eine Anwendung also abgesehen, aus dieser Schicht auszubrechen, kann sie dies bis zu einem gewissen Grad tun.


.deb Dateien aus dem Internet
-----------------------------

Manchmal kann es sinnvoll sein, auf die Programme aus der Anwendungsverwaltung zu verzichten und 
die offizielle Version eines Programms zu installieren.

.. warning:: 
    Man sollte unbedingt auf die Quelle der .deb Datei achten. 
    Bitte nur ausschließlich .deb Dateien von offiziellen Herstellerseiten installieren.
    Eine .deb Datei kann ALLES mit dem System machen:
    Das Zerstören des kompletten Systems, Wiederherstellungspunken und aller persönlicher Dateien kann man extrem schnell erreichen.

**Sollte die .deb Version der Herstellerseite keine nennenswerten Vorteile bringen,
wird dringends von der Installation abgeraten, da das Sicherheitsrisiko für das System extrem hoch sein kann.**

Für manche Anwendungen ist aber eine .deb Version unumgänglich, wenn man die Anwendungen nutzen möchte.
Beispielsweise wären das Softmaker Office.

Um eine .deb Datei zu installieren reicht es, diese herunterzuladen
und mit einem Doppelklick zu "starten", und auf ``Paket installieren`` zu drücken.


AppImages
---------

AppImages sind ganz spezielle Dateien: Sie enthalten alles, was eine Anwendung zum Laufen braucht.
Eine Installation ist nicht nötig. Es reicht lediglich, diese in einen Ordner (beispielsweise 'Programme') zu verschieben
und diese in den Datei-Eigenschaften als ausführbar zu markieren. (Siehe Benutzer und Berechtigungen)
Danach kann man das Programm durch einen Doppelklick auf die AppImage Datei starten.

.. tip:: 
    Man kann in den Menüeinstellungen einen neuen Menü-Eintrag für das Programm definieren.
    Dann kann man ein AppImage wie alle übrigen Anwendungen über das Startmenü starten.

.. note:: 
    AppImages werden nicht automatisch aktualisiert. Sicherheitsrelevante Anwendungen nutzen dieses Format aber sowieso nicht.

Fremdquellen (PPAs)
-------------------

Manche Anwendungen findet man nicht in der Anwendungsverwaltung. Anstattdessen "manuell" .deb Dateien zu installieren,
bieten manche Hersteller *Personal Package Archives* (PPAs) an.
Der Vorteil dabei ist, dass Anwendungen daraus auch automatisch Updates erhalten, 
was bei .deb Dateien aus dem Internet normalerweise nicht der Fall ist.

.. note:: 
    Manche .deb Dateien richten automatisch eine Fremdquelle ein und stellen sicher, dass das Programm automatisch Updates erhält.
    Google Chrome macht dies beispielsweise. (Dies muss nicht unbedingt ein PPA sein, wäre aber hier etwas zu weit ausgeholt)

Mit dem Programm ``Anwendungspaketquellen`` kann man PPAs und weitere zusätzliche Fremdquellen einsehen und konfigurieren.

Hat man eine neue Fremdquelle hinzufügt, kann man nach dem Aktualisieren des Zwischenspeichers die Anwendungen in der Anwendungsverwaltung finden.

.. note:: 
    Dafür muss man zusätzlich in der Anwendungsverwaltung im Burger-Menü rechts neben der Suche ``Bitte die Paketliste auffrischen`` auswählen.

.tar.gz oder .zip Dateien
-------------------------

Manchmal bieten Programm-Hersteller nur eine .tar.gz oder .zip Datei an.
Dies geschieht sehr selten und wird einem im regulären Linux-Alltag eigentlich nie begegnen.

Solche Dateien sollte man entpacken. Meist findet man dann dort eine ausführbare Datei (=meist keine Dateiendung), die man dann starten kann.

.. tip:: 
    Man kann in den Menüeinstellungen einen neuen Menüeintrag für das Programm definieren.
    Dann kann man dies wie alle anderen Anwendungen über das Startmenü starten.

.. note:: 
    AppImages werden nicht automatisch aktualisiert. Sicherheitsrelevante Anwendungen nutzen dieses Format aber sowieso nicht.

Sollte man keine ausführbare Datei finden und liegt stattdessen eine Datei mit dem Namen
``Makefile`` vor, muss man dieses Programm erst kompilieren. 
Dies wird allerdings im *Linux Mint für Fortgeschrittene* Kurs behandelt.