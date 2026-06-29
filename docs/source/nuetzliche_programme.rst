Nützliche Programme
===================

In diesem Kapitel stelle ich Ihnen weitere Anwendungen für Linux Mint vor,
die Ihre Produktivität steigern können.


Firefox
-------

Firefox ist einer der besten und sichersten Webbrowser.
Stattdessen können Sie auch Brave, Chromium, Google Chrome, Opera oder Microsoft Edge installieren.
Geben Sie Firefox jedoch eine Chance:
Mit ein paar Einstellungen vereint er Privatsphäre,
Freiheit und Benutzerfreundlichkeit.


Privatsphäre schützen
^^^^^^^^^^^^^^^^^^^^^

Viele möchten sicher einfach nur ungestört surfen.
Firefox ist einer der wenigen Browser, die von Haus aus viele Privatsphäre-Einstellungen mitbringen.

In den Einstellungen können Sie unter ``Datenschutz & Sicherheit`` den verbesserten Schutz vor Aktivitätenverfolgung auf ``Streng`` stellen.
Zusätzlich empfehle ich Ihnen das Add-on **uBlock Origin**,
das unerwünschte Werbung blockiert.

.. tip::
    Sollte eine Webseite einmal nicht so funktionieren,
    wie Sie es sich wünschen,
    können Sie uBlock Origin oben rechts über das rote Schild für diese Seite deaktivieren.
    Den eingebauten Firefox-Schutz können Sie am linken Ende der Adresszeile im Schild für diese Webseite ausstellen.

In den Einstellungen unter ``Suche`` können Sie auch die Standard-Suchmaschine umstellen.
Ich empfehle Ihnen ``DuckDuckGo`` oder ``Ecosia``.
Dadurch bleiben Ihre Suchanfragen weitestgehend anonym.
``Google`` gewinnt tatsächlich noch aktuell das Rennen in Schnelligkeit und Suchergebnissen,
dennoch ist die Privatsphäre bei Google nur bedingt gegeben.

.. tip::
    Sollten Sie die Lesezeichen-Leiste nutzen,
    empfehle ich Ihnen,
    unter ``Weitere Werkzeuge -> Symbolleiste anpassen`` unten links
    ``Symbolleisten -> Lesezeichen-Symbolleiste`` auf ``Nur bei neuem Tab anzeigen`` einzustellen.

.. note::
    Es besteht die Möglichkeit, sich ein Firefox-Konto zu erstellen und Lesezeichen oder Passwörter mit anderen Geräten zu synchronisieren.


KeePassXC
---------

KeePassXC ist ein großartiger, lokaler Passwortmanager.
Im Gegensatz zu Cloud-basierten Lösungen werden Ihre Passwörter in einer verschlüsselten Datei auf Ihrem eigenen Rechner gespeichert.

KeePassXC lässt sich einfach aus der Anwendungsverwaltung installieren.
Um den Komfort zu erhöhen, sollten Sie unbedingt die passende Browser-Erweiterung installieren,
die ein automatisches Ausfüllen von Zugangsdaten ermöglicht.

Zusätzlich bietet KeePassXC mächtige Zusatzfunktionen:

- **TOTP:** Sie können Zwei-Faktor-Authentifizierungscodes (Time-based One-Time Passwords) direkt in KeePassXC generieren lassen, was separate Authenticator-Apps überflüssig macht.
- **SSH-Keys:** Für die Fortgeschrittenen: KeePassXC verfügt über einen integrierten SSH-Agenten. Ihre SSH-Schlüssel können sicher in der Datenbank verwahrt und bei Bedarf automatisch bereitgestellt werden.

.. warning::
    - Verwenden Sie Passwörter niemals doppelt!
    - Da die Datenbank lokal liegt, sind Sie selbst für regelmäßige Backups der `.kdbx`-Datei verantwortlich.
    - Verwenden Sie ein starkes Master-Passwort, da dieses der einzige Schutz für all Ihre Daten ist.


Warpinator
----------

Mit diesem Programm können Sie sehr einfach Dateien im lokalen Netzwerk verschicken.
Das Programm gibt es für Linux und Android.

.. note::
    Haben Sie die Firewall aktiv,
    können Sie in den Einstellungen von Warpinator die Firewall-Regeln aktualisieren:

    .. image:: images/warpinator_firewall.png
    

USB-Stick-Formatierung
----------------------

Auf Linux Mint sind die Programme ``USB-Stick-Formatierer`` und ``USB-Abbilderstellung`` bereits vorinstalliert.

Mit der USB-Abbilderstellung können Sie beispielsweise ``.iso``-Dateien auf einen USB-Stick schreiben.
Damit können Sie dann auf anderen Rechnern beispielsweise Linux installieren.


Laufwerke
---------

Mit diesem Programm können Sie Partitionen auf Ihrer Festplatte verwalten und beispielsweise Einhängeoptionen anpassen.


Pix
---

Mit **Pix** können Sie Fotos von Ihrem Smartphone oder einer SD-Karte importieren und einfache Bearbeitungen vornehmen.
Möchten Sie Bilder detaillierter bearbeiten,
stehen Ihnen Programme wie ``Darktable``, ``GIMP`` oder für Einsteiger ``Pinta`` zur Verfügung.


Systemüberwachung
-----------------

Das Pendant dazu unter Windows ist der Taskmanager.
Über die Systemüberwachung können Sie Prozesse beenden,
sollte sich ein Programm einmal aufhängen.
Im Reiter ``Ressourcen`` finden Sie verschiedene Diagramme,
die den aktuellen Verbrauch von Arbeitsspeicher,
der Internetverbindung und die Auslastung der Prozessorkerne anzeigen.


Festplattenbelegungsanalyse
---------------------------

.. image:: images/festplattenbelegungsanalyse.png

Mit diesem Programm können Sie sehr leicht die Belegung Ihrer Festplatte analysieren.
Klicken Sie auf einen Ringabschnitt,
um in den jeweiligen Ordner zu navigieren.
Um wieder zum übergeordneten Ordner zurückzukehren,
klicken Sie einfach in die Mitte des Diagramms.


Ihre Wissensdatenbank
---------------------

Egal, was Sie an Ihrem Computer oder bei der Arbeit erledigen:
Das Schreiben eigener Anleitungen ist langfristig für die Produktivität essenziell.

Hierfür empfehle ich Ihnen die Nutzung von **Obsidian**.
Dieses Programm ist zwar aktuell nicht Open Source,
verwendet aber sehr offene Formate.
Da Obsidian alle Notizen als einfache `.md`-Dateien (Markdown) in einem normalen Ordner auf der Festplatte speichert,
ist das Format extrem zukunftssicher und flexibel.

.. tip::
    Durch das standardisierte Markdown-Format ist Obsidian hervorragend kompatibel mit **Nextcloud Notes**.
    Wenn Sie Ihren Notizen-Ordner über Nextcloud synchronisieren,
    können Sie Ihre Wissensdatenbank problemlos auf all Ihren Geräten (auch unter Android) nutzen und bearbeiten.


Bildschirmfoto
--------------

Mit diesem Programm können Sie ganz einfach Screenshots erstellen.

1. Mit ``Druck`` können Sie einen Screenshot von der gesamten Bildschirmfläche erstellen.
2. Mit ``Alt`` + ``Druck`` können Sie einen Screenshot vom aktuellen Fenster erstellen.
3. Mit ``Umschalt`` + ``Druck`` können Sie einen eigenen Bildschirmbereich festlegen, der abfotografiert werden soll.

Möchten Sie erweiterte Screenshots erstellen,
empfehle ich Ihnen das Programm **Flameshot** aus der Anwendungsverwaltung.
