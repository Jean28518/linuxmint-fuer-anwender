PDF-Dateien und Scannen
=======================

PDF-Dokumente (Portable Document Format) sind aus dem modernen Büroalltag nicht mehr wegzudenken. 
Doch sobald es an das Bearbeiten, Ausfüllen, Unterschreiben oder Scannen geht, stehen viele Anwender vor Hürden. 

Wichtiger Grundsatz zur PDF-Bearbeitung
---------------------------------------

Bevor Sie mit der Bearbeitung beginnen, ist ein technischer Aspekt entscheidend: 
**PDF-Dateien sind von ihrer Struktur her nicht für die nachträgliche Bearbeitung gedacht.** 
Sie sind fertige Endprodukte (vergleichbar mit einem gedruckten Blatt Papier). 

Wann immer es möglich ist, sollten Sie daher versuchen, das **Originaldokument** 
(z. B. eine ``.docx``-Datei in Word/Writer oder eine ``.odt``-Datei in LibreOffice) zu ändern und anschließend neu als PDF zu exportieren. 
Wenn das Original nicht vorliegt, bieten die folgenden Werkzeuge unter Linux Mint praktische Auswege.

Seiten verwalten (Trennen, Zusammenfügen, Drehen)
-------------------------------------------------

Häufig müssen Seiten aus verschiedenen Dokumenten zusammengefügt, einzelne Seiten gelöscht oder gedrehte Seiten korrigiert werden.

* **PDF Arranger:** 
  Dieses schlanke Open-Source-Werkzeug ist die absolute Empfehlung für diese Aufgaben. Sie können PDFs einfach per Drag-and-Drop in das Fenster ziehen, 
  Seiten mit der Maus verschieben (umordnen), drehen, weiße Ränder beschneiden oder Dokumente zusammenfügen (Mergen). 
  Nach getaner Arbeit exportieren Sie das Ergebnis wieder als neue PDF-Datei. 
  Das Programm ist extrem schnell, unkompliziert und lässt sich direkt über die Anwendungsverwaltung von Linux Mint installieren.

* **LibreOffice Draw:** 
  Auch die Zeichenanwendung von LibreOffice kann PDFs importieren. 
  Sie können in der Seitenleiste Seiten per Drag-and-Drop verschieben, kopieren oder löschen.


Inhalte und Text verändern
--------------------------

Möchten Sie Tippfehler direkt im PDF korrigieren oder Grafiken austauschen, gibt es dafür verschiedene Ansätze:

* **LibreOffice Draw (kostenlos & Open Source):**
  Wenn Sie eine PDF-Datei mit LibreOffice Draw öffnen, wird der Text in editierbare Boxen umgewandelt. 
  Das funktioniert für kleine Korrekturen gut. 
  Der Nachteil: Draw zerlegt zusammenhängende Absätze oft in einzelne Zeilen, was das Formatieren von Fließtext erschwert.


* **Master PDF Editor (proprietär, eingeschränkt kostenlos):**
  Dieses spezialisierte Programm bietet eine deutlich komfortablere Textbearbeitung. 
  In der kostenlosen Grundversion können Sie Texte editieren, Grafiken verschieben, skalieren oder austauschen. 
  
  .. note::
     Achten Sie darauf, dass manche erweiterte Funktionen in der kostenlosen Version ein Wasserzeichen auf dem gespeicherten Dokument hinterlassen. Für reine Textänderungen in bestehenden Textfeldern ist es dennoch eines der besten Werkzeuge unter Linux.


* **Adobe Online-Konverter (Web-basiert):**

  Wenn Sie eine PDF-Datei zwingend in ein echtes Word-Dokument (``.docx``) zurückverwandeln müssen, stoßen lokale Offline-Tools unter Linux oft an ihre Grenzen. 
  In solchen Fällen wird der kostenlose `Online-Konverter von Adobe <https://www.adobe.com/de/acrobat/online/pdf-to-word.html>`_ empfohlen, 
  um die bestmögliche Layout-Konvertierung zu erzielen.


PDFs ausfüllen, kommentieren und unterschreiben
-----------------------------------------------

Nicht jedes Formular ist digital interaktiv. Oft müssen Sie ein "klassisches" PDF-Dokument am PC ausfüllen oder digital unterschreiben.

* **Xournal++:**
  Das perfekte Werkzeug für handschriftliche Notizen, Skizzen und das Einfügen einer **digitalen Unterschrift**. 
  Sie können mit einer Maus oder einem Grafiktablett direkt auf dem Dokument unterschreiben. 
  Zudem lässt sich über die Textwerkzeuge ein Textfeld flexibel über jede beliebige Stelle des Dokuments legen, 
  um herkömmliche Formulare sauber am PC auszufüllen.

* **Okular:**
  Mit Okular können Sie Textstellen farblich markieren, Notizen oder Haftnotizen hinzufügen, 
  geometrische Formen einzeichnen und diese Anmerkungen direkt im PDF speichern.


Interaktive PDF-Formulare
-------------------------

Echte interaktive PDFs enthalten ausfüllbare Formularfelder, Kontrollkästchen oder Auswahllisten.

* **Formulare erstellen:**
  Sie können interaktive PDF-Formulare selbst mit **LibreOffice Draw** erstellen. 
  Aktivieren Sie unter ``Ansicht -> Symbolleisten -> Formular-Steuerelemente``. 
  Hier können Sie Textfelder, Optionsfelder (Radio Buttons), Kontrollkästchen und Listenfelder zeichnen. 
  Über einen Rechtsklick auf das jeweilige Feld gelangen Sie in die *Eigenschaften*, um Schriftarten, Zeichenbegrenzungen und Namen anzupassen. 
  Exportieren Sie das Dokument anschließend über ``Datei -> Exportieren als -> Als PDF exportieren`` und stellen Sie sicher, 
  dass der Haken bei *PDF-Formular erzeugen* gesetzt ist.

* **Formulare ausfüllen:**
  Manche komplexen PDF-Formulare (z. B. von Behörden) enthalten integrierte Berechnungen oder spezielle Formatierungen. 
  Standard-Dokumentenbetrachter scheitern hierbei oft. 
  Als stabiler und zuverlässiger PDF-Formular-Ausfüller wird der **Chromium Webbrowser** (oder Google Chrome) empfohlen. 
  Öffnen Sie die PDF-Datei einfach im Browser, füllen Sie sie aus und speichern Sie das ausgefüllte PDF-Dokument.

Scannen mit NAPS2 und OCR-Texterkennung
---------------------------------------

Ein wichtiger Schritt beim papierlosen Büro ist das Scannen von Dokumenten. 
Linux Mint bringt zwar ein Standard-Scanprogramm mit, für produktives Arbeiten empfiehlt sich jedoch **NAPS2** (Not Another PDF Scanner 2).

NAPS2 zeichnet sich durch eine extrem einfache, aufgeräumte Benutzeroberfläche aus und unterstützt sowohl Flachbettscanner 
als auch automatische Dokumenteneinzüge (ADF). Sie können gescannte Seiten schnell verschieben, drehen, zuschneiden und direkt als PDF speichern.

Installation von NAPS2 unter Linux Mint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Obwohl es NAPS2 als Flatpak gibt, kann diese Version manchmal Probleme mit den lokalen Scannertreibern (SANE) haben. 
Es wird daher empfohlen, das offizielle Debian-Paket (``.deb``) von der Webseite zu installieren.


Erstellen eines Scanner-Profils
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Nach dem ersten Start von NAPS2 müssen Sie ein Profil für Ihren Scanner erstellen:

1. Klicken Sie auf **Profile** und dann auf **Neu**.
2. Geben Sie dem Profil einen Namen (z. B. den Namen Ihres Scanners).
3. Wählen Sie unter Treiber **SANE-Treiber** (dies ist der Standard-Scan-Dienst unter Linux).
4. Klicken Sie auf **Gerät auswählen** und wählen Sie Ihren Scanner aus der Liste aus.
5. Bestätigen Sie mit **OK**. Jetzt können Sie über dieses Profil scannen.

OCR-Texterkennung (Suchbare PDFs erstellen)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Der größte Vorteil von NAPS2 ist die integrierte **OCR-Texterkennung** (Optical Character Recognition) auf Basis von *Tesseract*. 
Ein normaler Scan ist lediglich ein Foto des Dokuments, dessen Text Sie weder kopieren noch durchsuchen können. 
Durch OCR wird der Text im Bild erkannt und als unsichtbare, aber markier- und durchsuchbare Schriftebene hinter das Bild gelegt.

So aktivieren und nutzen Sie OCR in NAPS2:

1. Klicken Sie in der Menüleiste von NAPS2 auf **OCR**.
2. Setzen Sie den Haken bei **PDFs mittels OCR suchbar machen**.
3. Wählen Sie als Sprache **Deutsch** (German) aus. Sollte das Sprachpaket noch nicht auf Ihrem System vorhanden sein, lädt NAPS2 es automatisch im Hintergrund herunter.
4. Falls Sie mehrsprachige Dokumente scannen, können Sie über die Sprachverwaltung weitere Sprachen hinzufügen.
5. Klicken Sie auf **OK**.

Wenn Sie Ihre Scans nun über die Schaltfläche **PDF speichern** sichern, führt NAPS2 die Texterkennung durch. 
Das erzeugte PDF-Dokument sieht optisch genauso aus wie der Original-Scan, aber Sie können nun Text mit der Maus markieren, 
kopieren und das Dokument in Ihrem Dateimanager nach beliebigen Wörtern durchsuchen.
