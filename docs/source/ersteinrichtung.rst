Ersteinrichtung
===============

Bildschirmeinstellungen
-----------------------
Öffnen Sie das Programm ``Bildschirm``.
Wählen Sie hier die richtige Auflösung aus und klicken Sie unten auf ``Anwenden``.

.. tip::
    Sollten Sie die Drei Knöpfe am unteren Rand nicht sehen,
    können Sie mit der ``Alt`` Taste gedrückt das Fenster zusätzlich mit der Maustaste gedrückt nach oben über den Bildschirm hinaus verschieben.

    Diese Funktion kann in den ``Fenster`` Einstellungen unter ``Verhalten`` konfiguriert werden.


Skalierung der Schrift und der Leiste
*************************************


Sollten die Schrift zu klein dargestellt sein, empfehle ich, unter dem Programm ``Schriftauswahl`` den Skalierungsfaktor der Schrift zu ändern.


.. figure:: images/schriftauswahl.png


Die Leiste unten kann man mit Rechtsklick auf die Leiste und dann ``Leisteinstellungen``, dort die Größe des "symbolischen Symbols" (kurioser Übersetzungsfehler) ändern.
Dies muss man sowohl für den linken, (den mittleren), als auch den rechten Teil der Leiste machen.


.. figure:: images/leisteneinstellungen.png



Systemschnappschüsse
--------------------

.. note:: Hiermit werden keine Persönliche Daten gesichert. Dies wird im Kaptitel *Backups* beschrieben.


Systemschnappschüsse sind eine sehr gute Möglichkeit, das System im Falle eines Problems wiederherzustellen, 
dennoch frisst Timeshift unter Linux Mint viel Speicherplatz. 
Ich empfehle, 100 GB Festplattenspeicher dafür einzuplanen.
Hat man diesen Speicher nicht übrig, empfehle ich dieses Kapitel zu überspringen.


Starten Sie das Programm ``Timeshift`` und gehen Sie Schritt für Schritt den Konfigurationsassistent durch:

- Wählen Sie als Schnappschusstyp ``rsync`` aus.
- Wählen Sie als Schnappschussort Ihre Linux Mint-Partition aus.
- Als Schnappschussebene wählen Sie Ihre Konfiguration wie im Bild beschrieben aus:

.. figure:: images/timeshift.png

- Im nächsten Fenster lassen Sie die Konfiguration unverändert. Alle Dateien der Benutzer sollen ausgeschlossen werden.

Nach dem Info-Dialog sind nun die Systemschnappschüsse konfiguriert.
Sie können das Programm nun schließen.

Jeden Monat wird nun ein Systemschnappschuss erstellt.
Die letzten beiden Systemschnappschüsse werden behalten.


Zusätzliche Treiber
-------------------


Öffnen Sie die ``Treiberverwaltung``.

Installieren Sie die hier empfohlenen Treiber.

| Sollte das Fenster anzeigen, dass Ihr Rechner keine zusätzlichen Treiber benötigt:
| Perfekt! Sie haben hier nichts weiter zu tun.


Aktualisierungsverwaltung:
--------------------------

Updates sind sehr sehr wichtig. Durch diese bleibt der Rechner sicher.
Wenn sich die Aktualisierungsverwaltung noch nicht geöffnet hat, dann können Sie diese über das Startmenü öffnen.

.. image:: images/spiegelserver_wechseln.png

Sollte diese Nachricht bei Ihnen erscheinen, ist empfohlen dies durchzuführen. 
Wählen Sie am besten einen Ihnen vertrauten Server aus. Beispielsweise einen von einer nahe gelegenen Universität.
Die Hochschule Esslingen als auch die Friedrich Alexander Universität Erlangen Nürnberg haben sich über die Jahre bewährt.

Nun haben Sie die Wahl: Entweder kümmern Sie sich selber jede Woche um die Updates
oder Sie lassen dies vollautomatisch die Aktualisierungsverwaltung tun.

Es ist sehr empfohlen, dies die automatische Aktualisierungsverwaltung übernehmen zu lassen.

Dazu wählen Sie in der Aktualisierungsverwaltung ``Bearbeiten -> Einstellungen -> Automatisierung`` aus und aktivieren Sie alle vier oder vier Schalter.
Sie werden dabei auch nach Ihrem Passwo2xrt gefragt.

.. note::
    Wenn Sie Ihren Rechner herunterfahren wollen, während der Rechner Aktualisierungen durchführt,
    werden Sie im Herunterfahren-Dialog nicht die gewohnten Knöpfe finden.
    Währenddessen ist das Herunterfahren nämlich nicht erlaubt.
    Nach 5 Minuten sollte in der Regel dann wieder der ``Herunterfahren`` Knopf vorhanden sein.


Systemeinstellungen
-------------------

Hier ist die Steuerzentrale von Linux Mint. Sie bietet eine Übersicht aller möglichen Einstellungen.
Ich empfehle bei den Aktiven Ecken die linke obere Ecke wie folgt einzustellen:

.. figure:: images/aktive-ecken.png

Damit 


Firewall
--------

Sollten Sie einen Laptop haben, mit dem Sie ab und zu unterwegs sind,
ist es empfohlen, die Firewall mit dem Profil ``Öffentlich`` zu aktivieren.

Befinden Sie sich hingegen nur bei Ihnen zuhause,
ist das Aktivieren der Firewall nicht unbedingt nötig, solange Sie Ihren anderen Geräten zuhause vertrauen.
Ihr Internet-Router schützt Sie in der Regel bereits vom Rest des Internets.


Sprache
-------

Öffnen Sie ``Sprachen`` aus dem Menü. Und wählen Sie ``Sprachen hinzufügen/entfernen`` aus.
Installieren Sie hier gegebenenfalls Sprachpakete nach.
