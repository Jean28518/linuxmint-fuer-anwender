==============================
Schlussworte & Best Practices
==============================

Herzlichen Glückwunsch!
Sie haben sich durch die wichtigsten Kapitel dieses Handbuchs gearbeitet und besitzen nun das Fundament,
um Linux Mint sicher, produktiv und stabil im Alltag zu nutzen.

Zum Abschluss möchte ich Ihnen mein wertvollstes Wissen aus über 10 Jahren Linux-Support und tausenden Sitzungen mitgeben.
Linux ist flexibel, aber diese Flexibilität verleitet oft zu Fehlern.
Wenn Sie die folgenden Best Practices beherzigen, wird Ihr Linux Mint über Jahre hinweg wie ein Schweizer Uhrwerk laufen.


Die goldenen Best Practices für Linux-Anwender
==============================================

1. Die Systemphilosophie: Weniger ist mehr
------------------------------------------

* **Arbeite mit dem Standard:**
  Versuchen Sie so weit wie möglich mit den vorgegebenen Standards zu arbeiten,
  sei es bei der Dateistruktur, den System-Themes oder den Grundeinstellungen.
  Die Entwickler von Linux Mint haben sich bei diesen Vorgaben intensiv Gedanken über Stabilität und Ergonomie gemacht.
  Zu tiefgreifende optische oder strukturelle Eingriffe führen auf Dauer oft zu Fehlern bei Systemaktualisierungen.

* **Minimalismus gewinnt:**
  Halten Sie Ihr System schlank.
  Installieren Sie nur Programme, die Sie wirklich aktiv nutzen.
  Je mehr Software und ungenutzte Hintergrunddienste auf Ihrem System liegen,
  desto höher ist die Wahrscheinlichkeit für Konflikte.
  Misten Sie regelmäßig in Ihrer **Anwendungsverwaltung** aus und entfernen Sie Software,
  die Sie nicht mehr benötigen.

* **Lassen Sie sich nicht vom „Distro-Hopping“ blenden:**
  Es gibt Hunderte von Linux-Distributionen, und jede Woche wird eine neue „Revolution“ im Internet gehypet.
  Lassen Sie sich nicht verunsichern.
  Linux Mint ist aus gutem Grund eine der beliebtesten Distributionen weltweit:
  Es ist unaufgeregt, extrem stabil und einfach produktiv.

* **Vorsicht vor KI-Overengineering:**
  Künstliche Intelligenz ist ein mächtiges Werkzeug, neigt aber immer wieder dazu, Anwender zu „blenden“.
  KI-Modelle schlagen oft komplexe Terminal-Befehle oder tiefgreifende Systemänderungen vor,
  die für Ihr eigentliches Problem völlig überzogen sind.
  Vermeiden Sie es, Ihr System künstlich zu verkomplizieren.


2. Alltag, Pflege & Fehlervermeidung
------------------------------------

* **Dokumentieren Sie Ihre Schritte:**
  Machen Sie es sich zur Gewohnheit, alles zu dokumentieren, was Sie an Ihrem System verändern
  (z. B. installierte PPAs, spezielle Konfigurationen oder gelöste Probleme).
  Nutzen Sie dafür am besten das im Handbuch vorgestellte **Obsidian**.
  Wenn in zwei Jahren ein Problem erneut auftritt,
  werden Sie Ihrem vergangenen Ich für diese Notizen dankbar sein.

* **Das 3-Monate-Upgrade-Prinzip:**
  Wenn Linux Mint eine neue Hauptversion (z. B. den Sprung von Version 21 auf 22) veröffentlicht,
  müssen Sie nicht direkt am ersten Tag ein Upgrade durchführen.
  Warten Sie mindestens 3 Monate,
  am besten sogar **6 bis 9 Monate**.
  Zu diesem Zeitpunkt sind die ersten Kinderkrankheiten und Paketkonflikte durch Point-Releases bereits behoben,
  und Sie genießen ein absolut stressfreies Upgrade.

* **VMs zum Experimentieren nutzen:**
  Sie möchten eine neue Software, ein Skript oder eine andere Desktop-Umgebung testen?
  Tun Sie das niemals auf Ihrem Produktivsystem!
  Nutzen Sie dafür virtuelle Maschinen (VirtualBox oder KVM).
  Wenn dort etwas schiefgeht,
  löschen Sie die VM einfach,
  während Ihr Hauptsystem unangetastet bleibt.

* **Backups und Updates sind Gesetz:**
  Es gibt zwei Arten von Linux-Nutzern:
  Diejenigen, die Backups machen, und diejenigen, die noch nie Daten verloren haben (aber bald werden).
  Halten Sie Ihre Timeshift-Schnappschüsse und Datensicherungen aktuell.
  Zusammen mit regelmäßigen Updates ist das Ihre Lebensversicherung unter Linux.

* **Probleme selbst lösen stärkt das Wissen:**
  Wenn etwas nicht auf Anhieb funktioniert,
  versuchen Sie den Fehler zuerst selbst zu analysieren (Protokolle prüfen, gezielt suchen).
  Jedes selbst gelöste und dokumentierte Problem macht Sie unabhängiger und sicherer im Umgang mit Linux.


3. Erste Hilfe im Notfall
-------------------------

* **Der Live-USB-Stick in der Schublade:**
  Halten Sie *immer* einen bootbereiten Linux-Mint-Live-USB-Stick bereit.
  Sollte Ihr System nach einem Hardware-Defekt oder einem missglückten Experiment einmal nicht mehr starten,
  können Sie über den Stick booten,
  Ihre Daten retten oder das System mittels Timeshift im Handumdrehen reparieren.

* **Erste Hilfe bei hängenden Programmen:**
  Sollte sich der Cinnamon-Desktop oder ein Programm einmal aufhängen,
  müssen Sie den Rechner nicht hart ausschalten.
  Nutzen Sie diese Tastenkombinationen:

  * **Desktop neu starten:** Drücken Sie ``Alt`` + ``F2``, tippen Sie ein kurzes ``r`` ein und drücken Sie ``Enter``.
    Das startet die Cinnamon-Oberfläche im Hintergrund neu,
    ohne dass Ihre geöffneten Programme geschlossen werden.
  * **Programm abschießen (xkill):** Wenn ein einzelnes Fenster einfriert,
    öffnen Sie ein Terminal oder den Ausführen-Dialog (``Alt`` + ``F2``) und tippen Sie ``xkill`` ein.
    Ihr Mauszeiger wird zu einem Totenkopf/Kreuz.
    Klicken Sie auf das hängende Fenster, um es sofort hart zu beenden.

* **Sie sind nicht allein:**
  Wenn Sie einmal absolut nicht weiterwissen,
  scheuen Sie sich nicht, Hilfe zu suchen.
  Das **Linux Guides Forum** ist eine der freundlichsten Anlaufstellen im deutschsprachigen Raum.
  Alternativ gibt es fast überall lokale **LUGs (Linux User Groups)**,
  bei denen Sie sich persönlich bei einem Kaffee austauschen und gegenseitig helfen können.
  Natürlich biete ich Ihnen über Linux Guides auch kommerziellen Support an.



Empfohlene Software-Perlen für fortgeschrittene Einsatzzwecke
=============================================================

Ergänzend zu vielen Programmen aus den Hauptkapiteln finden Sie hier meine kuratierte Liste von Werkzeugen für spezielle Anwendungsfälle.
Die meisten davon lassen sich bequem als Flatpak oder über die Paketverwaltung installieren.

.. list-table:: Empfohlene Software
   :widths: 25 35 40
   :header-rows: 1

   * - Kategorie / Einsatzzweck
     - Empfohlene Software & Quelle
     - Beschreibung
   * - **Dokumentenverwaltung**
     - `Paperwork <https://flathub.org/de/apps/work.openpaper.Paperwork>`_ | `djpdf <https://flathub.org/apps/com.github.unrud.djpdf>`_
     - Perfekt, um gescannte Dokumente mit OCR-Texterkennung zu verwalten und durchsuchbar zu machen.
   * - **Erweitertes Scannen**
     - `NAPS2 <https://www.naps2.com/>`_ | `Skanpage <https://flathub.org/apps/org.kde.skanpage>`_
     - NAPS2 ist der Favorit für OCR. Skanpage ist eine hervorragende, schlanke KDE-Alternative für Mehrfachscans.
   * - **Desktop-Sicherheit**
     - `OpenSnitch <https://github.com/evilsocket/opensnitch>`_
     - Eine interaktive Anwendungs-Firewall für den Desktop (wie Little Snitch unter macOS). Meldet sofort, wenn ein Programm „nach Hause telefonieren“ will. Nur für die Nerds unter Ihnen.
   * - **Büro / Behörden**
     - `Quba Viewer <https://quba-viewer.org/>`_
     - Unverzichtbar im geschäftlichen Umfeld zur korrekten Anzeige von elektronischen Rechnungen (X-Rechnung / ZUGFeRD).
   * - **Finanzen & Banking**
     - `Hibiscus <https://www.willuhn.de/products/hibiscus/>`_ | `Portfolio Performance <https://www.portfolio-performance.info/>`_
     - Hibiscus ist die professionelle, quelloffene Banking-Software (unterstützt Chipkartenleser). Portfolio Performance trackt Ihre Aktien und Kurse.
   * - **Produktivität**
     - `Super Productivity <https://super-productivity.com/>`_
     - Ein genialer To-Do-Listen-Manager und Time-Tracker für strukturierte Projektplanung.
   * - **Notizen & Whiteboard**
     - `Xournal++ <https://github.com/xournalpp/xournalpp>`_ | `Rnote <https://flathub.org/apps/org.freedesktop.Rnote>`_ | Draw.io / Excalidraw
     - Xournal++ und Rnote sind perfekt für handschriftliche Notizen und Skizzen via Grafiktablet. Draw.io/Excalidraw eignen sich für Diagramme.
   * - **Total Commander Alternative**
     - ``doublecmd-gtk`` (Double Commander)
     - Ein mächtiger zweispaltiger Dateimanager im Stil des Total Commanders. Installation über die Anwendungsverwaltung: ``doublecmd-gtk``.
   * - **Zwischenablage**
     - ``copyq`` (CopyQ)
     - Ein erweiterter Zwischenablagen-Manager, der sich den Verlauf Ihrer kopierten Texte und Bilder merkt. Installation über die Anwendungsverwaltung: ``copyq``.
   * - **Systembereinigung**
     - `Czkawka <https://flathub.org/apps/com.github.qarmin.czkawka>`_ | `Raider <https://flathub.org/en/apps/com.github.ADBeveridge.Raider>`_
     - Czkawka findet zuverlässig Duplikate und leere Ordner. Raider schreddert sensible Dateien unwiederbringlich.
   * - **Hardware-Steuerung**
     - `Fan Control <https://flathub.org/apps/io.github.wiiznokes.fan-control>`_ | `Solaar <https://flathub.org/en/apps/io.github.pwr_solaar.solaar>`_ | `Piper <https://flathub.org/en/apps/org.freedesktop.Piper>`_ | `Input Remapper <https://github.com/sezanzeb/input-remapper>`_
     - *Fan Control* regelt die Lüfter. *Solaar* verwaltet Logitech-Geräte, *Piper* konfiguriert Gaming-Mäuse, und *Input Remapper* erlaubt freie Tastenbelegungen.
   * - **Audio-Routing**
     - `qpwgraph <https://flathub.org/apps/org.rncbc.qpwgraph>`_
     - Ein grafisches Verbindungsdiagramm für PipeWire. Erlaubt es, den Ton von App A digital direkt in App B umzuleiten.
   * - **Kamera & Grafik**
     - `Cameractrls <https://flathub.org/apps/hu.irl.cameractrls>`_ | `Gradia <https://flathub.org/de/apps/be.alexandervanhee.gradia>`_ | `InvokeAI <https://invoke.ai/>`_
     - *Cameractrls* stellt Webcams perfekt ein. *Gradia* hilft beim schnellen Bearbeiten von Screenshots. *InvokeAI* ist die Top-Adresse für lokale KI-Bildgenerierung.
   * - **Medien & Internet**
     - `YTDN <https://flathub.org/apps/io.github.aandrew_me.ytdn>`_ | Momentum | Expression Search NG
     - *YTDN* lädt YouTube-Videos unkompliziert herunter. *Momentum* ist ein Usenet-Reader. *Expression Search NG* peppt die Thunderbird-Suche massiv auf.
   * - **Label**
     - ``glabel`` (Geniustags / gLabels)
     - Hervorragendes Programm zum Gestalten und Drucken von Etiketten und Visitenkarten.