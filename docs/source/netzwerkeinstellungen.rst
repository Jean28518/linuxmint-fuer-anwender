Netzwerkeinstellungen
=====================

Da das Erklären aller Netzwerkeinstellungen Tage benötigt
und man vieles als Anwender niemals brauchen wird, beschränken wir uns hier auf reelle Anwendungsfälle.


VPN einrichten
--------------

Es gibt viele verschiedene Möglichkeiten, sich zu einem VPN zu verbinden.
Jeder gute VPN-Anbieter sollte eine Anleitung für Linux liefern.
Die Installation von zusätzlichen Paketen ist hierfür häufig erforderlich.

Große kommerziellen VPN-Anbieter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Große, aggressiv beworbene Anbieter wie CyberGhostVPN, NordVPN und Co. werden von mir bewusst **nicht** empfohlen. 
Das sogenannte Klumpenrisiko ist hier einfach zu groß: Wenn riesige Datenströme über wenige, zentrale Infrastrukturen laufen, 
konterkariert das die Idee von Dezentralisierung und Privatsphäre. 
Viele dieser Marken gehören zudem inzwischen zu denselben Mutterkonzernen. 
Ein eigenes VPN (z. B. auf dem eigenen Router zu Hause) oder kleinere, spezialisierte Anbieter sind aus Sicherheits- und Datenschutzsicht 
fast immer die bessere Wahl.

Ich selber verwende beispielsweise nie ein VPN, um meine Privatsphäre und Sicherheit zu "schützen".
Das macht mein aktueller Webbrowser mit den neuesten TLS-Zertifikaten auch schon ganz alleine, 
ohne dass eine weitere Firma eventuell mithört.
Solange Sie ihrem Internet-Anbieter mehr vertrauen, als teilweise sehr dubiosen VPN-Firmen die bspw. Ihren Sitz in Panama haben, 
empfehle ich Ihnen, das Geld zu sparen und anstattdessen ein Open Source Projekt Ihrer Wahl zu unterstützen.


WireGuard (Empfohlen)
^^^^^^^^^^^^^^^^^^^^^

WireGuard ist die modernste und empfohlene Technologie für VPN-Verbindungen, da sie besonders schnell und effizient ist.
Leider unterstützt Linux Mint Wireguard Konfigurations-Dateien immer noch nicht angemessen grafisch, was mich etwas traurig macht, hoffentlich wird da bald nachgebessert.
Deswegen brechen wir hierfür eine Paradigma dieses Kurses und geben doch ein paar Befehle die im Terminal ausgeführt werden sollen.

.. code-block:: bash
    
    sudo apt install wireguard wireguard-tools
    cd Downloads
    sudo cp meineWiregardDatei.conf /etc/wireguard/wg0.conf
    sudo chmod 600 /etc/wireguard/wg0.conf
    # Mit dem nächsten Befehl wird wireguard für immer automatisch aktiviert:
    sudo systemctl enable --now wg-quick@wg0.service

    # Möchte man die Wireguard Verbindung wieder deaktivieren:
    sudo systemctl disable --now wg-quick@wg0.service


    # Wireguard nur kurzfristig aktivieren:
    sudo systemctl start wg-quick@wg0.service
    # Und wieder deaktivieren:
    sudo systemctl stop wg-quick@wg0.service
   


OpenVPN aus Datei
^^^^^^^^^^^^^^^^^

Gute Anbieter bieten eine .ovpn Datei zum Download an.
Diese kann man dann in den Netzwerkeinstellungen unter ``+ -> Aus einer Datei importieren...`` einlesen.
In der Regel muss man dann nur noch seine Anmeldedaten des VPN Anbieters eintragen.


DNS-Server umstellen
--------------------

Um eventuell schnellere DNS-Antworten zu bekommen, kann man einen anderen DNS-Server konfigurieren.
Dies kann man in den Einstellungen der jeweiligen Verbindung unter ``IPv4`` und/oder ``IPv6`` erledigen.
Ein möglicher DNS-Server ist beispielsweise `OpenDNS <https://www.opendns.com/>`_ oder `Quad9 <https://quad9.net/>`_.
Unbedingt benötigt wird dieser Schritt meist jedoch nicht.