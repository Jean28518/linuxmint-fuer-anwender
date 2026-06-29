Der Dateimanager
================

Der vorinstallierte Dateimanager (**Nemo**) ist meiner Ansicht nach einer der besten,
den die Linux-Welt zu bieten hat.
Der Windows-Explorer kann meiner Meinung nach hier nicht mithalten.


Ansichtsoptionen
----------------

.. image:: images/nemo_ansichtsoptionen.png

Ich gehe die Symbole im Folgenden von links nach rechts mit Ihnen durch:

- **Pfadeingabe:** Damit können Sie die Pfadansicht umschalten.
  Dies ist sehr praktisch,
  wenn Sie einen Pfad kopieren möchten.
- **Suche:** Hiermit können Sie Dateien ausgehend vom aktuellen Ordner durchsuchen.
  Sogar nach dem Inhalt von Dateien lässt sich suchen,
  sodass keine Datei verloren geht.
- **Symbolansicht:** Dies ist die normale Ansicht von Ordnern.
  Sie können die Standardansicht in den Einstellungen festlegen.
  Ansonsten wird die gewählte Ansicht nur für den aktuellen Ordner gespeichert.
- **Listenansicht:** Mit der erweiterten Ansicht können Sie nach verschiedenen Kategorien wie beispielsweise dem Änderungsdatum sortieren.
  Mit einem Rechtsklick auf die Kategorienleiste können Sie die gewünschten Parameter festlegen.
- **Kompaktansicht:** Probieren Sie diese Ansicht gerne aus,
  ich persönlich nutze sie im Alltag jedoch kaum.

.. tip::
    Mit der Taste ``F3`` können Sie eine Zwei-Spalten-Ansicht ein- und ausschalten.
    Dies ist sehr hilfreich,
    wenn Sie Dateien kopieren möchten.

.. tip::
    Mit der Tastenkombination ``Strg`` + ``H`` können Sie versteckte Dateien ein- und ausblenden.

Weitere Tabs können Sie mit ``Strg`` + ``T`` öffnen.


Lesezeichen
-----------

Sie können für häufig genutzte Ordner Lesezeichen anlegen.
Ziehen Sie dafür einfach den gewünschten Ordner in die Seitenleiste unter „Lesezeichen“.
Das Lesezeichen ist somit in allen Auswahldialogen,
im Dateimanager und im Startmenü unter „Orte“ aufgelistet.

Ich empfehle Ihnen sehr,
die Lesezeichenliste alphabetisch zu sortieren,
was Sie manuell tun können.


Favoriten
---------

Sie können beliebige Dateien oder Ordner als Favorit markieren.
Favoriten erhalten einen eigenen Eintrag im Dateimanager,
sind mit einem Stern markiert,
haben einen eigenen Eintrag im Startmenü,
sind in der Leiste rechts unten unter dem Sternsymbol aufrufbar
und können in verschiedenen Anwendungen direkt geöffnet werden.


Angeheftete Einträge
--------------------

Um im Dateimanager bestimmte Ordner oder Dateien als erstes anzeigen zu lassen,
können Sie diese mit einem Rechtsklick darauf anheften.

.. tip::
    **Wann sollten Sie welche Funktion nutzen?**
    Ich empfehle Ihnen Folgendes:

    - **Lesezeichen:** Momentan häufig aufgerufene Ordner oder Projekte.
    - **Favoriten:** Dateien, die Sie ständig benötigen, wie beispielsweise Kundendatenbanken, Rechnungsvorlagen oder persönliche Notizzettel.
    - **Angeheftete Einträge:** Einträge innerhalb eines Ordners, die Sie häufig benötigen, wenn Sie diesen Ordner aufrufen (z. B. Ressourcen, Anforderungen, Meetings).


Verknüpfungen
-------------

Um Verknüpfungen zu erstellen,
halten Sie die Tasten ``Strg`` + ``Umschalt`` gedrückt und ziehen Sie den Ordner oder die Datei mit der Maustaste an die gewünschte Stelle.

Alternativ können Sie eine Verknüpfung auch mit der Tastenkombination ``Strg`` + ``M`` erstellen.


Archive erstellen und entpacken
-------------------------------

``.zip``, ``.tar.gz`` oder weitere Archive können Sie im Dateimanager direkt entpacken oder erstellen.
Sie benötigen dafür kein externes Programm.


Archiv erstellen
^^^^^^^^^^^^^^^^

- Klicken Sie mit der rechten Maustaste auf einen Ordner oder eine Datei und wählen Sie ``Komprimieren ...`` aus.
- Hier können Sie den Dateinamen und das Archivformat festlegen.
  ``.tar.gz``-Dateien können in der Regel nur Unix-Systeme lesen,
  mit ``.zip``-Archiven machen Sie hingegen meist nichts falsch.
- Unter den erweiterten Einstellungen können Sie bei manchen Archivformaten beispielsweise ein Passwort festlegen.
- Klicken Sie nun auf ``Anlegen``.
  Je nach Größe des Ordners kann dies einige Minuten dauern.


Archiv entpacken
^^^^^^^^^^^^^^^^

- Klicken Sie mit der rechten Maustaste auf das Archiv.
- Wählen Sie ``Hier entpacken`` aus.

.. note::
    Für komplexere Aufgaben mit Archiven können Sie das Programm ``Archivverwaltung`` verwenden.


Auf entfernte Server zugreifen
------------------------------

Wählen Sie im Startmenü ``Verbinden mit...`` oder im Dateimanager ``Datei -> Mit Server verbinden...``.

Folgende Verbindungstypen sind verfügbar:

- SSH
- FTP
- Windows-Freigabe
- WebDAV
- Sicheres WebDAV

Geben Sie die Serveradresse und die erforderlichen Benutzerdetails an,
um auf den Server zuzugreifen.
Im Ordner-Feld reicht in den allermeisten Fällen ``/`` völlig aus.

Danach sind die Verbindungen in der Seitenleiste des Dateimanagers unter „Netzwerk“ verfügbar.


Ordner freigeben
----------------

.. note::
    Dazu muss das Paket ``Samba`` installiert sein,
    die Anwendung in den Firewall-Regeln freigegeben sein und Ihr Benutzerkonto in der Gruppe ``sambashare`` eingetragen sein (siehe Kapitel *Benutzer und Berechtigungen*).

Klicken Sie mit der rechten Maustaste auf den gewünschten Ordner und wählen Sie ``Freigabeoptionen``.
Die Einstellungen im Konfigurationsdialog sind weitgehend selbsterklärend.
Wenn Sie den ``Gastzugriff`` nicht auswählen,
müssen sich andere Benutzer mit einem auf Ihrem Rechner eingerichteten Benutzerkonto anmelden,
um auf den Ordner zugreifen zu können.

.. note::
    Ich persönlich nutze die klassische Ordnerfreigabe im Alltag nicht,
    sondern setze stattdessen auf Nextcloud.


Dateimanagement
---------------

Im Folgenden gebe ich Ihnen ein paar Tipps,
die langfristig Ihre Produktivität steigern,
während sich Ihr zukünftiges Ich und Ihre Backup-Festplatte darüber freuen werden.

- Ich empfehle Ihnen,
  die vorgegebene Struktur einzuhalten und pro Projekt oder Arbeitsauftrag einen eigenen Ordner anzulegen.
  Es lohnt sich auch,
  einzelne Projekte nach Jahren oder Monaten zu sortieren.
- Wenn Sie Nextcloud nutzen,
  können Sie beispielsweise Ihren Dokumenten-Ordner über eine Verknüpfung direkt in den Nextcloud-Synchronisationsordner verweisen lassen.
- Kennen Sie das Problem,
  dass Sie nicht wissen,
  wo Sie eine Datei auf die Schnelle abspeichern sollen?
  Ich empfehle Ihnen das Anlegen eines zusätzlichen ``Tmp``-Ordners (für temporäre Dateien).
  Dort können Sie Dateien ablegen,
  die Sie nach Ablauf der Woche sicher nicht mehr benötigen.
  Am Ende der Woche können Sie den Inhalt dieses Ordners dann einfach löschen.
- Vermeiden Sie es,
  direkt im Downloads-Ordner zu arbeiten.
  Wenn Sie dies beherzigen,
  können Sie Ihren Downloads-Ordner wöchentlich komplett leeren.
- Versuchen Sie,
  keine Dateien direkt auf dem Desktop (der Arbeitsfläche) abzuspeichern,
  um eine saubere Ordnerstruktur beizubehalten.
- Im persönlichen Ordner selbst sollten sich nur die Hauptverzeichnisse befinden;
  einzelne Dokumente oder Bilder haben dort nichts verloren.