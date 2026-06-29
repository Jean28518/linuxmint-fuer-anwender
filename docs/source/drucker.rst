Drucker
=======

Häufig erkennt und richtet Linux Mint Ihren Drucker vollkommen automatisch ein.

.. tip::
    Um nachzusehen, ob Ihr eigener Drucker unter Linux unterstützt wird,
    können Sie dies unter `Open Printing <https://www.openprinting.org/printers>`_ nachschlagen.

Wenn Ihr Drucker bereits erkannt und eingerichtet wurde,
können Sie dies in der Regel unten in der Leiste an dem Druckersymbol erkennen.
Steht der Drucker bereits in der Liste,
ist von Ihrer Seite keine Aktion mehr erforderlich.


Drucker hinzufügen
------------------

- Stellen Sie sicher, dass sich der Drucker entweder im gleichen lokalen Netzwerk befindet oder über USB angeschlossen ist.
- Öffnen Sie die Anwendung ``Drucker`` und klicken Sie auf ``Hinzufügen``.
- In dieser Liste sollten Sie Ihren Drucker finden.
  Ist er über das lokale Netzwerk erreichbar,
  öffnen Sie die Netzwerkdrucker-Liste.
  Innerhalb einer Minute müsste der Drucker in der Liste auftauchen.
- Wählen Sie den Drucker in der Liste aus.
  Nach wenigen Sekunden sollten sich verschiedene Möglichkeiten zeigen,
  den Drucker hinzuzufügen.
  Die erste Option ist meist die beste Wahl.
- Im nächsten Schritt werden Sie eventuell gefragt,
  ob ein Duplexer installiert ist.
  Kann Ihr Drucker beidseitig drucken,
  wählen Sie diese Option aus.
- Im nächsten Fenster können Sie einen Namen für den Drucker festlegen.
  Dies ist rein kosmetischer Natur,
  kann aber sehr hilfreich sein.
- Am Ende werden Sie gefragt,
  ob Sie eine Testseite drucken möchten.
  Ich empfehle Ihnen dies,
  wenn Sie den Drucker produktiv nutzen möchten.

.. note::
    Manche Drucker lassen sich leider nicht so einfach installieren.
    Ich kann dies an dieser Stelle leider nur schwer dokumentieren,
    da manche Hersteller ihre ganz eigenen Methoden haben.


Nun ist der Drucker in jedem Druckdialog aufgelistet und auswählbar.
Ein Neustart des Systems ist nicht nötig.

Nun ist der Drucker in jedem Druckdialog aufgelistet und auswählbar.
Ein Neustart des Systems ist nicht nötig.


Sonderfall: Brother-Drucker installieren
----------------------------------------

Sollte Ihr Brother-Drucker nicht automatisch erkannt werden oder Funktionen wie das Scannen nicht direkt klappen, 
stellt Brother ein Installations-Werkzeug für Linux bereit: das **Driver Install Tool**.

Schritt 1: Den richtigen Treiber finden
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Rufen Sie die offizielle Support-Seite von Brother auf (support.brother.com).
2. Suchen Sie nach Ihrem genauen Druckermodell (z. B. *MFC-L2710DW*).
3. Wählen Sie als Betriebssystem-Familie **Linux** und als Version **Linux (deb)** aus (Linux Mint basiert auf Ubuntu/Debian, daher sind `.deb`-Pakete korrekt).
4. Suchen Sie in der Liste nach dem **Driver Install Tool** (oft das oberste Suchergebnis) und laden Sie es herunter. Es handelt sich um eine komprimierte Datei mit der Endung ``.gz`` (z. B. ``linux-brprinter-installer-*.gz``).
5. Entpacken Sie die heruntergeladene Datei direkt im Dateimanager mit einem Rechtsklick.


Schritt 2: Das Installations-Skript starten
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Machen Sie das Skript ausführbar und starten Sie es als Administrator (mittels ``sudo``)::

.. code-block:: bash

    chmod +x linux-brprinter-installer-*

    # Das Brother Install Tool braucht eine andere Sane (Scanner) version:
    sudo add-apt-repository ppa:sane-project/sane-release
    sudo apt update

    # Zusätzliche Treiber Installation starten:
    sudo ./linux-brprinter-installer-*

2. Das Skript fragt Sie nun nach dem genauen Modellnamen. Tippen Sie diesen ein (z. B. ``MFC-L2710DW``) und bestätigen Sie.
3. Bestätigen Sie die darauffolgenden Fragen zur Lizenzvereinbarung und Installation der Pakete jeweils mit **Y** (für Yes/Ja).

Schritt 3: Anschlussart festlegen (Wichtig für Netzwerkdrucker)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wenn alle Treiber heruntergeladen wurden, fragt das Skript nach der Anschlussart:

* **Bei USB:** Antworten Sie bei der Frage ``Will you specify the Device URI?`` mit **N** (Nein).
* **Bei WLAN / LAN (Netzwerk):** Antworten Sie hier mit **Y** (Ja). 

.. tip::
    Wenn Sie ein Netzwerkgerät nutzen, zeigt Ihnen das Skript kurz darauf eine nummerierte Liste mit verschiedenen Verbindungsarten (z. B. *LPD/LPR*, *IPP*). 
    
    Wählen Sie hier den Eintrag, der am Ende **(I)** für "IP-Adresse" stehen hat (oft Option 11 oder 12). Das Skript fragt Sie anschließend direkt nach der IP-Adresse Ihres Druckers (z. B. ``192.168.178.50``). Diese können Sie im Display Ihres Druckers unter den Netzwerkeinstellungen ablesen.

Schritt 5: Abschluss
~~~~~~~~~~~~~~~~~~~~

Am Ende des Prozesses werden Sie gefragt, ob Sie eine Testseite drucken möchten. 
Bestätigen Sie dies, um zu prüfen, ob alles geklappt hat. Das Skript installiert in der Regel auch gleich die passenden Scannertreiber mit, 
sodass Ihr Brother-Gerät nun vollständig einsatzbereit ist.


