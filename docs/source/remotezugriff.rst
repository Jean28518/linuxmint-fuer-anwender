Remotezugriff
=============

Es gibt verschiedene Möglichkeiten,
auf einen Rechner über das Netzwerk zuzugreifen.

Die einfachste und gängigste Methode unter Linux ist die *Secure Shell* (SSH).
Diese baut lediglich eine reine Terminal-Verbindung auf.
Für Server-Administratoren ist dies hervorragend,
für Sie als Desktop-Anwender im Alltag jedoch meist wenig hilfreich.

Neben SSH gibt es noch weitere Methoden,
sich mit einem Rechner zu verbinden.
Eines der am weitesten verbreiteten Protokolle ist das *Remote Desktop Protocol* (RDP).
Dadurch können Sie über ein entsprechendes Programm direkt auf den Desktop des entfernten Rechners zugreifen.


Entfernter Rechner
^^^^^^^^^^^^^^^^^^

Um auf Ihren Rechner aus der Ferne zuzugreifen,
müssen Sie auf diesem das Paket ``Xrdp`` aus der Anwendungsverwaltung installieren.
Zudem benötigen Sie die IP-Adresse des Rechners,
um die Verbindung später herstellen zu können.
Diese können Sie ganz einfach in den Netzwerkeinstellungen über das Zahnrad-Symbol ablesen
(die IPv4-Adresse ist dabei zu bevorzugen).

.. note::
    Wenn Ihre Firewall aktiv ist,
    müssen Sie in den Firewall-Einstellungen die Anwendung ``RDP`` erlauben.


Rechner vor Ort
^^^^^^^^^^^^^^^

Auf dem steuernden Rechner müssen Sie lediglich das Programm **Remmina** aus der Anwendungsverwaltung installieren.
Ich verwende in diesem Beispiel die Flatpak-Variante.

In Remmina fügen Sie eine neue Verbindung oben links über das ``+``-Symbol hinzu.
Wählen Sie als Protokoll ``RDP - Remote Desktop Protokoll``.
Unter ``Server`` tragen Sie die IP-Adresse des entfernten Rechners ein.
Als Benutzernamen und Passwort tragen Sie die Anmeldedaten des entfernten Rechners ein.
Bei der Auflösung empfehle ich Ihnen die Einstellung ``Auflösung des Client verwenden``.
Am Ende können Sie auf ``Speichern und verbinden`` klicken.

Ein korrektes Einstellungsfenster sieht wie folgt aus:

.. image:: images/remmina_verbindungsprofil.png


.. note::
    Ein Benutzer kann grafisch nur einmal angemeldet sein.
    Es ist nicht möglich, dass derselbe Benutzer lokal und gleichzeitig aus der Ferne angemeldet ist.
    
    Auf dem entfernten Rechner sehen Sie auch nichts auf dem Bildschirm,
    wenn jemand aus der Ferne angemeldet ist.

    Die Rechner müssen sich im selben lokalen Netzwerk befinden.

.. tip::
    Wenn Sie zusätzlich eine VPN-Verbindung einrichten,
    können Sie auf diese Weise problemlos auch auf Rechner in hunderten Kilometern Entfernung zugreifen.


RustDesk
--------

Eine sehr beliebte Open-Source-Alternative zu bekannten kommerziellen Fernwartungsprogrammen wie TeamViewer oder AnyDesk ist **RustDesk**.
Im Gegensatz zu RDP benötigt RustDesk im Standardbetrieb keine aufwendige VPN-Einrichtung oder Portfreigaben im Router,
da die Verbindung über öffentliche Vermittlungsserver (Relay-Server) hergestellt wird.

**Vorteile von RustDesk:**
Die Bedienung ist denkbar einfach:
Die Verbindung wird unkompliziert per ID und Einmalpasswort aufgebaut (ähnlich wie bei TeamViewer),
ganz ohne VPN-Einrichtung.
RustDesk läuft auf allen gängigen Systemen (Linux, Windows, macOS, Android, iOS),
verschlüsselt standardmäßig Ende-zu-Ende und erlaubt es Ihnen sogar,
einen eigenen Server aufzusetzen,
um die volle Kontrolle über Ihre Daten zu behalten.

**Nachteile von RustDesk:**
Wer die kostenlosen, öffentlichen Server von RustDesk nutzt,
muss sich seit einiger Zeit auf dem steuernden Gerät zwingend mit einem Account (z. B. Google, GitHub oder E-Mail) anmelden,
um Missbrauch zu verhindern.
Zudem teilen Sie sich die Bandbreite mit der restlichen Community,
was zu Stoßzeiten zu spürbaren Rucklern oder langsamen Verbindungen führen kann.

.. note::
   Wenn Sie die Registrierungspflicht umgehen und maximale Privatsphäre genießen möchten,
   können Sie sich relativ einfach einen eigenen RustDesk-Server (bestehend aus den Diensten ``hbbs`` und ``hbbr``) auf einem eigenen Minicomputer (z. B. Raspberry Pi) oder einem virtuellen Server im Internet einrichten.