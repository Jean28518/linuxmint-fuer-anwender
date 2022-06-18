Der Dateimanager
================

Der vorinstallierte Dateimanager (nemo) ist unserer Ansicht nach einer der besten oder sogar der beste, den die Linux-Welt zu bieten hat.
Der Windows-Explorer kann unserer Meinung nach hier nicht mithalten.

Ansichtsoptionen
----------------
.. image:: images/nemo_ansichtsoptionen.png

Gehen wir die Symbole von links nach rechts durch:

- **Pfadeingabe:** Damit kann man die Pfad-Ansicht umschalten. Dies ist sehr praktisch, wenn man mal einen Pfad kopieren möchte.
- **Suche:** Hiermit kann man entweder Dateien vom aktuellen Ordner aus durchsuchen. Sogar nach dem Inhalt von Dateien kann man suchen. Somit bleibt keien Datei verloren.
- **Symbolansicht:** Die "normale" Ansicht von Ordnern. Man kann die Standard-Ansicht in den Einstellungen definieren. Ansonsten wird die gewählte Ansicht nur für den aktuellen Ordner gespeichert.
- **Listenansicht:** Mit der erweiteren Ansicht kann man nach verschiedenen Kategorien wie bspw. dem Änderungsdatum sortieren. Mit einem Rechtsklick auf die Kategorien-Leiste kann man die Parameter definieren.
- **Kompaktansicht:** Probieren Sie es aus! Aber keine von uns nitzt diese Ansicht im Alltag.

.. tip:: 
    Schon gewusst? Mit der Taste ``F3`` kann man eine Zwei-Listen-Ansicht an- und ausschalten. Dies ist sehr hilfreich, wenn man Dateien kopieren möchte.

.. tip:: 
    Mit der Tastenkombination ``Strg`` + ``H`` kann man versteckte Dateien ein- und ausblenden.

Weitere Tabs kann man mit ``Strg`` + ``T`` erstellen.

Lesezeichen
-----------
Sie können für häufig genutzte Ordner Lesezeichen anlegen. 
Ziehen Sie dafür einfach den gewünschten Ordner an die Seitenleiste unter 'Lesezeichen'.
Das Lesezeichen ist somit unter allen Auswahldialogen, im Dateimanager und im Startmenü unter 'Orte' gelistet.

Es empfiehlt sich sehr, die Lesezeichenliste nach Alphabet zu sortieren. Dies muss manuell bewerkstelligt werden.

Favoriten
---------
Sie können beliebige Dateien oder Ordner als Favorit markieren. 
Favoriten erhalten einen eigenen Eintrag im Dateimanager, sind als Stern markiert,
haben einen eigenen Eintag im Startmenü, sind in der Leiste rechts unten unter dem Sternsymbol aufrufbar
und können in verschiedenen Anwendungen direkt geöffnet werden.

Angeheftete Einträge
--------------------
Um im Dateimanager gewisse Ordner oder Dateien als erstes anzeigen zu lassen können Sie diese mit einem Rechtsklick darauf anheften.


.. tip:: 
    **Was sollte man wofür nutzen?**
    Wir empfehlen:

    - **Lesezeichen:** Momentan oft aufgerufene Ordner/Projekte
    - **Favoriten:** Dateien, die man einfach immer verwendet. Bspw. Kundendatenbanken, Rechnungsvorlagen oder ganz persönliche "Schmierzettel"
    - **Angeheftete Einträge:** Gewisse Einträge in einem Ordner, die man häufig braucht, wenn man diesen Ordner aufruft. Bspw. Ressourcen, Anforderungen, Meetings

Verknüpfungen
-------------
Die Funktion muss in den Einstellungen im Dateimanager aktiviert werden.
Um Verknüpfungen zu erstellen, tätigen Sie Rechtsklick auf eine Datei oder einen Ordner und wählen Sie ``Verknüpfung erstellen`` aus. 
Andernfalls können Sie eine Verknüpfung mit ``Strg`` + ``Shift`` + ``M`` erstellen.


Archive erstellen und Entpacken
-------------------------------
``.zip``, ``.tar.gz`` oder weitere Archive können Sie im Dateimanager direkt entpacken oder erstellen.
Sie benötigen dazu keine externes Programm.

Archiv erstellen
^^^^^^^^^^^^^^^^
- Klicken Sie mit der rechten Maustaste auf einen Ordner oder eine Datei und wählen Sie ``Komprimieren ...`` aus.
- Nun können Sie den Dateinamen und das Archiv-Format definieren. ``.tar.gz`` Dateien können in der Regel nur Unix-Systeme lesen. Mit ``.zip`` Archiven machen Sie meist nichts falsch.
- Unter ``Erweitere Einstellungen`` können Sie bei manchen Archiven-Formaten beispieslweise ein Passwort definieren.
- Klicken Sie nun auf ``Anlegen``. Je nach Größe des Ordners kann dies einige Minuten dauern.

Archiv entpacken
^^^^^^^^^^^^^^^^
- Klicken Sie mit der rechten Maustastem auf ein Archiv.
- Wählen Sie ``Hier entpacken`` aus.

.. note:: 
    Möchten Sie andere Sachen mit Archiven erledigen, können Sie dies über die ``Archivverwaltung`` machen.


Auf entfernte Server zugreifen
------------------------------
Wählen Sie im Startmenü ``Verbinden mit...`` aus, oder wählen Sie im Dateimanager ``Datei -> Mit Server verbinden...`` aus.

Folgende Verbindungstypen sind verfügbar:

- SSH
- FTP
- Windows Freigabe
- WebDAV
- Sicheres WebDAV

Geben Sie jeweils die Serveradresse und häufig Benutzerdetails an, um auf die Server zuzugreifen.
Im Ornder-Feld reicht in den allermeisten Fällen ``/`` vollkommen aus.

Danach sind die Verbindungen in der Seitenleiste des Dateimanagers unter 'Netzwerk' verfügbar.


Ordner freigeben
----------------
.. note:: 
    Dazu muss das Paket ``Samba`` installiert sein und ggf. die Anwendung ``SAMBA`` in den Firewall-Regeln hinzugefügt sein. 
    Außerdem muss der aktuelle Benutzer in der Gruppe ``sambashare`` sein. (Siehe Kapitel *Benutzer und Berechtigungen*)

Klicken Sie mit der rechten Maustaste auf den gewünschten Ordner und wählen Sie ``Freigabeoptionen``. 
Der Konfigurationsdialog sollte selbstverständlich sein.
Wählen Sie ``Gastzugriff`` nicht aus, 
muss sich der Benutzer mit einem auf dem Rechner definierten Benutzerkonto anmelden, um auf den Ordner zuzugreifen können.

.. note::
    Wir nutzen im Alltag die Ordner-Freigabe nicht. Stattdessen setzen wir hier auf Nextcloud.


Dateimanagment
--------------
Hier ein paar Tipps, die langfristig die Produktivität steigern können. Außerdem dankt dies Ihre Backup-Platte und Ihr zukünftiges Ich.

- Versuchen Sie, die vorgegebene Struktur einzuhalten und pro Projekt/Arbeitsauftrag einen eigenen Ordner anzulegen. Es lohnt sich auch, die einzelnen Projekte in Jahre und/oder Monate einzuordnen.
- Nutzen Sie die Nextcloud, können Sie bspw den Dokumenten Ordner über eine Verknüpfung in den Nextcloud-Synchronisations-Ordner zeigen lassen.
- Haben Sie auch manchmal das Problem, dass Sie nicht wissen, wo man schnell mal kurz nur diese Datei abspeichen soll? Wir empfehlen das Anlegen eines zusätzlichen ``Tmp`` (Temporären) Ordners. In Ihm können Dateien gespeichert werden, die man nach Ende der Woche sicher nicht mehr braucht. Am Ende der Woche löscht man dann ganz einfach den Inhalt.
- Arbeiten Sie nicht im Downloads-Ordner. Wenn Sie dies einhalten, können Sie Ihren Downloads-Ordner wöchtenlich komplett leeren.
- Versuchen Sie, nichts auf der Arbeitsfläche selber zu speichern. Dies ist für die Ordner-Struktur sehr hilfreich.
- Im Persönlichen Ordner selber sollten nur wichtige Ordner sein. Dokumente oder Bilder haben hier nichts verloren.