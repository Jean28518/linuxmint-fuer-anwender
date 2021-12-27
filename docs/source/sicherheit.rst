Linux Mint sicher nutzen
========================

Updates
-------
Ein Großteil aller Hackerangriffe setzt auf Sicherheitslücken,
die in alten Programm-Versionen enthalten sind.
Deswegen sind Aktualisierungen sehr wichtig.

Lesen Sie dafür den Abschnitt *Aktualisierungsverwaltung* im Kapitel *Ersteinrichtung*.

Wine deinstallieren
-------------------
Wine ist eine Laufzeitumgebung für Windows Programme.
Windows Viren können so also doch auf Linux funktionieren, wenn wine installiert sein sollte.
Sollten Sie also nicht aktiv ein Windows Programm auf Linux nutzen,
Deinstallieren Sie Wine.

Generell raten wir von der Benutzung von Windows-Programmen auf Linux aufgrund möglicher eingeschränkter Benutzererfahrung ab.

Wine ist standardmäßig nicht installiert.

Webbrowser sicher einrichten
----------------------------
Lesen Sie dafür den Abschnitt Firefox im Kaptiel *Nützliche Programme*.
Mit anderen Browsern funktioniert die Anleitung genau so.

Virenschutz
-----------
Unter Linux benötigen Sie keinen zusätzlichen Virenschutz. 
Viele Experten empfehlen sogar unter Windows keinen zusätzlichen Virenschutz. (`https://youtu.be/NDlYeJSyqeU <https://youtu.be/NDlYeJSyqeU>`_ )

Ein Virenprogramm bietet keinen zusätzlichen Schutz:

- Wenn Ihr Linux Mint aktuell ist,
- Sie nur so viele Anwendungen wie nötig auf Ihren Linux installiert haben,
- Sie nicht wahllos externe Anwendungen (außerhalb der Annwenndungsverwaltung) installieren
- und Sie keine unbekannten Anhänge aus E-Mails öffnen.

Auch wenn Sie einen Fehler machen, versagen in der Paxis leider noch häufig genug Virenschutzprogramme.
Möchten Sie den Kopf beim Nutzen Ihres Computers ausschalten, schalten Sie am besten Ihren Computer gleich mit aus.

.. note:: 
    Nutzen Sie einfach ``brain.sh`` (ihren Verstand, das beste Antivirenschutzprogramm auf dem Markt)
    und befolgen Sie die Tipps in diesem Kapitel und in den 10 Goldenen Sicherheitsregeln, die Sie im Kurs bekommen haben.
    Ihre Sicherheit auf Linux ist daraufhin extrem hoch.

Passwortmanager
---------------
Nutzen Sie Passwortmanager!
Wichtig ist, dass Sie für jede Anmeldung ein komplett neues, **sicheres** Passwort verwenden.
Dabei ist es egal, ob Sie sich alle Passwörter für jede Anmeldung merken, Sie diese auf Zettel schreiben
oder einen Passwortmanager wie das freie Open Source Programm ``Bitwarden`` verwenden. Eine Alternative ist beispielsweise ``KeePassXC``.

.. note:: 
    Unter einem sicheren Passwort verstehen wir folgende Kriterien:

    - Länge über 20 Zeichen
    - Sonderzeichen enthalten
    - Zahlen enthalten
    - Groß- und Kleinbuchstaben enthalten
    - Enthält keine auf Sie zurückführbare Informationen

    Zum Generieren sicherer Passwörter empfehlen wir den ersten Teil dieses `Videos <https://youtu.be/MNQxg7uyE3I?t=71>`_ .

Backups
-------
Machen Sie regelmäßig Backups von Ihren Dateien.
Dies ist Ihre Lebensversicherung.
Weitere Informationen finden Sie im Kapitel **Backups**.

Fremquellen
-----------
Achten Sie darauf, welche Anwendungspaketquellen (PPAs, weitere Fremquellen) auf Ihrem System aktiviert sind.
Solche Quellen können auch böswillig ausgenutzt werden.

Eine Übersicht erhalten Sie im Programm ``Anwendungspaketquellen``.

10 Goldene Sicherheitsregeln
----------------------------
Im Kurs erhalten Sie kompakt 10 Goldene Sicherheitsregeln, die Sie sich praktisch ausdrucken können.