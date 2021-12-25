Netzwerkeinstellungen
=====================

Da das erklären aller Netzwerkeinstellungen alleine schon mehrere Stunden benötigt
und man vieles alsn Anwender nie brauchen wird, beschränken wir uns hier auf relle Anwendungsfälle.


VPN einrichten
--------------

Es gibt viele verschiedene Möglichkeiten, sich zu einem VPN zu verbinden.
Jeder gute VPN-Anbieter sollte eine Anleitung für Linux liefern.
Die Installation von zusätzlichen Paketen ist hierfür häufig erforderlich.
Sollte hier Hilfe benötigt werden, können wir diese gerne im Kurs einrichten.


OpenVPN aus Datei
^^^^^^^^^^^^^^^^^

Gute Anbieter bieten eine .ovpn Datei zum Download an.
Diese kann man dann in den Netzwerkeinstellungen unter ``+ -> Import From File`` einlesen.
In der Regel muss man dann nur noch seine Anmeldedaten des VPN Anbieters eintragen.


DNS-Server umstellen
--------------------

Um eventuell schnellere DNS-Antworten zu bekommen, kann man einen anderen DNS-Server konfigurieren.
Dies kann man in den Einstellungen der jeweiligen Verbindung unter ``IPv4`` und/oder ``IPv6`` erledigen.
Ein möglicher DNS-Server ist beispielsweise `OpenDNS <https://www.opendns.com/>`_.
Unbedingt benötigt wird dieser Schritt aber nicht.