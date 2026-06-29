Büroanwendungen
===============

Empfohlene Büroanwendungen
--------------------------

- Dokumente/Rechnungen/Präsentationen/Tabellen erstellen: **LibreOffice**
- Ausfüllen und (visuelles) Unterschreiben von PDFs: **Xournal++**
- Erstellen einfacher Protokolle, Notizen, Wissensdatenbank: **Obsidian oder xed** mit `Markdown Exporter <https://www.markdowntopdf.com/>`_
- E-Mail-Kommunikation (inklusive Vorlagen): **Thunderbird**
- Finanz-Buchhaltung: **GnuCash** oder **Fakturama**
- Internet-Browser: **Firefox**, **Brave** oder **Chromium**
- Kalender: **Kalender** (gnome-calendar) oder **Nextcloud-Kalender** (im Browser)
- Meetings: **Jitsi**
- Team-Chat: **Element, Matrix**
- Projektmanagement: **OpenProject**
- Synchronisation von Daten, Kalender, Organisation von Teams, ...: **Nextcloud**
- Virtuelle Klebezettel: **Notizen** (sticky)


LibreOffice
-----------

Leider funktioniert Microsoft Office bis heute nicht nativ unter Linux.
Dennoch gibt es mittlerweile zahlreiche Alternativen,
die dieses Problem beheben.
Auch Sie werden Ihren vollwertigen Ersatz finden.

Ich empfehle Ihnen ganz klar LibreOffice.
Es ist bei Linux Mint bereits vorinstalliert.
LibreOffice besitzt eine Vielzahl von Funktionen und deckt jeden erdenklichen Anwendungsfall ab:
Sie können Präsentationen, Formulare, Rechnungen, Vorlagen, Dokumentationen,
funktionale Tabellen, mathematische Formeln, Postkarten,
Briefe und vieles mehr erstellen.

.. tip::
    Sollte Ihnen die Oberfläche nicht gefallen,
    können Sie dies unter ``Ansicht -> Benutzeroberfläche`` anpassen.
    Meine persönliche Empfehlung ist ``In Registern``.
    Diese Oberfläche bietet mehr Funktionen als die Standardoberfläche und erinnert stark an MS Office.
    
    Zusätzlich lässt sich über das Symbol ganz links außen die klassische **Menüleiste parallel aktivieren**.
    Das hilft enorm,
    wenn Sie Online-Anleitungen suchen,
    die oft den klassischen Menüpfad beschreiben.

.. important::
    **Hässliche oder unsichtbare Symbole korrigieren:**
    Falls LibreOffice (z. B. durch eine fehlerhafte Erkennung von dunklen System-Themes) kontrastarme oder unleserliche Symbole anzeigt,
    lässt sich das schnell beheben:
    Unter ``Extras -> Optionen -> Ansicht`` das Symbolthema manuell auf **Colibre** umstellen und anwenden.

Einen Nachteil hat LibreOffice jedoch:
Die Kompatibilität zu Microsoft-Formaten wie .docx, .ppt oder .xls ist standardmäßig nicht perfekt.
Sollten Sie zwingend darauf angewiesen sein,
empfehle ich Ihnen stattdessen entweder das kostenpflichtige `Softmaker Office <https://www.softmaker.de/softmaker-office>`_,
die `Online-Variante von MS Office <https://www.office.com/>`_ oder `OnlyOffice <https://www.onlyoffice.com/de/>`_.

.. tip::
    **Standardmäßig als Microsoft Word (.docx) speichern:**
    Wer viele Dokumente mit MS-Office-Nutzern austauscht,
    kann LibreOffice anweisen,
    standardmäßig im Word-Format zu speichern:
    Unter ``Extras -> Optionen -> Laden/Speichern -> Allgemein`` den Dokumententyp auf *Textdokument* setzen
    und bei *Immer speichern als* den Eintrag **Word 2010–365 (*.docx)** wählen.


Microsoft-Schriftarten installieren
-----------------------------------

Viele Nutzer sind die Microsoft-Schriftarten gewohnt und möchten diese unter Linux weiter nutzen.
Sie können die Schriftarten mit dem Paket ``ttf-mscorefonts-installer`` aus der Anwendungsverwaltung nachinstallieren.

.. note::
    Hier müssen Sie während der Installation die EULA-Lizenz akzeptieren:
    Setzen Sie den Haken im aufploppenden Fenster und klicken Sie auf ``Next``.

    .. image:: images/ttf-mscorefonts-installer-eula.png

Danach müssen Sie alle Office-Anwendungen neu starten,
damit diese die neuen Schriftarten (wie Arial oder Times New Roman) erkennen.


Moderne MS-Schriftarten (Calibri & Cambria) in LibreOffice
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Neuere Windows-Schriftarten wie *Calibri* oder *Cambria* unterliegen anderen Lizenzen und fehlen im obigen Paket.
Linux bietet hierfür jedoch exakte,
metrisch kompatible Open-Source-Alternativen,
die das Layout von Dokumenten nicht zerschießen:

- **Carlito** (freier Ersatz für Calibri)
- **Caladea** (freier Ersatz für Cambria)

Suchen Sie in der *Anwendungsverwaltung* nach den Paketen ``fonts-carlito`` sowie ``fonts-caladea`` und installieren Sie diese.


Automatisches Font-Mapping einrichten
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Damit LibreOffice beim Öffnen von fremden Word-Dateien die fehlenden Originalschriftarten unsichtbar und sauber ersetzt (ohne die Datei beim Zurückspeichern zu verändern),
lässt sich eine Ersetzungstabelle anlegen:

1. Navigieren Sie zu ``Extras -> Optionen -> LibreOffice -> Schriftarten``.
2. Setzen Sie den Haken bei **Ersetzungstabelle anwenden**.
3. Tragen Sie links als Schriftart ``Calibri`` ein und wählen Sie rechts bei *Ersetzen durch* **Carlito** aus.
   Klicken Sie auf das grüne Häkchen.
   Setzen Sie die Haken bei *Immer* und *Bildschirm*.
4. Wiederholen Sie den Vorgang in der Zeile darunter für ``Cambria`` -> **Caladea**.


Standardschrift für neue Dokumente festlegen
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Wenn Sie beim Erstellen eines neuen Dokuments nicht mehr mit der Linux-Schrift *Liberation Serif* starten möchten,
können Sie die Standard-Grundschrift global anpassen:

Wählen Sie unter ``Extras -> Optionen -> LibreOffice Writer -> Grundschriften (Westlich)`` bei den gewünschten Kategorien (Standard, Überschrift, Liste etc.) die Schriftart **Carlito** aus.


Softmaker Office
----------------

Viele Linux-Nutzer sind mit dem kostenpflichtigen `Softmaker Office <https://www.softmaker.de/softmaker-office>`_ sehr zufrieden.
Das proprietäre Programm wird von einem Nürnberger Unternehmen entwickelt und bietet eine sehr hohe Kompatibilität zu den Microsoft-Formaten.

Eine kostenlose Testversion mit eingeschränkter Funktionalität gibt es ebenfalls: `FreeOffice <https://www.freeoffice.com/de>`_


Weitere Alternativen
--------------------

Weitere Alternativen zu MS Office sind unter anderem:

- `Online-Variante von MS Office <https://www.office.com/>`_
- `Google Docs <https://www.google.de/intl/de/docs/about/>`_
- `WPS Office <https://www.wps.com/de-DE>`_


