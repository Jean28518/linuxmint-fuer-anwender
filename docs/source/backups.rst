Backups
=======

Backups sind essenziell.
Sollten Sie einmal einen Fehler machen oder Ihr Rechner bzw. System kaputtgehen,
sind Ihre Daten nicht verloren.
Dafür empfehle ich Ihnen dringend eine große externe Festplatte,
die idealerweise in einem anderen Gebäude oder Zimmer gelagert wird.

Formatieren Sie die externe Festplatte mit dem Programm ``USB-Stick-Formatierer``.
Als Partitionstyp empfehle ich Ihnen beispielsweise ``ext4``.

Ich setze auf das darunterliegende Programm ``borg``.
Es komprimiert Backups,
kann diese verschlüsseln
und speichert in mehreren Iterationen nur veränderte Daten.
``borg`` wird von vielen Profis und Unternehmen unter Linux genutzt.

Da ``borg`` jedoch normalerweise eine Interaktion auf dem Terminal benötigt,
empfehle ich das Programm ``Pika Datensicherung``,
welches borg nutzt.
Sie können ``Pika Datensicherung`` ganz einfach aus der Anwendungsverwaltung installieren.
Es ist sehr einfach zu bedienen.


Einrichtung
-----------

- Stecken Sie Ihre externe Festplatte an und formatieren Sie diese gegebenenfalls.

.. note::
    Sollten Sie keine externe Festplatte besitzen,
    empfehle ich Ihnen für Backups dringend die Anschaffung einer solchen.
    Sollte Ihre Festplatte im Computer kaputtgehen oder Ihr Computer beispielsweise einen Wasserschaden erleiden,
    sind Ihre Daten ohne eine externe Festplatte in der Regel verloren.

- Installieren und starten Sie das Programm ``Pika Datensicherung``.
- Wählen Sie ``Datensicherung einrichten`` und wählen Sie unter ``Ein neues Sicherungsdepot anlegen`` den Eintrag ``Ort auf dem Datenträger``.
- Wählen Sie als Ort Ihre externe Festplatte aus.
  (Wenn Sie keine externe Festplatte zur Hand haben,
  wählen Sie Ihren persönlichen Ordner).
- Sollten Sie sensible Daten besitzen,
  wählen Sie ``Verschlüsselt``,
  andernfalls ``Unverschlüsselt``.

.. warning::
    Sollten Sie bei einem verschlüsselten Backup Ihr Passwort vergessen oder verlieren,
    gibt es keine Möglichkeit mehr,
    das Backup wiederherzustellen.

- Wählen Sie rechts oben ``Anlegen``.
- Nun können Sie unter ``Zu sichernde Dateien`` weitere Ordner hinzufügen.
  Standardmäßig wird der persönliche Ordner gesichert.
  Dies reicht in der Regel vollkommen aus.
  Sollten Sie weitere Partitionen wie beispielsweise ``/data`` nutzen,
  fügen Sie hier die entsprechenden Ordner hinzu.
- Bei ``Von Sicherung ausschließen`` empfehle ich Ihnen,
  folgende Ordner auszuschließen:

    - *(Sollten Sie als Datensicherungsort Ihren persönlichen Ordner ausgewählt haben, fügen Sie den entsprechenden Ordner hinzu. Er beginnt mit* ``backup`` *)*
    - ``Downloads``
    - ``Warpinator``
    - (``Tmp``)
    - (``VirtualBox VMs``)
    - (``.steam``)

.. warning::
    Sollten Sie Verknüpfungen in Ihrem persönlichen Ordner haben,
    werden diese vom Backup-Programm nicht verfolgt.
    Denken Sie daran,
    eventuell eine andere Partition zusätzlich zum Backup hinzuzufügen.


Durchführung
------------

Ich empfehle Ihnen,
Backups beispielsweise jede Woche oder jeden Monat auszuführen.
Schließen Sie Ihre externe Festplatte an,
öffnen Sie ``Pika Datensicherung`` und klicken Sie auf ``Back Up Now``.

.. note::
    Sollte die Datensicherung beim ersten Mal fehlschlagen,
    stellen Sie sicher,
    dass Sie Schreibrechte im ausgewählten Sicherungsort besitzen.
    Sollte dies nicht der Fall sein,
    müssen Sie die Einrichtung wiederholen.

Dieser Vorgang kann beim ersten Mal sehr lange dauern.
Starten Sie das Backup am besten direkt vor dem Feierabend.


Wiederherstellung von Daten
---------------------------

.. tip::
    Es ist sehr wichtig,
    dass Sie diesen Schritt einmal ausprobieren.
    Somit sind Sie auf einen Ernstfall vorbereitet und wissen,
    dass Ihr Backup funktioniert.

- Öffnen Sie das Backup-Verzeichnis in der ``Pika Datensicherung``.
  (Dieser Schritt ist nur nötig,
  falls Sie das Backup von einem anderen System aus öffnen.)
- Wählen Sie den Reiter ``Archive``.
- Wählen Sie Ihren gewünschten Zeitpunkt aus und wählen Sie ``Gesicherte Dateien öffnen``.
- Ein Dateimanager öffnet sich nun mit den Dateien.
  Kopieren Sie aus diesem Verzeichnis verschiedene Dateien auf Ihren Rechner.
  Die Zwei-Spalten-Ansicht mit ``F3`` empfehle ich Ihnen hierbei sehr.
- Am Ende wählen Sie im Pika-Datensicherungsprogramm ``Auswerfen`` aus (das Symbol dazu sehen Sie im Bild unten).

.. image:: images/pika_auswerfen.png


    
