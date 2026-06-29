Installation
============

Download
--------

Sie können Linux Mint von der offiziellen Seite herunterladen: `https://linuxmint.com/download.php <https://linuxmint.com/download.php>`_.
Als Download-Server empfehle ich Ihnen unter anderem die Hochschule Esslingen oder die Friedrich-Alexander-Universität Erlangen-Nürnberg,
da diese seit vielen Jahren sehr zuverlässig funktionieren.
Wenn Sie einen sehr neuen Rechner verwenden,
können Sie auf die „HWE“-Version (Hardware Enablement) zurückgreifen,
die die Entwickler zur Verfügung gestellt haben.
Ich empfehle Ihnen,
diese Version nur dann zu verwenden,
wenn die reguläre Version nicht funktioniert,
da andere auf Linux Mint zugeschnittene Treiber eventuell nicht mit dieser neueren Version kompatibel sind.


Bootstick erstellen
-------------------

Hierfür empfehle ich Ihnen das Programm `Etcher <https://www.balena.io/etcher/>`_.
Ein alternatives Windows-Programm ist `Rufus <https://rufus.ie/>`_.
Wählen Sie dort unter „Auswahl“ die heruntergeladene ISO-Datei aus,
und belassen Sie die restlichen Optionen auf den Standardeinstellungen.
Eventuelle Fragen zu Dateien,
die zusätzlich heruntergeladen werden sollen,
beantworten Sie bitte mit „Ja“.
Wenn Sie bereits eine Linux-Mint-Maschine zur Verfügung haben,
können Sie dies über das vorinstallierte Programm ``USB-Abbilderstellung`` erledigen.


Speicherplatz frei machen
-------------------------

Dies können Sie unter Windows über das Programm ``Festplattenpartitionen erstellen`` erledigen.
Unter Linux Mint können Sie dies über das Programm ``gparted`` oder über ``Laufwerke`` tun.
Ich empfehle Ihnen,
mindestens 50 GB Speicherplatz freizugeben.
Das Erstellen einer Partition auf dem freien Speicherplatz ist dabei nicht nötig.

.. note::
    Wenn Sie Linux Mint neben Windows installieren möchten,
    empfehle ich Ihnen,
    die beiden Systeme auf jeweils eigene Festplatten zu installieren.
    Somit hat Windows weniger Möglichkeiten,
    den Linux-Bootloader zu überschreiben.
    Im Zweifelsfall müssen Sie in diesem Parallelbetrieb den Bootloader von Linux Mint wiederherstellen.
    Ich gehe darauf im Kapitel über die Problembehebung genauer ein.


Installation
------------

Starten Sie den USB-Stick.
Sollten Sie Probleme beim Starten des USB-Sticks haben,
suchen Sie im Internet nach Ihrem Laptop-Modell oder Mainboard-Hersteller
und fügen Sie die Suchbegriffe ``von USB-Stick starten`` hinzu.
Gängige Tasten für das Boot-Menü sind:
``ESC``, ``F2``, ``F8``, ``F11``, ``F12`` oder ``Entf``.

.. note::
    Sollte es Probleme beim Hochfahren von Linux Mint geben,
    können Sie beim Starten des USB-Sticks den ``Compatibility``-Modus auswählen.
    Wenn danach die Bildschirmauflösung noch nicht optimal sein sollte,
    ist das vorerst kein Problem.

Gehen Sie bei der Installation wie gewohnt vor.
Ich empfehle Ihnen dringend,
die Multimedia-Codecs direkt mitzuinstallieren.

Sollten Sie nach einem Passwort für Secure Boot gefragt werden,
empfehle ich Ihnen,
Secure Boot im BIOS/UEFI zu deaktivieren,
da dies später erfahrungsgemäß zu Komplikationen führt,
ohne die Sicherheit merklich zu erhöhen.

Wenn Sie wie oben beschrieben freien Speicherplatz geschaffen haben,
wählen Sie bitte die Option ``Linux Mint daneben installieren``.
Der Rest wird automatisch erledigt.
Ich empfehle diese Vorgehensweise,
da sie am wenigsten Komplikationen verursacht.

Konfigurieren Sie danach in den restlichen Schritten Ihre Linux-Mint-Installation nach Ihren Wünschen.


Verschlüsselung
---------------

Im Fenster für die Installationsart finden Sie unter „Erweiterte Funktionen...“ die Möglichkeit,
das System vollständig zu verschlüsseln.
Diese Option empfehle ich Ihnen vor allem für Laptops,
mit denen Sie häufig unterwegs sind.

.. tip::
    Bei der Benutzererstellung können Sie dann auch die „Automatische Anmeldung“ auswählen,
    da die Systemverschlüsselung bereits einen vollwertigen Passwortschutz bietet.
    Sollten Sie später im installierten System dazu aufgefordert werden,
    ein Passwort für den Anmeldeschlüsselbund anzulegen,
    können Sie das Passwortfeld leer lassen und die Warnung mit „Ignorieren“ bestätigen.
    Denn Ihre Passwörter sind durch die Systemverschlüsselung bereits geschützt abgelegt
    und müssen nicht zwingend doppelt verschlüsselt werden.
    Damit müssen Sie Ihren Laptop nur beim Systemstart entschlüsseln
    und können danach direkt mit der Arbeit loslegen,
    ohne weitere Passwörter eingeben zu müssen.


.. warning::
    Bitte wählen Sie bei der Benutzerkonfiguration die Option ``Meinen Persönlichen Ordner verschlüsseln`` nicht aus:
    Dieser Verschlüsselungsmechanismus gilt als veraltet und unsicher.
    Zudem verhindert diese Methode manche Systemfunktionen,
    wie etwa das korrekte Speichern des Änderungs- oder Erstellungsdatums von Dateien.
    Auch ist die Wiederherstellung dieser Daten im Falle eines Systemabsturzes oder einer Neuinstallation äußerst schwierig
    und kaum dokumentiert.


Manuelle Verschlüsselung von /home im Nachhinein (für Fortgeschrittene)
***********************************************************************

Wenn Sie Ihre persönlichen Daten im Nachhinein verschlüsseln möchten,
können Sie dies wie folgt durchführen:

- Starten Sie den Rechner vom Linux-Mint-Installationsstick.
- Anstatt ``Install Linux Mint`` auszuwählen,
  öffnen Sie ``gparted`` aus dem Anwendungsmenü und wählen Sie oben rechts das richtige Laufwerk aus.
- Sollte nur wenig freier Speicherplatz vorhanden sein,
  sichern Sie Ihre persönlichen Daten vorab beispielsweise auf einer externen Festplatte.
- Verkleinern Sie die vorhandene Linux-Mint-Partition.
  Ich empfehle Ihnen,
  ca. 20 bis 100 GB freien Speicherplatz („Luft“) auf der Systempartition zu lassen,
  damit Sie später problemlos weitere Programme installieren können.
- Wenden Sie die Änderungen in GParted über das grüne Haken-Symbol an.

.. figure:: images/gpartedVerkleinern.png

- Öffnen Sie danach das Programm **Laufwerke** (Disks) und erstellen Sie im neuen freien Speicherplatz über das ``+``-Symbol eine neue Partition.
- Wählen Sie dort als Typ das Linux-Dateisystem und die Passwortverschlüsselung (LUKS) aus.

.. figure:: images/GnomeDisksFestplatteVerschluesselung.png

- Nach dem Anlegen dieser Partition hängen Sie die ursprüngliche Linux-Mint-Systempartition ein (in diesem Beispiel Partition 2).
- Öffnen Sie auf dieser Partition die Datei ``/etc/fstab`` mit Administratorrechten und tragen Sie folgende Zeile ein:

``/dev/mapper/luks-XXXXXX /home ext4 defaults 0 2``

Der LUKS-Code (luks-XXXXXX) muss exakt dem Namen entsprechen,
der in der Laufwerksverwaltung unter der entschlüsselten Partition angezeigt wird:

.. figure:: images/devmapperAdresse.png

- So sollte Ihre Datei am Ende ungefähr aussehen:

.. figure:: images/etc-fstab-dev-mapper.png

- Erstellen Sie nun auf der Systempartition mit Administratorrechten eine neue Datei unter dem Pfad ``/etc/crypttab`` (direkt neben der fstab-Datei) mit folgendem Inhalt:

``luks-XXXXXX UUID=XXXXXXXXXXX none luks``

Dabei ist der LUKS-Teil derselbe wie oben erwähnt.
Der UUID-Teil entspricht der UUID der verschlüsselten Elternpartition,
wie im folgenden Bild dargestellt:

.. figure:: images/LuksUUID.png

Die fertige crypttab-Datei sieht in unserem Beispiel wie folgt aus:

.. figure:: images/crypttab-example.png

- Damit sind Sie fast fertig:
  Nun müssen Sie noch die Daten auf die neue verschlüsselte Partition verschieben.
  Ich empfehle Ihnen dafür das Programm ``grsync``,
  das Sie in der Live-Sitzung des USB-Sticks ganz normal über die Anwendungsverwaltung installieren können.
  Stellen Sie vor dem Start sicher,
  dass beide Partitionen eingehängt sind.
  Klicken Sie dazu in ``Laufwerke`` bei beiden Partitionen auf das dreieckige Wiedergabe-Symbol.

  .. figure:: images/DisksPartitionEinhängen.png

- Konfigurieren Sie grsync anschließend wie folgt:

    - Quelle (Source, erstes Feld): Klicken Sie auf ``Open``, gehen Sie auf ``Other Locations``, wählen Sie die Linux-Mint-Festplatte aus, öffnen Sie den Ordner ``home`` und bestätigen Sie mit ``Open``.
    - **Sehr wichtig:** Fügen Sie am Ende des Pfads im ersten Feld manuell einen Schrägstrich (/) hinzu. Dies ist für grsync zwingend erforderlich, da der Kopiervorgang sonst fehlerhaft verläuft.
    - Ziel (Destination, zweites Feld): Klicken Sie auf ``Open``, gehen Sie auf ``Other Locations``, wählen Sie die verschlüsselte Partition aus und bestätigen Sie mit ``Open``.
    - Wählen Sie alle „Preserve“-Optionen aus, um Dateirechte und Zeitstempel zu erhalten.
    - Starten Sie den Vorgang mit einem Klick auf den grauen Pfeil, um die Daten zu übertragen.

.. figure:: images/grsyncHomeFolder.png

- Fahren Sie nach Abschluss des Kopiervorgangs das Live-System herunter und starten Sie den Rechner normal neu.
  Nun sollten Sie beim Booten zur Eingabe des Entschlüsselungspassworts aufgefordert werden.

- Wenn alles erfolgreich war,
  sieht die Partitionierung in Ihrem installierten Linux Mint unter dem Programm ``Laufwerke`` in etwa so aus:

.. figure:: images/LuksMountedHome.png
