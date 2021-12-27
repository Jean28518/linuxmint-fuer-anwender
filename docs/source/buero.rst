Büroanwendungen
===============

Empfohlene Büroanwendungen
--------------------------

- Dokumente/Rechnungen/Präsentationen/Tabellen erstellen: **Libre Office**
- Ausfüllen und (visuelles) Unterschreiben von PDFs: **Xournal++**
- Erstellen einfacher Protokolle, Notizen: **xed**, `Markdown Exporter <https://www.markdowntopdf.com/>`_ 
- E-Mail Kommunikatation (inklusive Vorlagen): **Thunderbird**
- Finanz-Buchhaltung: **GnuCash**
- Internet Browser: **Firefox**
- Kalender: **Kalender** (gnome-calendar)
- Meetings abhalten: **Jitsi**
- Team-Chat: **Rocket.Chat**
- Synchronisation von Daten, Kalender, Organisation von Teams, ...: **Nextcloud**
- Virtuelle Klebezettel: **Notizen** (sticky)

Alternativen zu Microsoft Office
--------------------------------

Leider funktioniert bis jetzt Microsoft Office nicht unter Linux.
Dennoch gibt es mittlerweile zahlreiche Alternativen, die dies beheben.
Auch Sie werden Ihren vollwertigen Ersatz finden.

Libre Office
^^^^^^^^^^^^
Wir empfehlen ganz klar Libre Office. Es ist bei Linux Mint bereits vorinstalliert.
Libre Office hat Tonnen von Funktionen und deckt jeden erdenklichen Anwendungsfall ab:
Man kann Präsentationen, Formulare, Rechnungen, Vorlagen, Dokumentationen, funktionale Tabellen, Mathematische Formeln, Postkarten, Briefe und vieles mehr erstellen.

Sollte Ihnen die Oberfläche nicht gefallen, kann man dies unter ``Ansicht -> Benutzerobferfläche`` einstellen.
Unsere Empfehlung ist ``In Registern``. Diese Oberfläche bietet mehr Funktionen als die Standard-Oberfläche und erinnert stark an MS Office.

Einen Nachteil hat Libre Office jedoch: Die Kompatibilität zu Microsoft-Formaten wie .docx, .ppt oder .xls ist leider nicht so hoch.
Sollte man an diese angewiesen sein, empfehlen wir stattdessen entweder die  `Online-Variante von MS Office <https://www.office.com/>`_, 
`Softmaker Office <https://www.softmaker.de/softmaker-office>`_ oder `WPS Office <https://www.wps.com/de-DE>`_.

Softmaker Office 
^^^^^^^^^^^^^^^^
Viele Linux Nutzer sind mit dem kostenpflichtigen `Softmaker Office <https://www.softmaker.de/softmaker-office>`_ sehr zufrieden. 
Das proprietäre Programm wird von einem Nürnberger Unternehmen entwickelt und bietet eine sehr hohe Kompatibilität zu den Microsoft Formaten.

Eine kostenlose Test-Version mit eingeschränkter, älterer Funktionalität gibt es auch: `FreeOffice <https://www.freeoffice.com/de>`_ 

Weitere Alternativen
^^^^^^^^^^^^^^^^^^^^
Weitere Alternativen zu MS Office sind unter anderem:

- `Online-Variante von MS Office <https://www.office.com/>`_
- `Google Docs <https://www.google.de/intl/de/docs/about/>`_ 
- `WPS Office <https://www.wps.com/de-DE>`_
- `Only Office <https://www.onlyoffice.com/>`_ 


Microsoft Schriftarten installieren
-----------------------------------
Viele Nutzer sind die Microsoft Schriftarten gewohnt und möchten diese unter Linux weiter nutzen.
Man kann die Schriftarten mit dem Paket ``ttf-mscorefonts-installer`` aus der Anwendungsverwaltung nachinstallieren.

.. note:: 
    Hier muss man während der Installation die EULA-Lizenz akzeptieren: 
    Den Haken im aufploppenden Fenster setzen und auf ``Next`` klicken.

    .. image:: images/ttf-mscorefonts-installer-eula.png

Danach müssen alle Office-Anwendungen neu gestartet werden, damit diese die neuen Schriftarten erkennen.
    