Büroanwendungen
===============

Empfohlene Büroanwendungen
--------------------------

- Dokumente/Rechnungen/Präsentationen/Tabellen erstellen: **Libre Office**
- Ausfüllen und (visuelles) Unterschreiben von PDFs: **Xournal++**
- Erstellen einfacher Protokolle, Notizen, Wissensdatenbank: **Obsidian oder xed** mit `Markdown Exporter <https://www.markdowntopdf.com/>`_
- E-Mail Kommunikatation (inklusive Vorlagen): **Thunderbird**
- Finanz-Buchhaltung: **GnuCash** oder **Fakturama**
- Internet Browser: **Firefox**, **Brave** oder **Chromium**
- Kalender: **Kalender** (gnome-calendar) oder **Nextcloud-Kalender** (im Browser)
- Meetings: **Jitsi**
- Team-Chat: **Element, Matrix**
- Projektmanagement: **OpenProject**
- Synchronisation von Daten, Kalender, Organisation von Teams, ...: **Nextcloud**
- Virtuelle Klebezettel: **Notizen** (sticky)

Libre Office
------------

Leider funktioniert bis jetzt Microsoft Office nicht unter Linux.
Dennoch gibt es mittlerweile zahlreiche Alternativen, die dies beheben.
Auch Sie werden Ihren vollwertigen Ersatz finden.

Wir empfehlen ganz klar Libre Office. Es ist bei Linux Mint bereits vorinstalliert.
Libre Office hat Tonnen von Funktionen und deckt jeden erdenklichen Anwendungsfall ab:
Man kann Präsentationen, Formulare, Rechnungen, Vorlagen, Dokumentationen, funktionale Tabellen, Mathematische Formeln, Postkarten, Briefe und vieles mehr erstellen.

.. tip::
    Sollte Ihnen die Oberfläche nicht gefallen, kann man dies unter ``Ansicht -> Benutzeroberfläche`` einstellen.
    Meine Empfehlung ist ``In Registern``. Diese Oberfläche bietet mehr Funktionen als die Standard-Oberfläche und erinnert stark an MS Office.
    
    Zusätzlich lässt sich über das Symbol ganz links außen die klassische **Menüleiste parallel aktivieren**. Das hilft enorm, wenn man Online-Anleitungen sucht, die oft den klassischen Menüpfad beschreiben.

.. important::
    **Hässliche oder unsichtbare Symbole fixieren:** Falls Libre Office (z. B. durch eine fehlerhafte Erkennung von dunklen System-Themes) kontrastarme oder unleserliche Symbole anzeigt, lässt sich das schnell beheben:
    Unter ``Extras -> Optionen -> Ansicht`` das Symbolthema manuell auf **Colibre** umstellen und anwenden.

Einen Nachteil hat Libre Office jedoch: Die Kompatibilität zu Microsoft-Formaten wie .docx, .ppt oder .xls ist leider standardmäßig nicht so hoch.
Sollte man an diese angewiesen sein, empfehlen wir stattdessen entweder die `Softmaker Office <https://www.softmaker.de/softmaker-office>`, `Online-Variante von MS Office <https://www.office.com/>`_ oder `Only Office <https://www.onlyoffice.com/de/>`_.

.. tip::
    **Standardmäßig als Microsoft Word (.docx) speichern:** Wer viel mit MS-Office-Nutzern austauscht, kann LibreOffice anweisen, standardmäßig im Word-Format zu speichern:
    Unter ``Extras -> Optionen -> Laden/Speichern -> Allgemein`` den Dokumententyp auf *Textdokument* setzen und bei *Immer speichern als* den Eintrag **Word 2010–365 (*.docx)** wählen.

Microsoft Schriftarten installieren
-----------------------------------
Viele Nutzer sind die Microsoft Schriftarten gewohnt und möchten diese unter Linux weiter nutzen.
Man kann die Schriftarten mit dem Paket ``ttf-mscorefonts-installer`` aus der Anwendungsverwaltung nachinstallieren.

.. note::
    Hier muss man während der Installation die EULA-Lizenz akzeptieren:
    Den Haken im aufploppenden Fenster setzen und auf ``Next`` klicken.

    .. image:: images/ttf-mscorefonts-installer-eula.png

Danach müssen alle Office-Anwendungen neu gestartet werden, damit diese die neuen Schriftarten (wie Arial oder Times New Roman) erkennen.

Moderne MS-Schriftarten (Calibri & Cambria) in Libre Office
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Neuere Windows-Schriftarten wie *Calibri* oder *Cambria* unterliegen anderen Lizenzen und fehlen im obigen Paket. Linux bietet hierfür jedoch exakte, metrisch kompatible Open-Source-Alternativen, die das Layout von Dokumenten nicht zerschießen:

- **Carlito** (freier Ersatz für Calibri)
- **Caladea** (freier Ersatz für Cambria)

Suchen Sie in der *Anwendungsverwaltung* nach den Paketen ``fonts-carlito`` sowie ``fonts-caladea`` und installieren Sie diese.

Automatisches Font-Mapping einrichten
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Damit LibreOffice beim Öffnen von fremden Word-Dateien die fehlenden Originalschriftarten unsichtbar und sauber ersetzt (ohne die Datei beim Zurückspeichern zu verändern), lässt sich eine Ersetzungstabelle anlegen:

1. Navigieren Sie zu ``Extras -> Optionen -> LibreOffice -> Schriftarten``.
2. Setzen Sie den Haken bei **Ersetzungstabelle anwenden**.
3. Tragen Sie links als Schriftart ``Calibri`` ein und wählen Sie rechts bei *Ersetzen durch* **Carlito** aus. Klicken Sie auf das grüne Häkchen. Setzen Sie die Haken bei *Immer* und *Bildschirm*.
4. Wiederholen Sie den Vorgang in der Zeile darunter für ``Cambria`` -> **Caladea**.

Standardschrift für neue Dokumente festlegen
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Wer beim Erstellen eines neuen Dokuments nicht mehr mit der Linux-Schrift *Liberation Serif* starten möchte, kann die Standard-Grundschrift global anpassen:

Wählen Sie unter ``Extras -> Optionen -> LibreOffice Writer -> Grundschriften (Westlich)`` bei den gewünschten Kategorien (Standard, Überschrift, Liste etc.) die Schriftart **Carlito** aus.


Softmaker Office
----------------

Viele Linux Nutzer sind mit dem kostenpflichtigen `Softmaker Office <https://www.softmaker.de/softmaker-office>`_ sehr zufrieden.
Das proprietäre Programm wird von einem Nürnberger Unternehmen entwickelt und bietet eine sehr hohe Kompatibilität zu den Microsoft Formaten.

Eine kostenlose Test-Version mit eingeschränkter Funktionalität gibt es auch: `FreeOffice <https://www.freeoffice.com/de>`_

Weitere Alternativen
--------------------

Weitere Alternativen zu MS Office sind unter anderem:

- `Online-Variante von MS Office <https://www.office.com/>`_
- `Google Docs <https://www.google.de/intl/de/docs/about/>`_
- `WPS Office <https://www.wps.com/de-DE>`_


