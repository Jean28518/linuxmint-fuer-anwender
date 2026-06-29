Netzwerkeinstellungen
=====================

Da das Erklären aller Netzwerkeinstellungen Tage in Anspruch nehmen würde
und Sie vieles davon als Anwender niemals benötigen werden,
beschränke ich mich in diesem Kapitel auf die praxisnahen Anwendungsfälle.


VPN einrichten
--------------

Es gibt viele verschiedene Möglichkeiten,
eine VPN-Verbindung herzustellen.
Jeder gute VPN-Anbieter sollte eine Anleitung für Linux bereitstellen.
Die Installation zusätzlicher Pakete ist hierfür häufig erforderlich.


Große kommerzielle VPN-Anbieter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Große, aggressiv beworbene Anbieter wie CyberGhostVPN, NordVPN und Co. empfehle ich Ihnen bewusst **nicht**.
Das sogenannte Klumpenrisiko ist hier einfach zu groß:
Wenn riesige Datenströme über wenige, zentrale Infrastrukturen laufen,
konterkariert das die Idee von Dezentralisierung und Privatsphäre.
Viele dieser Marken gehören zudem inzwischen zu denselben Mutterkonzernen.
Ein eigenes VPN (z. B. auf dem eigenen Router zu Hause) oder kleinere, spezialisierte Anbieter sind aus Sicherheits- und Datenschutzsicht
fast immer die bessere Wahl.

Ich selbst verwende beispielsweise nie ein VPN,
um meine Privatsphäre und Sicherheit zu „schützen“.
Das macht mein aktueller Webbrowser mit den neuesten TLS-Zertifikaten auch schon ganz allein,
ohne dass eine weitere Firma eventuell mithört.
Solange Sie Ihrem Internetanbieter mehr vertrauen als teilweise sehr dubiosen VPN-Firmen,
die beispielsweise ihren Sitz in Panama haben,
empfehle ich Ihnen,
das Geld zu sparen und stattdessen ein Open-Source-Projekt Ihrer Wahl zu unterstützen.


WireGuard (empfohlen)
^^^^^^^^^^^^^^^^^^^^^

WireGuard ist die modernste Technologie für VPN-Verbindungen und meine persönliche Empfehlung,
da sie besonders schnell und effizient arbeitet.
Leider unterstützt Linux Mint die grafische Einrichtung von WireGuard-Konfigurationsdateien immer noch nicht optimal,
was ich sehr schade finde.
Hoffentlich wird hier bald nachgebessert.
Deswegen breche ich an dieser Stelle mit einem Prinzip dieses Handbuchs
und zeige Ihnen doch ein paar Befehle,
die Sie im Terminal ausführen können:

.. code-block:: bash
    
    sudo apt install wireguard wireguard-tools
    cd Downloads
    sudo cp meineWiregardDatei.conf /etc/wireguard/wg0.conf
    sudo chmod 600 /etc/wireguard/wg0.conf
    # Mit dem nächsten Befehl wird wireguard für immer automatisch aktiviert:
    sudo systemctl enable --now wg-quick@wg0.service

    # Wenn Sie die WireGuard-Verbindung wieder deaktivieren möchten:
    sudo systemctl disable --now wg-quick@wg0.service


    # Wireguard nur kurzfristig aktivieren:
    sudo systemctl start wg-quick@wg0.service
    # Und wieder deaktivieren:
    sudo systemctl stop wg-quick@wg0.service
   


OpenVPN aus Datei
^^^^^^^^^^^^^^^^^

Gute Anbieter bieten eine ``.ovpn``-Datei zum Download an.
Diese können Sie dann in den Netzwerkeinstellungen über das ``+``-Symbol unter ``Aus einer Datei importieren...`` einlesen.
In der Regel müssen Sie dort nur noch die Anmeldedaten Ihres VPN-Anbieters eintragen.


DNS-Server umstellen
--------------------

Um eventuell schnellere DNS-Antworten zu erhalten,
können Sie einen anderen DNS-Server konfigurieren.
Dies können Sie in den Einstellungen der jeweiligen Verbindung unter ``IPv4`` und/oder ``IPv6`` vornehmen.
Ein empfehlenswerter DNS-Server ist beispielsweise `OpenDNS <https://www.opendns.com/>`_ oder `Quad9 <https://quad9.net/>`_.
Unbedingt benötigt wird dieser Schritt meist jedoch nicht.