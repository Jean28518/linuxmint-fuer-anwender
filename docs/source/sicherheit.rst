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
Lesen Sie dafür den Abschnitt Firefox im Kapitel *Nützliche Programme*.
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
    und befolgen Sie die Tipps in diesem Kapitel und in den 5 Goldenen Sicherheitsregeln am Ende dieses Kapitels.
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

Fremdquellen
------------
Achten Sie darauf, welche Anwendungspaketquellen (PPAs, weitere Fremquellen) auf Ihrem System aktiviert sind.
Solche Quellen können auch böswillig ausgenutzt werden.

Eine Übersicht erhalten Sie im Programm ``Anwendungspaketquellen``.

5 Goldene Sicherheitsregeln
---------------------------

Zusammenfassend lässt sich die Sicherheit Ihres Systems auf fünf goldene Regeln reduzieren. Wenn Sie diese beherzigen, ist Ihr Linux-System extrem sicher:

.. image:: images/5GoldeneSicherheitsregeln.jpg
   :alt: 5 Goldene Sicherheitsregeln
   :align: center

|


1. **Aktualisierungen (Updates):**
   Sobald solche Sicherheitslücken bekannt werden, schließen Entwickler sie über Sicherheitsupdates.
   Angreifer suchen gezielt nach Systemen mit veralteter Software, um diese Schwachstellen auszunutzen. 
   Halten Sie Ihr System und Ihre Programme daher immer aktuell. 
   Die Aktualisierungsverwaltung von Linux Mint macht Ihnen das sehr einfach – richten Sie dort am besten automatische Updates für Systempakete und Flatpaks ein (wie im Kapitel *Ersteinrichtung* beschrieben).

2. **Vermeidung unnötiger Software:**
   Wenn ein Programm eine Sicherheitslücke aufweist, kann dies das gesamte System gefährden – selbst wenn Sie die Anwendung nur selten nutzen. 
   Installieren Sie daher nur Software, die Sie wirklich brauchen, und entfernen Sie nicht mehr benötigte Programme. 
   Weniger installierte Software bedeutet schlichtweg weniger potenzielle Einfallstore für Schadcode.

3. **Sichere, einzigartige Passwörter:**
   Wird ein einziger Online-Dienst gehackt, haben Angreifer sofort Zugriff auf all Ihre Konten bei anderen Plattformen. 
   Verwenden Sie für jeden Zugang ein eigenes, langes und zufälliges Passwort. 
   Da man sich diese unmöglich alle merken kann, ist der Einsatz eines Passwortmanagers wie **Bitwarden** oder **KeePassXC** dringend zu empfehlen. 
   Sie müssen sich dann nur noch ein einziges Master-Passwort merken.

4. **Nicht täuschen lassen (Phishing & Social Engineering):**
   Da Desktop-Systeme selber mittlerweile nahezu unerreichbar sind, versuchen Kriminelle meist den Menschen vor dem Bildschirm auszutricksen. 
   Sie versenden täuschend echte E-Mails von Banken oder Paketdiensten und verlinken auf gefälschte Login-Seiten, um Zugangsdaten abzugreifen. 
   Seien Sie stets misstrauisch: Klicken Sie nicht voreilig auf Links, 
   prüfen Sie die Absenderadresse und achten Sie im Browser auf Tippfehler in der Adresszeile (z. B. ``paypal-sicherheit.de`` statt ``paypal.com``). 
   Im Zweifel rufen Sie die Seite manuell über eine Suchmaschine auf.

5. **Regelmäßige Backups:**
   **Es gibt keine hundertprozentige Sicherheit.** Hardware kann kaputtgehen, 
   Dateien können versehentlich gelöscht werden oder das System nimmt bei einem Fehler Schaden.
   Ein Backup ist Ihre absolute Lebensversicherung. 
   Sichern Sie Ihre persönlichen Daten (Dokumente, Fotos) regelmäßig auf eine externe Festplatte oder einen Netzwerkspeicher. 
   Linux Mint bietet dafür mit **Pika Backup** (für Dateien) und **Timeshift** (für das System) hervorragende Werkzeuge. 
   Details dazu finden Sie im Kapitel **Backups**.
